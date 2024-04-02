---
product-area: documents
navigation-topic: approvals
title: 자산 검토 및 승인 개요
description: Workfront의 공식 검토 및 승인 프로세스에 대해 자세히 알아보십시오.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: b0bd63012d86f38db238b555d21a1c51b0a8b165
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# 자산 검토 및 승인 개요

새로운 에셋 검토 및 승인 워크플로우는 Workfront과 Frame.io 간의 긴밀한 통합을 기반으로 구축됩니다. 이 통합은 각 제품이 제공하는 기능을 최대한 활용하고 이를 결합하여 콘텐츠 작성에 관여하는 모든 사용자가 선택한 도구에서 작업할 수 있는 환경을 만드는 동시에 두 시스템 간에 실시간으로 동기화된 주석, 파일 및 상태 업데이트에 액세스할 수 있습니다.

<!-- link to frame docs-->

## Workfront의 작업 시작 및 계획

프로젝트 코디네이터는 Workfront에서 시작합니다. 프로젝트가 생성되고, 작업이 할당되고, 지침이 전송됩니다.

프로젝트 코디네이터는 WF 프로젝트를 생성하고, 동기화된 프로젝트 폴더를 사용하여 Frame.io 내의 크리에이티브에 정보 및 지원 자료를 보냅니다.

처음부터 또는 템플릿을 통해 승인 작업 과정 설정

작업 할당

프로젝트를 현재 또는 같게 설정하여 프레임 프로젝트 및 경고 크리에이티브 만들기

### 기본 Frame.io 계정 구성

Workfront 관리자는 Workfront의 설정 영역에서 기본 Frame.io 계정을 추가하여 Workfront 및 Frame.io 통합을 활성화합니다. 기본 Frame.io 계정이 설정되면 통합에서 Workfront과 Frame.io 간에 연결된 프로젝트를 만들 수 있습니다.

자세한 내용은 [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### Frame.io 사용자 활성화

Frame.io를 정기적으로 사용하는 Workfront 사용자는 Frame.io 사용자로 표시되어야 합니다. Workfront 관리자는 Workfront 사용자 프로필에서 Frame.io 사용자를 지정할 수 있습니다.

사용자가 Workfront에서 Frame.io 사용자로 표시되고 프로젝트에 추가되면 다음과 같이 됩니다.

* Frame.io에서 공동 작업자로 추가됩니다
* 정식 검토 및 승인을 위해 Frame.io에서 Workfront으로 자산을 전송할 수 있습니다.

자세한 내용은 [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>크리에이티브 도구에서 정기적으로 작업하고 검토 및 승인을 위해 에셋을 업로드하는 사용자를 Frame.io 사용자로 활성화하는 것이 좋습니다.

### Frame.io와 연결된 프로젝트 만들기

프로젝트 코디네이터는 Frame.io와 연결된 Workfront 프로젝트를 만들 수 있습니다. 연결된 프로젝트를 만들 때 다음과 같은 작업을 수행할 수 있습니다

* **작업에 Frame.io 사용자 할당**: Frame.io를 사용하는 사용자는 완료해야 할 작업이 있음을 알리는 작업에 할당되면 이메일로 알림을 받습니다.
* **Frame.io 사용자와 프로젝트 공유**: Frame.io가 활성화된 사용자와 공유된 프로젝트는 Frame.io 내의 프로젝트에 대한 액세스 권한을 부여합니다.
* **Frame.io와 크리에이티브 자료 공유**: 단방향 동기화 프로젝트 폴더를 사용하여 Workfront의 지침과 자료를 Frame.io의 크리에이티브 사용자에게 직접 보낼 수 있습니다.
* **작업 진행 추적**: 크리에이티브는 Frame.io를 종료하지 않고 완료된 에셋을 보내고 작업을 완료로 표시할 수 있습니다.

자세한 내용은 [].

<!--Preassign approval templates to asks coming in the future-->


## Frame.io의 컨텐츠 제작 및 공동 작업

크리에이티브는 자신이 선택한 도구에 머무르며 Frame.io 내에서 동료 리뷰를 만들고 반복하고 수행할 수 있는 자유를 가질 수 있습니다.

크리에이티브가 통합 프로젝트에 추가되면 Frame.io를 종료하지 않고 다음 작업을 모두 수행할 수 있습니다.

* 프로젝트 코디네이터의 액세스 지침
* 비공식 동료 검토 수행
* 공식적인 검토 및 승인을 위해 완료된 에셋을 Workfront으로 전송
* 작업 상태 변경 또는 완료 표시
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## Workfront에서 에셋 검토 및 승인

크리에이티브가 완성된 에셋을 Frame.io에서 Workfront으로 전송하면 프로젝트 코디네이터는 Workfront의 공식 검토 및 승인 프로세스를 시작할 수 있습니다. 모든 검토 및 승인 활동이 Workfront에 기록됩니다.

Frame.io에서 작성한 주석은 Workfront의 업데이트 탭에도 반영됩니다. Workfront에서 만든 답글은 Frame.io에서 반영되지 않습니다.

Team only라고 표시된 댓글은 Workfront 업데이트 탭에 표시되지 않습니다.

### 공식 검토 및 승인 시작

일회성 검토 및 승인을 생성하거나 workfront의 설정 영역에서 재생성 가능한 승인 템플릿을 생성할 수 있습니다.

검토자, 승인자 또는 두 가지 모두를 혼합하여 할당할 수 있습니다.

* **검토자** 은 자산을 주석 및 마크업할 수 있습니다. 완료되면 검토를 완료된 것으로 표시할 수 있습니다. <!--example of when to add reviewers-->
* **승인자** 은(는) 주석 달기, 마크업 자산을 할 수 있으며 승인 프로세스를 진행하도록 결정해야 합니다.

검토자 및 승인자를 일회용 또는 승인 템플릿에 추가할 수 있습니다.

<!--can also assign teams and set deadline-->

* **일회용 승인**: 승인 마감 설정

* **승인 템플릿**
Workfront 설정 영역에서 Standard 라이선스를 가진 사용자는 다시 생성 가능한 승인 템플릿을 만들 수 있습니다. 템플릿 내에서 사용자는 일정을 지정하고 검토자와 승인자를 추가할 수 있습니다. <!--do we want to mention any upcoming plans here? -->

  템플릿이 생성되면 Frame.io에서 전송된 자산에 적용하여 Workfront에서 공식 검토 및 승인 프로세스를 시작할 수 있습니다.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### 검토 및 승인 알림

다른 섹션과 결합하시겠습니까?

홈 내 승인 위젯 이메일 대기 중 - 기한 이메일 72, 24 및 마감일

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### 에셋 검토 및 승인

Frame.io 연결된 자산 이해 당사자는 프레임 뷰어 내에서 workfront 업데이트 스트림, 의사 결정 등과 동기화되는 주석을 검토하고 승인할 수 있습니다

<!-- include screenshot from frame.io-->

외부 WF 사용자에게 프레임에 대한 로그인을 만들라는 메시지가 표시됩니다.

자산이 프레임에 연결되지 않은 경우 WF에서 썸네일을 보고 주석 스트림을 사용할 수 있습니다. 검토 및 승인 결정을 내릴 수 있습니다.

### 검토 및 승인 지표 추적

홈 승인 속도 보고서의 위젯

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* Workfront에서 에셋을 업로드하고 검토 및 승인을 위해 프레임으로 보냅니다. 곧 지원됩니까?

## 캠페인 자산 승인 워크플로우 예

소개 파라?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
