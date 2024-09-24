---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 자동화된 워크플로 템플릿 만들기 및 관리
description: Adobe Workfront 관리자는 조직의 콘텐츠 검토 프로세스가 자주 반복되거나 동일한 사람이 콘텐츠를 검토하는 경우, 사용자가 지정하는 증명 역할 및 알림 설정을 통해 이러한 검토자가 포함된 자동화된 워크플로 템플릿을 만들 수 있습니다. 자동화된 워크플로 템플릿은 한 두 명의 검토자만으로 단순하거나 많은 단계와 종속성이 있는 복잡한 작업이 될 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 7a2cfddf4683b5b49121bbe3987498297b963ffa
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# 자동화된 워크플로 템플릿 만들기 및 관리

<!-- Audited: 2/2024 -->

Adobe Workfront 관리자는 조직의 콘텐츠 검토 프로세스가 자주 반복되거나 동일한 사람이 콘텐츠를 검토하는 경우, 사용자가 지정하는 증명 역할 및 알림 설정을 통해 이러한 검토자가 포함된 자동화된 워크플로 템플릿을 만들 수 있습니다. 자동화된 워크플로 템플릿은 한 두 명의 검토자만으로 단순하거나 많은 단계와 종속성이 있는 복잡한 작업이 될 수 있습니다.

자동화된 워크플로 템플릿을 사용하면 자동화된 워크플로로 증명을 쉽게 만들 수 있습니다. 사용자가 증명을 만들 때 필요한 템플릿을 선택하면 됩니다.

언제든지 검토자와 단계를 추가하거나 제거하여 모든 자동화된 워크플로 템플릿을 쉽게 변경할 수 있습니다. 템플릿을 사용하는 증명 작성자는 증명에 대한 검토자를 추가하거나 제거할 수 있습니다.

자동화된 워크플로우 템플릿을 사용할 때는 다음 사항을 고려하십시오.

1. 자동화된 워크플로 템플릿의 설정은 증명에 대한 자동화된 워크플로로 수행할 수 있는 작업을 결정합니다. 예를 들어, 템플릿에서 단계 추가 버튼이 비활성화되어 있는 경우 증명에 대한 자동화된 워크플로 설정으로 작업할 때 이 버튼이 표시되지 않습니다.
1. 자동화된 워크플로 템플릿의 단계에 추가되었지만 증명에 이미 검토자로 존재하는 경우 템플릿을 적용하면 검토자가 단계에서 제거됩니다. 스테이지에 다른 검토자를 추가하지 않으면 하나를 추가하라는 메시지가 표시됩니다.
1. 자동화된 워크플로 템플릿을 수정하는 기능은 의 설명과 같이 Workfront 관리자가 구성한 템플릿 설정에 따라 다릅니다. 템플릿 수정 기능이 비활성화된 경우 템플릿 소유자만 수정할 수 있습니다.

자동화된 워크플로에 대한 자세한 내용은 [자동화된 워크플로 개요](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>새로 만들기: 모두</p><p>현재: Pro 이상</p><p>레거시: Premium 또는 Select</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 표준</p><p>현재: 작업 또는 계획</p> <p>레거시: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>증명 권한 프로필에서 관리자를 선택해야 합니다. </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 자동화된 워크플로우 템플릿 만들기

{{step1-to-proofing}}

1. 왼쪽 패널에서 **워크플로**&#x200B;를 클릭합니다.
1. **워크플로** 탭에서 **새로 만들기** > **새 템플릿**&#x200B;을 클릭합니다.

1. **세부 정보** 섹션에서 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 이름</td> 
      <td>(필수) 템플릿 이름을 입력합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 소유자</td> 
      <td>템플릿을 관리할 Workfront 관리자 또는 Workfront Proof 관리자를 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 그룹</td> 
      <td> <p> 조직의 자동화된 워크플로가 그룹으로 구성된 경우 그룹의 이름을 선택할 수 있습니다. 자세한 내용은 이 문서의 뒷부분에서 <a href="#create-automated-workflow-template-groups" class="MCXref xref">자동화된 워크플로 템플릿 그룹 만들기</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">템플릿 시간대 </td> 
      <td> <p>템플릿의 기본 시간대는 작업 중인 시간대입니다. 템플릿을 사용할 증명 작성자 및 검토자의 시간대가 다른 경우 여기서 시간대를 변경하여 해당 사용자에 대해 적절한 시간에 스테이지 기한을 설정할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">허용</td> 
      <td> <p>템플릿을 사용하여 증명을 만들 수 있도록 단계 활동을 선택할 수 있습니다.</p> 
      <p><b>경고</b>: 단계 추가 및 단계에 사람 추가 옵션을 선택하지 않으면 템플릿 소유자나 이 템플릿을 사용하는 모든 증명 소유자가 단계를 추가하거나 증명을 공유할 수 없습니다. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. **단계** 섹션에서 자동화된 워크플로 템플릿의 각 단계를 구성합니다.

   여러 단계를 추가하고 두 단계 사이에 을 만들 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>단계 이름은 워크플로 섹션의 맨 위에 있는 자동화된 워크플로 다이어그램, 증명 세부 정보 페이지 및 검토자에게 전송된 이메일 알림에 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 활성화</td> 
      <td> <p>스테이지를 자동으로 활성화할지 수동으로 활성화할지 지정합니다. 첫 번째 단계에서는 <strong>증명 생성 시</strong>, <strong>특정 날짜 및 시간에</strong> 또는 <strong>수동으로</strong>를 선택할 수 있습니다.</p> <p>다른 옵션은 상위 단계를 선택해야 하므로 두 번째 단계를 추가할 때 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음에서 계산된 기한:</td> 
      <td> <p>기한을 계산할 방법을 지정합니다.</p> 
       <ul> 
        <li> <p><strong>증명 만들기</strong>: <strong>기한(+ 영업일)</strong> 아래의 드롭다운 목록에서 증명 만들기 날짜에 추가할 영업일 수를 선택하여 증명에 대한 기한을 자동으로 설정합니다.</p> </li> 
        <li><strong>단계가 시작될 때</strong>: <strong>기한(+ 영업일)</strong> 아래의 드롭다운 목록에서 단계 활성화 날짜에 추가할 영업일 수를 선택하여 증명에 대한 기한을 자동으로 설정합니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">스테이지 잠금</td> 
      <td>스테이지를 댓글에 대해 잠글 수 있도록 할지 여부를 지정합니다. 다음 단계가 시작될 때 또는 상위 단계에서 모든 결정이 내려질 때 단계를 수동으로 또는 자동으로 잠그는 옵션이 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">주요 의사 결정자</td> 
      <td> <p>단계에 검토자를 추가한 후에만 사용 가능한 의사 결정자가 목록에 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 결정은 단 하나입니다.</td> 
      <td>의사 결정자 중 한 명이 의사 결정을 제출하면 단계에 대한 검토 절차가 완료된다. 자세한 내용은 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof에서 증명 설정 구성</a>을 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">비공개 단계</td> 
      <td>단계에 추가되지 않았거나 Workfront 관리자가 아닌 사용자에게에서 주석 및 결정을 숨깁니다. 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">자동화된 워크플로 개요</a>를 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 단계 삭제 허용 안 함</td> 
      <td> <p>스테이지를 필수 항목으로 만듭니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 이 템플릿을 사용할 증명이 항상 스테이지의 동일한 사람에게 전송되는 경우 사용자가 증명을 만들 때마다 추가할 필요가 없도록 여기에 추가하십시오.

   이 템플릿을 사용할 증명에 대한 각 사용자의 **역할**&#x200B;과(와) 이 템플릿을 사용하는 증명에 대한 작업을 수행할 때 사용자가 받게 될 **전자 메일 경고**&#x200B;를 선택하십시오.

   증명에 대한 역할에 대한 자세한 내용은 [기본 증명 역할 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)을 참조하십시오. 증명 전자 메일 경고에 대한 자세한 내용은 문서 [Workfront Proof에서 전자 메일 알림 설정 구성](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)의 [사용자에 대한 증명 기본값 구성](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) 섹션을 참조하십시오.

   각 사용자를 한 단계에만 추가할 수 있습니다. 단계에 원하는 만큼 사용자를 추가할 수 있습니다.

   >[!TIP]
   >
   >단계 다이어그램의 단계 간에 검토자 이름을 끌어서 놓을 수 있습니다. 사용 가능한 단계는 파란색으로 강조 표시됩니다.

1. 템플릿에 추가하려는 다른 단계에 대해 앞의 두 단계를 반복합니다.

   **워크플로** 섹션의 맨 위에 설정 중인 자동화된 워크플로의 다이어그램을 볼 수 있습니다. 단계를 계속 추가하면 이들 단계가 다이어그램에 표시되고 두 단계 사이의 종속성이 표시된 줄이 표시됩니다. 다이어그램에서 단계를 클릭하여 해당 단계에 대한 설정을 볼 수 있습니다.

   다이어그램을 볼 필요가 없으면 **다이어그램 숨기기**&#x200B;를 클릭할 수 있습니다.

1. **템플릿 공유** 섹션에서 옵션을 클릭하여(템플릿을 아직 조직 전체와 공유하지 않은 경우) 사용할 수 있는 사용자를 지정합니다.

   기본적으로 새로운 자동화된 워크플로 템플릿은 조직의 모든 사용자와 공유됩니다.

1. Click **Create**.

## 자동화된 워크플로우 템플릿 수정

Workfront Proof 관리자는 자동화된 워크플로 템플릿을 수정할 수 있습니다. 변경 사항을 만들면 자동으로 저장됩니다.

{{step1-to-proofing}}

1. 왼쪽 패널에서 **워크플로**&#x200B;를 클릭합니다.
1. 표시되는 **워크플로 템플릿** 목록에서 수정할 템플릿을 클릭합니다.
1. **세부 정보** 섹션에서 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 이름</td> 
      <td>(필수) 템플릿 이름을 입력합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 소유자</td> 
      <td>템플릿을 관리할 Workfront 관리자 또는 Workfront Proof 관리자를 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 그룹</td> 
      <td> <p> 조직의 자동화된 워크플로가 그룹으로 구성된 경우 그룹의 이름을 선택할 수 있습니다. 자세한 내용은 이 문서의 뒷부분에서 <a href="#create-automated-workflow-template-groups" class="MCXref xref">자동화된 워크플로 템플릿 그룹 만들기</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 시간대 </td> 
      <td> <p>템플릿의 기본 시간대는 작업 중인 시간대입니다. 템플릿을 사용할 증명 작성자 및 검토자의 시간대가 다른 경우 여기서 시간대를 변경하여 해당 사용자에 대해 적절한 시간에 스테이지 기한을 설정할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">허용</td> 
      <td> <p>템플릿을 사용하여 증명을 만드는 사람이 사용할 수 있도록 하려는 단계 활동을 선택합니다. </p> <p><b>경고</b>: 단계 추가 및 단계에 사람 추가 옵션을 선택하지 않으면 템플릿 소유자나 이 템플릿을 사용하는 모든 증명 소유자가 단계를 추가하거나 증명을 공유할 수 없습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **워크플로** 섹션에서 단계 이름을 변경하고 설정 ![](assets/arrow-button.png)을(를) 확장하여 필요한 대로 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">다음에서 계산된 기한:</td> 
      <td> <p>기한을 계산할 방법을 지정합니다.</p> 
       <ul> 
        <li> <p><strong>증명 만들기에서 계산된 기한</strong>: <strong>단계 기한 설정</strong> 드롭다운 목록에서 증명 만들기 날짜에 추가할 영업일 수를 선택하여 증명에 대한 기한을 자동으로 설정합니다.</p> </li> 
        <li><strong>단계 활성화에서 계산된 기한</strong>: <strong>단계 기한 설정</strong> 드롭다운 목록에서 단계 활성화 날짜에 추가할 영업일 수를 선택하여 증명에 대한 기한을 자동으로 설정합니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 활성화</td> 
      <td> <p>스테이지를 자동으로 활성화할지 수동으로 활성화할지 지정합니다. 첫 번째 단계에서는 <strong>증명 생성 시</strong>, <strong>특정 날짜 및 시간에</strong> 또는 <strong>수동으로</strong>를 선택할 수 있습니다.</p> <p>다른 옵션은 상위 단계를 선택해야 하므로 두 번째 단계를 추가할 때 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">스테이지 잠금</td> 
      <td>스테이지를 댓글에 대해 잠글 수 있도록 할지 여부를 지정합니다. 다음 단계가 시작될 때 또는 상위 단계에서 모든 결정이 내려질 때 단계를 수동으로 또는 자동으로 잠그는 옵션이 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정</td> 
      <td>의사 결정자 중 한 명이 의사 결정을 처음 제출할 때 단계를 종료합니다. 자세한 내용은 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof에서 증명 설정 구성</a>을 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">개인 정보 보호</td> 
      <td>단계에 추가되지 않은 사람 또는 계정에서 감독자가 아닌 사람과 그 위에 있는 사람에 대한 주석 및 결정을 숨깁니다. 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">자동화된 워크플로 개요</a>를 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">스테이지 삭제</td> 
      <td>스테이지를 필수 항목으로 만듭니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기타 <img src="assets/more-icon.png"></td> 
      <td>스테이지에 검토자를 추가하거나 스테이지를 삭제합니다.<p>각 증명이 특정 단계에 있는 동일한 사람들에게 전송되는 경우, 증명을 만들 때마다 추가할 필요가 없도록 여기에 해당 이름을 지정할 수 있습니다. 단계에 추가할 사용자의 이름을 입력하고 선택한 다음 증명에 <strong>역할</strong> 및 사용자에 대해 원하는 <strong>전자 메일 경고</strong> 설정을 추가하십시오. 증명 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">기본 증명 역할 구성</a>을 참조하십시오. 증명 전자 메일 경고에 대한 자세한 내용은 문서 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Workfront Proof에서 전자 메일 알림 설정 구성</a>의 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">사용자에 대한 증명 기본값 구성</a> 섹션을 참조하십시오.</p><p>단계에 원하는 만큼 사용자를 추가할 수 있습니다</p><p>팁: 단계 다이어그램의 단계 간에 검토자 이름을 끌어서 놓을 수 있습니다. 사용 가능한 단계는 파란색으로 강조 표시됩니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 템플릿에 추가하려는 다른 단계에 대해 단계를 반복합니다.

   **워크플로** 섹션의 맨 위에 설정 중인 자동화된 워크플로의 다이어그램을 볼 수 있습니다. 단계를 계속 추가하면 이들 단계가 다이어그램에 표시되고 두 단계 사이의 종속성이 표시된 줄이 표시됩니다. 다이어그램에서 단계를 클릭하여 해당 단계에 대한 설정을 볼 수 있습니다.

   다이어그램을 볼 필요가 없으면 **다이어그램 숨기기**&#x200B;를 클릭할 수 있습니다.

1. **다음 사용자와 공유** 섹션에서 사용자를 삭제하려면 오른쪽에 있는 기타 ![](assets/more-icon.png) 단추를 클릭한 다음 **제거**&#x200B;를 클릭합니다.

## 자동화된 워크플로우 템플릿 그룹 만들기 {#create-automated-workflow-template-groups}

Workfront 관리자는 조직 계정의 모든 자동화된 워크플로 템플릿을 보고 관리할 수 있습니다. 템플릿을 그룹으로 구성하는 것이 도움이 될 수 있습니다.

자동화된 워크플로우 템플릿 그룹을 생성하려면 다음을 수행합니다.

{{step1-to-proofing}}

1. 왼쪽 패널에서 **워크플로**&#x200B;를 클릭합니다.
1. **워크플로** 탭에서 **새로 만들기** > **새 템플릿 그룹**&#x200B;을 클릭합니다.
1. 새 템플릿 그룹의 수사적 이름을 입력한 다음 **Enter**&#x200B;를 누릅니다.

끌어다 놓아 그룹 간에 템플릿을 이동할 수 있습니다.

## 자동화된 워크플로 템플릿 관리

{{step1-to-proofing}}

1. Workfront Proof의 왼쪽 패널에서 **워크플로**&#x200B;를 클릭합니다.
1. 표시되는 **워크플로** 페이지에서 다음 중 하나를 수행합니다.

   * 새 템플릿 추가
   * 새 템플릿 그룹 추가
   * 하나 이상의 템플릿 그룹 삭제
   * 템플릿 세부 정보 액세스
   * 템플릿을 다른 템플릿 그룹으로 드래그
