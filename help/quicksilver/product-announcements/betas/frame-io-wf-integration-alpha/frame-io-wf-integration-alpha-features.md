---
content-type: reference
navigation-topic: betas
title: "Adobe Workfront 및 Frame.io 기본 통합 알파: 기능"
description: Adobe Workfront 및 Frame.io 기본 통합 알파에 대해 계획된 기능
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 9e6033e495e83afa994b21996a4026ac484045a0
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Adobe Workfront 및 Frame.io 기본 통합 알파: 기능 및 테스트

이 통합을 통해 크리에이티브가 원하는 도구(CC 또는 Frame.io)에 머무르며 컨텐츠 생성 및 피어 검토를 수행하는 동시에 프로젝트 관리자가 작업을 조정하고 Workfront 내부에서 공식 검토 프로세스를 초기화 및 모니터링할 수 있도록 하는 것이 목표입니다. 이는 Frame.io에서 제공하는 콘텐츠 검토 기능과 함께 콘텐츠 승인 관리를 위한 Workfront의 새 문서 승인이라는 두 가지 솔루션의 장점을 활용하여 달성할 수 있습니다. 전체적으로 새로운 문서 승인 및 Frame.io는 새로운 컨텐츠 검토 및 승인 환경을 형성합니다. 

알파의 작동 방식과 참여 방법에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 및 Frame.io 통합 알파: 개요](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>이 알파 프로그램에 귀사가 참여하지 않은 상태에서 이 페이지를 접한 경우, 여기에서 정보를 주의 깊게 처리하고 자세한 내용은 Workfront 또는 Frame.io 관리자에게 문의하십시오.
>

## 데모 비디오

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## 기본 테스트 시나리오

알파 프로그램의 새로운 기능을 쉽게 테스트할 수 있도록 새로운 테스트 Frame.io 계정을 만들고 다음과 같은 새 그룹에 연결했습니다. `Frame.io alpha testing` 기존 Workfront 미리보기 또는 샌드박스 환경에서.

기능을 테스트하려면 Workfront 미리보기 또는 샌드박스 인스턴스에 로그인하고 다음 단계를 수행하십시오.

1. **코디네이터:** Workfront 내에서 `Frame.io alpha testing` 프로젝트 그룹으로 할당된 그룹.

1. **코디네이터:** Workfront 내에서 크리에이티브 작업이 필요한 작업을 프레임 사용(작업 세부 정보에서)으로 표시하고 크리에이티브를 이 작업에 할당합니다(전체 워크플로우를 테스트하려는 경우 자신을 할당).

>[!NOTE]
>
>하위 작업은 프레임을 사용하도록 설정한 것으로 표시할 수 없습니다.
>

1. **코디네이터:** Creative Brief를 업로드하고 프로젝트 상태를 &quot;현재&quot;로 변경합니다.

1. **광고:** 새로 만든 Frame.io 프로젝트에 대한 초대를 위해 이메일을 확인하십시오.

1. **광고:** 초대 이메일의 &quot;프로젝트 참여&quot; 버튼을 클릭하여 Frame.io 프로젝트에 참여하고, 프로젝트 내의 Creative Brief를 검토하고, 선택한 Creative Cloud 도구에서 컨텐츠 생성을 시작합니다.

1. **광고:** 생성된 에셋을 Frame.io에 업로드하고 할당된 프레임 사용 작업 중 하나를 선택하여 연결된 Workfront 프로젝트에 추가합니다. 작업을 완료로 표시하려면 옵션을 선택합니다.

1. **코디네이터:** Workfront 내에서 프레임 지원 작업에서 연결된 Frame.io 자산을 찾아 작업의 상태가 &quot;완료&quot;로 변경되었는지 확인합니다.

1. **코디네이터:** 연결된 Frame.io 자산에 검토자/승인자를 할당합니다. 전체 워크플로우를 테스트하려면 자신을 승인자로 지정하십시오. (검토/승인자 지정에 대한 자세한 내용은 [문서에 승인자 또는 검토자 추가](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **이해 당사자:** Workfront 내에서 홈, 문서 세부 정보 또는 수신한 이메일 알림에서 승인 요청을 봅니다. Frame.io 뷰어에서 에셋을 열고 피드백이 포함된 댓글을 남긴 다음 의사 결정을 합니다.

1. **코디네이터:** Workfront 내에서 Frame.io 연결 문서의 업데이트 섹션 내에서 관련자가 작성한 댓글과 승인 섹션 또는 문서 요약 창 내의 결정을 봅니다.

1. **광고:** Frame.io 내에서 자산에 대해 결정된 전반적인 승인 결정을 확인합니다.

1. **광고:** Frame.io 내에서 업데이트된 버전을 연결된 자산의 버전 스택에 추가하여 요청된 변경 사항을 적용합니다.

1. **코디네이터:** Workfront 내에서 승인자/검토자를 새로 업로드한 버전에 할당하고 로그오프에 도달할 때까지 진행 상황을 모니터링합니다.

## 자세한 테스트 시나리오

추가 기능을 테스트하려는 참가자를 위해 더 많은 관련 테스트 시나리오를 만들었습니다. 이 세부 테스트 시나리오에 대한 안내서는 여기에서 다운로드할 수 있습니다. [WF + Frame.io 상세 테스트 시나리오 연습](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## 기능 계획

다음은 해결하고자 하는 주요 사용 사례와 현재 계획한 기능에 대한 정보입니다. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>아래에 글머리 기호 **&quot;향후 릴리스에서 잠재적인 개선 사항&quot;** 알파 피드백 및 발전하는 개발 계획에 따라 헤더가 향후 릴리스에 포함될 수도 있고 포함되지 않을 수도 있습니다.
>

### Workfront 관리자는 Workfront 그룹과 Frame.io 계정 간의 연결을 설정할 수 있습니다

* Workfront 내에서는 Workfront 그룹을 Frame.io 계정에 연결할 수 있습니다

* 연결된 Workfront 그룹을 나타내는 새 Frame.io 팀이 Frame.io 내에 만들어집니다(이 기능은 프로덕션에서 통합을 사용하는 고객에게만 활성화되었습니다.). 샌드박스 또는 미리보기에서 테스트하는 고객은 Adobe 팀이 연결을 구성합니다.)

**향후 릴리스에서 잠재적인 개선 사항:**

* Frame.io 계정에서 Workfront 그룹 연결 끊기

* 기존 Frame.io 팀에 Workfront 그룹 연결

### 프로젝트 코디네이터는 Frame.io로 전송되는 Workfront 프로젝트를 구성하고, 할당된 Workfront 크리에이티브를 Frame.io의 프로젝트에 추가하도록 할 수 있습니다.

* Frame 연결 그룹을 할당하여 활성화된 Frame.io로 Workfront 프로젝트를 표시하는 기능

* Workfront 프로젝트 내의 작업을 프레임 작업으로 전환하여 Frame.io 내에 작업 폴더를 만드는 기능

* Workfront 프로젝트에 프레임 연결 그룹이 할당되고 하나 이상의 프레임 사용 작업이 있는 경우 Workfront 프로젝트 상태가 현재로 설정되면 연결된 프로젝트가 프레임에서 생성되고 Workfront 할당 사용자가 프레임 프로젝트에 추가되며 Frame.io에서 이메일 알림이 전송됩니다

   * 프레임 사용 Workfront 작업에 할당된 사용자 및 팀은 Frame.io 프로젝트에 공동 작업자로 추가되고 알림을 받습니다(프로젝트 생성 및 이후 시)

* 프로젝트 및 프레임 사용 작업에 추가된 문서(Creative Brief)는 프로젝트가 만들어지면(트리거: 프로젝트 상태를 현재로 설정) Frame.io 프로젝트(각 작업 폴더 내)로 푸시됩니다.

   * Frame.io로 불필요한 여러 문서를 보내지 않도록 Creative Brief만 활성화하기 전에 프로젝트에 추가되는 문서의 양을 제한하는 것이 좋습니다

   * 초기 프로젝트 동기화 후 추가된 문서/작업은 Frame.io로 푸시되지 않고 사용자/팀만 푸시됩니다.

**향후 릴리스에서 잠재적인 개선 사항:**

* 프레임 사용 작업은 프로젝트 템플릿에서 구성할 수 있습니다.

* Creative Brief에 대한 새 버전 업로드가 프레임으로 푸시됨

* 최적화된 프로젝트 동기화 (프로젝트 연결 해제, 프로젝트 및 문서 재동기화 등)

### Frame.io 내에서 크리에이티브는 공식 검토를 위해 생성된 에셋을 Workfront 프로젝트에 보낼 수 있습니다

* 단일 Frame.io 자산을 WF 프로젝트 또는 작업에 연결하는 기능입니다. Workfront 내에 에셋 참조가 만들어집니다.

* Frame.io 내의 새 버전 업로드는 연결된 자산에서 Workfront 내의 새 문서 버전을 자동으로 만듭니다.

* Frame.io 내에서 참조된 Workfront 작업을 완료로 표시하는 기능

* 연결된 Workfront 문서가 삭제되는 경우 Frame.io 내에 유지되며 동일한 프로젝트 작업 또는 다른 프로젝트 작업에 다시 연결할 수 있습니다

**향후 릴리스에서 잠재적인 개선 사항:**

* 여러 Frame.io 자산을 한 번에 Workfront에 보낼 수 있는 기능

* Frame.io 내에서 Workfront 프로젝트/작업에 대한 시간 로깅

### 프로젝트 코디네이터는 Frame.io에서 링크된 문서에 공식 승인 프로세스를 할당할 수 있습니다.

* Workfront 사용자 및 팀을 Frame.io 연결 문서에 대한 새 문서 승인에 추가할 수 있습니다.

* 사용자/팀이 프레임 사용 문서에서 공유되지 않으면 Frame.io Viewer의 자산에 대한 액세스 권한도 상실됩니다

**향후 릴리스에서 잠재적인 개선 사항:**

* 여러 에셋을 단일 검토로 전송

* Workfront 문서에 승인자/검토자 일괄 할당

### 이해 당사자는 Frame.io Viewer 내에서 검토 및 승인을 수행할 수 있습니다.

* 이해 당사자에게 알림이 전송되며 Frame.io 뷰어 내에서 Frame 연결된 문서를 볼 수 있습니다.

* Frame.io 뷰어는 Workfront 내의 다른 위치(예: 문서 목록, 문서 세부 정보, Workfront 홈)에서 액세스할 수 있습니다

* Workfront의 업데이트 스트림과 동기화되는 Frame.io 뷰어에서 제공하는 기존 검토 및 주석 달기 기능을 활용하는 기능

* Frame.io 뷰어 내에서 새 문서 승인 결정을 내리는 기능
