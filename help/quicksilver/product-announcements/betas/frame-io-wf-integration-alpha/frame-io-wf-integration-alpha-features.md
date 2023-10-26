---
content-type: reference
navigation-topic: betas
title: "Adobe Workfront 및 Frame.io 기본 통합 알파: 기능"
description: Adobe Workfront 및 Frame.io 기본 통합 알파에 대해 계획된 기능
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Adobe Workfront 및 Frame.io 기본 통합 알파: 기능

## 사용 사례 및 기능 테스트

이 통합을 통해 크리에이티브가 원하는 도구(CC 또는 Frame.io)에 머무르며 컨텐츠 생성 및 피어 검토를 수행하는 동시에 프로젝트 관리자가 작업을 조정하고 Workfront 내부에서 공식 검토 프로세스를 초기화 및 모니터링할 수 있도록 하는 것이 목표입니다. 이는 Frame.io에서 제공하는 콘텐츠 검토 기능과 함께 콘텐츠 승인 관리를 위한 Workfront의 새 문서 승인이라는 두 가지 솔루션의 장점을 활용하여 달성할 수 있습니다. 전체적으로 새로운 문서 승인 및 Frame.io는 새로운 컨텐츠 검토 및 승인 환경을 형성합니다. 

알파의 작동 방식과 참여 방법에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 및 Frame.io 통합 알파: 개요](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>이 알파 프로그램에 귀사가 참여하지 않은 상태에서 이 페이지를 접한 경우, 여기에서 정보를 주의 깊게 처리하고 자세한 내용은 Workfront 또는 Frame.io 관리자에게 문의하십시오.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## 기능 계획

다음은 해결하고자 하는 주요 사용 사례와 현재 계획한 기능에 대한 정보입니다. <!--, along with documentation to get you started testing.-->


### Workfront 관리자는 Workfront 그룹과 Frame.io 계정 간의 연결을 설정할 수 있습니다

* _Workfront 내에서는 Workfront 그룹을 Frame.io 계정에 연결할 수 있습니다_

* 연결된 Workfront 그룹을 나타내는 Frame.io 내에 새 Frame.io 팀이 만들어집니다

**향후 릴리스에서 잠재적인 개선 사항:**

* Frame.io 계정에서 Workfront 그룹 연결 끊기

* 기존 Frame.io 팀에 Workfront 그룹 연결

### 프로젝트 코디네이터는 Frame.io로 전송되는 Workfront 프로젝트를 구성하고, 할당된 Workfront 크리에이티브를 Frame.io의 프로젝트에 추가하도록 할 수 있습니다.

* Frame 연결 그룹을 할당하여 활성화된 Frame.io로 Workfront 프로젝트를 표시하는 기능

* _개선 사항: Workfront 프로젝트 내의 작업을 프레임 작업으로 전환하여 Frame.io 내에 작업 폴더를 만드는 기능_

* Workfront 프로젝트 상태를 현재로 설정하면 연결된 프로젝트가 프레임에 만들어지고 Workfront에서 할당한 사용자가 프레임 프로젝트에 추가되고 Frame.io에서 이메일 알림이 전송됩니다

   * 모든 Workfront 프로젝트 멤버(사용자 및 팀)는 프로젝트 생성 시 Frame.io 프로젝트에 공동 작업자로 추가됩니다.

   * _변경: 프레임 사용 Workfront 작업에 할당된 사용자 및 팀은 Frame.io 프로젝트에 공동 작업자로 추가되고 알림을 받습니다(프로젝트 생성 및 이후 시)_

* 프로젝트 및 프레임 사용 작업에 추가된 문서(Creative Brief)는 프로젝트가 만들어지면(트리거: 프로젝트 상태를 현재로 설정) Frame.io 프로젝트(각 작업 폴더 내)로 푸시됩니다.

   * Frame.io로 불필요한 여러 문서를 보내지 않도록 Creative Brief만 활성화하기 전에 프로젝트에 추가되는 문서의 양을 제한하는 것이 좋습니다

* _개선 사항: 프레임 사용 Workfront 작업에서 명시적으로 할당 해제된 사용자/팀은 Frame.io 프로젝트에서 제거됩니다_

**향후 릴리스에서 잠재적인 개선 사항:**

* 프레임 사용 작업은 프로젝트 템플릿에서 구성할 수 있습니다.

* Creative Brief에 대한 새 버전 업로드가 프레임으로 푸시됨

* 최적화된 프로젝트 동기화 (프로젝트 연결 해제, 프로젝트 및 문서 재동기화 등)

### Frame.io 내에서 크리에이티브는 공식 검토를 위해 생성된 에셋을 Workfront 프로젝트에 보낼 수 있습니다

* 단일 Frame.io 자산을 WF 프로젝트 또는 작업에 연결하는 기능입니다. Workfront 내에 에셋 참조가 만들어집니다.

* Frame.io 내의 새 버전 업로드는 연결된 자산에서 Workfront 내의 새 문서 버전을 자동으로 만듭니다.

* _개선 사항: 참조된 Workfront 작업을 Frame.io 내에서 완료된 것으로 표시하는 기능_

* _개선 사항: 연결된 Workfront 문서가 삭제되면 Frame.io 내에 유지되며 동일한 프로젝트 작업 또는 다른 프로젝트 작업에 다시 연결할 수 있습니다_

**향후 릴리스에서 잠재적인 개선 사항:**

* 여러 Frame.io 자산을 한 번에 Workfront에 보낼 수 있는 기능

* Frame.io 내에서 Workfront 프로젝트/작업에 대한 시간 로깅

### 프로젝트 코디네이터는 Frame.io에서 링크된 문서에 공식 승인 프로세스를 할당할 수 있습니다.

* Workfront 사용자 및 팀을 Frame.io 연결 문서에 대한 새 문서 승인에 추가할 수 있습니다.

* _개선 사항: 사용자/팀이 프레임 활성화 문서에서 공유되지 않으면 Frame.io 뷰어의 자산에 대한 액세스 권한도 상실됩니다._

**향후 릴리스에서 잠재적인 개선 사항:**

* 여러 에셋을 단일 검토로 전송

* Workfront 문서에 승인자/검토자 일괄 할당

### 이해 당사자는 Frame.io Viewer 내에서 검토 및 승인을 수행할 수 있습니다.

* 이해 당사자에게 알림이 전송되며 Frame.io 뷰어 내에서 Frame 연결된 문서를 볼 수 있습니다.

* Frame.io 뷰어는 Workfront 내의 다른 위치(예: 문서 목록, 문서 세부 정보, Workfront 홈)에서 액세스할 수 있습니다

* Workfront의 업데이트 스트림과 동기화되는 Frame.io 뷰어에서 제공하는 기존 검토 및 주석 달기 기능을 활용하는 기능

* _Frame.io 뷰어 내에서 새 문서 승인 결정을 내리는 기능_

### Frame.io 내에서 크리에이티브에게 연결된 Frame.io 자산에 대해 결정된 전반적인 사항에 대해 알려줍니다

* _개선 사항: 전체 문서 승인 상태가 Frame.io 내의 자산에 표시됩니다._

### 프로젝트 코디네이터는 최종 에셋을 AEM에 보낼 수 있습니다.

* _개선 사항: 기존 Workfront + AEM Asset CS 커넥터를 사용하여 메타데이터를 비롯한 프레임에 연결된 문서를 AEM으로 보낼 수 있습니다._