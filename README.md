# Bolg to Github.io

[https://2jh200234.github.io](https://2jh200234.github.io) <<최종 블로그 주소

## *시작*
  1. github 페이지에서 <username>.github.io라는 이름의 public repositories를 생성한다.
  2. 이 repositories의 주소를 복사한 뒤 CMD를 실행한다.
  3. $git clone <주소> <폴더명>을 입력해 <폴더명>으로 clone을 생성한다.

## *테마 적용*
  1. [Clean Blog](https://jekyllthemes.io/theme/startbootstrap-clean-blog-jekyll) 테마를 이용했다.
  2. [Clean Blog Github](https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll) 사이트에서 fork 기능을 이용해 나의 github로 가져왔다.
  3. 위의 시작과정을 다시 진행해 나의 블로그에 Clean Blog 테마를 적용했다.
  
 ## *포스트*
  1. _posts 폴더 내에 새로운 .md 파일을 생성한다.
  2. 상단에 
     ---
     layout: post
     title:  "<제목>"
     date:   "<날짜>"
     categories: jekyll update
     comments: true
     ---
     를 순서대로 입력한다. comments는 후에 댓글 기능을 추가하기 위해 작성되었다.
  3. 추가한 파일을 github blog에 연동한다.
     $git status
     $git add .
     $git commit -m "post"
     $git push origin main 
     명령어를 명령프롬포트 창, clone된 폴더 위치에서 순서대로 입력한다.
  4. 블로그 주소를 들어가 변경사항을 확인한다.
  
 ## *댓글*
  1. disqus 가입을 한 뒤 universer code를 획득한다.
  2. _posts 폴더의 댓글을 활성화 하고싶은 글의 .md파일에서 comments: true 줄을 추가한다. (포스트 -2)
  3. _layouts 폴더의  post.html 파일에 universer code를 붙여넣은 뒤 수정을 한다.
     수정된 코드의 내용은 다음과 같다.
     {% if page.comments %}
     <h2>Comments</h2>
     <div id="disqus_thread"></div>
     <script>
         /**
          *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
          *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables
          */
         let PAGE_URL = "{{site.url}}{{page.url}}"
         let PAGE_IDENTIFIER = "{{page.url}}"
         var disqus_config = function () {
             this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
             this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
         };
          (function() {  // DON'T EDIT BELOW THIS LINE
             var d = document, s = d.createElement('script');
             s.src = 'https://2jh200234.disqus.com/embed.js';
             s.setAttribute('data-timestamp', +new Date());
             (d.head || d.body).appendChild(s);
          })();
     </script>
     <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>
     {% endif %}
  4. 수정한 내용을 저장하기 위해 포스트 3번 내용의 명령어를 다시 입력해준다.
  5. 블로그 주소를 통해 확인하면 끝
  
## *시행착오*
  1. 테마를 적용하는 과정에서 $jekyll new . --force 명령어가 적용되지 않는 문제가 발생했다.
     기존 테마의 jekyll 버전과 나의 버전이 일치하지 않아 생긴 문제라고 생각했고, 적용 가능한 다른 테마를 찾았다.
  2. %bundle exec jekyll serve 명령어 사용 중 오류가 발생했다.
     변경사항의 push 기능을 이용하는데엔 문제가 없어 그대로 이용했다.
     다만 로컬 서버에서 나의 블로그를 열어볼 수 없어 변경 사항을 곧바로 확인하는 부분에서 어려움을 겪었다.
  
  
