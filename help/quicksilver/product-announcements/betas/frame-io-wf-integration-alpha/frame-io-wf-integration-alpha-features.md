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
source-git-commit: 02e55be36d3b649aeb5b81d185538f77ac3d4ec7
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 0%

---

# Adobe Workfront 및 Frame.io 기본 통합 알파: 기능 및 테스트

이 통합을 통해 크리에이티브가 원하는 도구(CC 또는 Frame.io)에 머무르며 컨텐츠 생성 및 피어 검토를 수행하는 동시에 프로젝트 관리자가 작업을 조정하고 Workfront 내부에서 공식 검토 프로세스를 초기화 및 모니터링할 수 있도록 하는 것이 목표입니다. 이는 Frame.io에서 제공하는 콘텐츠 검토 기능과 함께 콘텐츠 승인 관리를 위한 Workfront의 새 문서 승인이라는 두 가지 솔루션의 장점을 활용하여 달성할 수 있습니다. 전체적으로 새로운 문서 승인 및 Frame.io는 새로운 컨텐츠 검토 및 승인 환경을 형성합니다. 

알파의 작동 방식과 참여 방법에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 및 Frame.io 통합 알파: 개요](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>이 알파 프로그램에 귀사가 참여하지 않은 상태에서 이 페이지를 접한 경우, 여기에서 정보를 주의 깊게 처리하고 자세한 내용은 Workfront 또는 Frame.io 관리자에게 문의하십시오.

## 기본 테스트 시나리오

알파 프로그램의 새로운 기능을 쉽게 테스트할 수 있도록 새로운 테스트 Frame.io 계정을 만들고 다음과 같은 새 그룹에 연결했습니다. `Frame.io alpha testing` 기존 Workfront 미리보기 또는 샌드박스 환경에서.

기능을 테스트하려면 Workfront 미리보기 또는 샌드박스 인스턴스에 로그인하고 다음 단계를 수행하십시오.

1. **코디네이터:** Workfront 내에서 `Frame.io alpha testing` 프로젝트 그룹으로 할당된 그룹.

1. **코디네이터:** Workfront 내에서 프로젝트 또는 프레임 활성화 작업에 크리에이티브를 할당하고 프로젝트 상태를 &quot;현재&quot;로 변경합니다.

1. **광고:** 새로 만든 Frame.io 프로젝트에 대한 초대를 위해 이메일을 확인하십시오.

1. **광고:** 초대 이메일의 &quot;프로젝트 참여&quot; 버튼을 클릭하여 Frame.io 프로젝트에 참여하고, 프로젝트 내의 Creative Brief를 검토하고, 선택한 Creative Cloud 도구에서 컨텐츠 생성을 시작합니다.

1. **광고:** 만든 에셋을 Frame.io에 업로드하고 연결된 Workfront 프로젝트(또는 할당된 프레임 사용 작업)에 추가합니다.

1. **코디네이터:** Workfront 내에서 연결된 Frame.io 에셋을 찾아 프로젝트에서 검토자/승인자를 할당합니다(검토자/승인자 할당에 대한 자세한 내용은 다음을 참조하십시오.) [문서에 승인자 또는 검토자 추가](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **이해 당사자:** Workfront 내에서 홈 또는 문서 세부 정보에서 승인 요청을 보고 Frame.io 뷰어에서 프레임 연결 문서를 검토한 다음 피드백이 포함된 댓글을 남깁니다.

1. **코디네이터:** Workfront 내에서 Frame.io 연결 문서의 업데이트 섹션 내에서 관련자가 작성한 주석을 확인합니다.

1. **이해 당사자:** Frame.io 뷰어 내에서 결정합니다.

1. **광고:** Frame.io 내에서 자산에 대해 결정된 전반적인 승인 결정을 확인합니다.

1. **광고:** Frame.io 내에서 업데이트된 버전을 연결된 자산의 버전 스택에 추가하여 요청된 변경 사항을 적용합니다.

1. **코디네이터:** Workfront 내에서 승인자/검토자를 새로 업로드한 버전에 할당하고 로그오프에 도달할 때까지 진행 상황을 모니터링합니다.

## 기능 계획

다음은 해결하고자 하는 주요 사용 사례와 현재 계획한 기능에 대한 정보입니다. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">강조 표시된 텍스트</span> 아래는 아직 구현되지 않았지만 이후 릴리스에 포함될 기능을 참조합니다.
>
>아래에 글머리 기호 **&quot;향후 릴리스에서 잠재적인 개선 사항&quot;** 알파 피드백 및 발전하는 개발 계획에 따라 헤더가 향후 릴리스에 포함될 수도 있고 포함되지 않을 수도 있습니다.
>


### Workfront 관리자는 Workfront 그룹과 Frame.io 계정 간의 연결을 설정할 수 있습니다

* <span class="preview">Workfront 내에서는 Workfront 그룹을 Frame.io 계정에 연결할 수 있습니다</span>

* 연결된 Workfront 그룹을 나타내는 Frame.io 내에 새 Frame.io 팀이 만들어집니다

**향후 릴리스에서 잠재적인 개선 사항:**

* Frame.io 계정에서 Workfront 그룹 연결 끊기

* 기존 Frame.io 팀에 Workfront 그룹 연결

### 프로젝트 코디네이터는 Frame.io로 전송되는 Workfront 프로젝트를 구성하고, 할당된 Workfront 크리에이티브를 Frame.io의 프로젝트에 추가하도록 할 수 있습니다.

* Frame 연결 그룹을 할당하여 활성화된 Frame.io로 Workfront 프로젝트를 표시하는 기능

* <span class="preview">개선 사항: Workfront 프로젝트 내의 작업을 프레임 작업으로 전환하여 Frame.io 내에 작업 폴더를 만드는 기능</span>

* Workfront 프로젝트 상태를 현재로 설정하면 연결된 프로젝트가 프레임에 만들어지고 Workfront에서 할당한 사용자가 프레임 프로젝트에 추가되고 Frame.io에서 이메일 알림이 전송됩니다

   * 모든 Workfront 프로젝트 멤버(사용자 및 팀)는 프로젝트 생성 시 Frame.io 프로젝트에 공동 작업자로 추가됩니다.

   * <span class="preview">변경: 프레임 사용 Workfront 작업에 할당된 사용자 및 팀은 Frame.io 프로젝트에 공동 작업자로 추가되고 알림을 받습니다(프로젝트 생성 및 이후 시)</span>

* 프로젝트 및 프레임 사용 작업에 추가된 문서(Creative Brief)는 프로젝트가 만들어지면(트리거: 프로젝트 상태를 현재로 설정) Frame.io 프로젝트(각 작업 폴더 내)로 푸시됩니다.

   * Frame.io로 불필요한 여러 문서를 보내지 않도록 Creative Brief만 활성화하기 전에 프로젝트에 추가되는 문서의 양을 제한하는 것이 좋습니다

* <span class="preview">개선 사항: 프레임 사용 Workfront 작업에서 명시적으로 할당 해제된 사용자/팀은 Frame.io 프로젝트에서 제거됩니다</span>

**향후 릴리스에서 잠재적인 개선 사항:**

* 프레임 사용 작업은 프로젝트 템플릿에서 구성할 수 있습니다.

* Creative Brief에 대한 새 버전 업로드가 프레임으로 푸시됨

* 최적화된 프로젝트 동기화 (프로젝트 연결 해제, 프로젝트 및 문서 재동기화 등)

### Frame.io 내에서 크리에이티브는 공식 검토를 위해 생성된 에셋을 Workfront 프로젝트에 보낼 수 있습니다

* 단일 Frame.io 자산을 WF 프로젝트 또는 작업에 연결하는 기능입니다. Workfront 내에 에셋 참조가 만들어집니다.

* Frame.io 내의 새 버전 업로드는 연결된 자산에서 Workfront 내의 새 문서 버전을 자동으로 만듭니다.

* <span class="preview">개선 사항: 참조된 Workfront 작업을 Frame.io 내에서 완료된 것으로 표시하는 기능</span>

* <span class="preview">개선 사항: 연결된 Workfront 문서가 삭제되면 Frame.io 내에 유지되며 동일한 프로젝트 작업 또는 다른 프로젝트 작업에 다시 연결할 수 있습니다</span>

**향후 릴리스에서 잠재적인 개선 사항:**

* 여러 Frame.io 자산을 한 번에 Workfront에 보낼 수 있는 기능

* Frame.io 내에서 Workfront 프로젝트/작업에 대한 시간 로깅

### 프로젝트 코디네이터는 Frame.io에서 링크된 문서에 공식 승인 프로세스를 할당할 수 있습니다.

* Workfront 사용자 및 팀을 Frame.io 연결 문서에 대한 새 문서 승인에 추가할 수 있습니다.

* <span class="preview">개선 사항: 사용자/팀이 프레임 활성화 문서에서 공유되지 않으면 Frame.io 뷰어의 자산에 대한 액세스 권한도 상실됩니다.</span>

**향후 릴리스에서 잠재적인 개선 사항:**

* 여러 에셋을 단일 검토로 전송

* Workfront 문서에 승인자/검토자 일괄 할당

### 이해 당사자는 Frame.io Viewer 내에서 검토 및 승인을 수행할 수 있습니다.

* 이해 당사자에게 알림이 전송되며 Frame.io 뷰어 내에서 Frame 연결된 문서를 볼 수 있습니다.

* Frame.io 뷰어는 Workfront 내의 다른 위치(예: 문서 목록, 문서 세부 정보, Workfront 홈)에서 액세스할 수 있습니다

* Workfront의 업데이트 스트림과 동기화되는 Frame.io 뷰어에서 제공하는 기존 검토 및 주석 달기 기능을 활용하는 기능

* <span class="preview">Frame.io 뷰어 내에서 새 문서 승인 결정을 내리는 기능</span>

### Frame.io 내에서 크리에이티브에게 연결된 Frame.io 자산에 대해 결정된 전반적인 사항에 대해 알려줍니다

* <span class="preview">개선 사항: 전체 문서 승인 상태가 Frame.io 내의 자산에 표시됩니다.</span>

### 프로젝트 코디네이터는 최종 에셋을 AEM에 보낼 수 있습니다.

* <span class="preview">개선 사항: 기존 Workfront + AEM Asset CS 커넥터를 사용하여 메타데이터를 비롯한 프레임에 연결된 문서를 AEM으로 보낼 수 있습니다.</span>
