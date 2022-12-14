---
layout: post
title:  "Git과 Github"
date:   2022-11-29 01:37:32 +0900
categories: jekyll update
comments: true
---
## *Git이란?*
Git은 가장 일반적으로 사용되는 버전 관리 시스템(version control system)이다.
Git은 파일에 대한 변경 내용을 추적하므로 수행된 작업에 대한 기록이 있으며 필요할 경우 특정 버전으로 되돌릴 수 있다.
Git은 또한 협업을 더 쉽게 만들어 여러 사람의 변경 사항을 모두 하나의 소스로 병합할 수 있다.

Git은 로컬로 실행되는 소프트웨어이다. 
파일과 파일 기록이 컴퓨터에 저장된다. 
또한 온라인 호스트(예: GitHub 또는 Bitbucket)를 사용하여 파일의 복사본과 해당 수정 기록을 저장할 수 있다. 
변경사항을 업로드하고 다른 개발자의 변경사항을 다운로드할 수 있는 중앙 위치에 있으므로 다른 개발자와 더 쉽게 협업할 수 있게된다. 
Git은 자동으로 변경 사항을 병합할 수 있으므로 두 사람이 같은 파일의 다른 부분을 작업하고 
나중에 서로의 작업을 잃지 않고 변경 사항을 병합할 수 있는 장점을 가지고있다.

Git이 파일을 저장하기 위해선 Commit을 남겨야한다.

## *Github의 장점 I - 협업의 효율화*
GitHub를 사용하는 가장 첫번째 이유는 바로 버전 제어 및 액세스 제어를 포함한 일련의 프로젝트 협업 기능입니다.

GitHub의 장점을 보여주기 위해 다음 시나리오를 가정 해봅시다. 당신은 온라인 게임을 코딩하고 싶고, 당신의 친구에게 도움을 청합니다. GitHub에 현재 및 이전 버전을 포함한 모든 파일을 저장하는 Repo를 만든 다음 친구 공동작업자에게 이 Repo에 대한 액세스 권한도 부여합니다.

파트너가 게임 메뉴 및 설정 화면을 처리하는 동안 기본 게임 플레이 및 화면에서 작업하기로 결정합니다. 다른 사람의 작업을 방해하지 않고 두 사람이 동시에 변경 사항을 추진하기 위해 팀 동료가 화면을 작성할 수 있는 별도의 개발 영역인 Branch를 만듭니다. 그러는 동안, 당신은 당신의 지점에서 일을 계속합니다.

당신의 친구가 그들의 일을 마치면, 그들은 당신의 일과 그들의 일을 Merge해 달라는 PR(Pull Request)을 할 수 있습니다. 승인하면 branch를 merge하여 코드를 병합할 수 있습니다.

이제 다른 개발자가 게임의 Repo를 보고 멀티플레이어 모드를 추가할 아이디어를 가지고 있다고 가정해 봅시다. 사용자는 리포지토리를 Fork하거나 자체 복사본을 만든 다음 새 기능을 추가할 수 있습니다. 완료되면 pull request을 제출할 수 있습니다. 승인된 이후에는 이 fork된 Repo가 사용자의 Repo와 merge되고 이제 게임은 멀티플레이어가 됩니다! Public Repo는 누구나 branch를 만들 수 있지만 PR을 수락하거나 거부할지는 Repo 소유자에게 달려 있습니다.

물론 처음부터 완벽한 소프트웨어는 없습니다. 따라서 Github Repo에는 할 일을 나열하고 게임의 문제를 보고하고 토론하고 해결한 것으로 표시하기 위한 Issue 섹션도 있습니다. 이러한 문제를 해결하려면 파일의 변경 로그를 다시 검토하여 문제가 발생한 시기와 위치를 확인할 수 있습니다.

요약하자면, GitHub는 몇 명, 수십 명, 심지어 수천 명의 개발자가 다른 사람의 작업을 무시하거나 변경 사항을 추적할 걱정 없이 프로젝트에 원활하게 기여할 수 있는 Centralized Workspace을 제공합니다.



## *Github의 장점 II - 쉬운 파일 관리*
GitHub는 Git 위에 그래픽 사용자 인터페이스(GUI) 계층을 추가합니다. Git는 자체적으로 Command Line(컴퓨터의 Command Line Interface)을 통해 작동합니다. 개발자는 명령줄을 사용하는 방법을 알고 있지만 대부분의 경우 명령줄이 파일과 상호 작용하는 가장 효율적인 방법은 아닙니다.

GitHub의 인터페이스는 Git 작업을 수행하고 파일 기록을 볼 수 있는 깨끗하고 사용자 친화적인 수단을 제공합니다. 이것은 개발자에게 더 편리하고 Git에 정통한 초보자에게 더 쉽게 접근할 수 있습니다.

GitHub에 더 쉽게 액세스할 수 있는 또 다른 이점은 클라우드 기반 인프라입니다. GitHub 사용자는 모든 위치 및 장치에서 저장소에 액세스하고 리포지토리를 다운로드하고 변경사항을 적용할 수 있습니다. GitHub를 사용하는 것은 하나의 장치나 환경에 제한되지 않는다는 것을 의미합니다


## *Github의 장점 III - 엔지니어들의 SNS*
GitHub 사용자들에게 Github는 단순히 코드를 작업하는 장소가 아닙니다. 모든 GitHub 사용자는 자신의 프로젝트, 기여 및 활동을 사이트에 표시할 수 있는 프로필을 가지고 있으며 모든 사용자의 공개 프로필 및 Repository를 볼 수 있습니다.

GitHub의 소셜 네트워크는 개발자들이 모든 종류의 오픈 소스 프로젝트를 탐색하고 기여하도록 장려하기 때문에 개발자로서의 성장에 매우 중요한 역할 중 하나로 자리매김했습니다. 이전에는 프로젝트에 기여를 하고싶은 사람이 프로젝트 소유자에게 직접 연락하여 기여 허가를 요청해야 했습니다. GitHub를 사용하면 프로젝트를 fork한 다음 PR을 하는 것만큼 쉽습니다. 그런 다음 프로젝트 소유자는 요청을 수락하기 전에 누군가의 프로필과 과거 기여도를 검토할 수 있습니다.

GitHub는 또한 고용주들을 위한 프로젝트를 보여주는 하나의 방법으로, 일종의 포트폴리오 역할을 합니다. 예를 들어, 잠재 고객의 코드는 누구나 검토할 수 있기 때문에 채용 담당자들은 종종 인재를 스카우트하기 위해 Github를 사용합니다.
