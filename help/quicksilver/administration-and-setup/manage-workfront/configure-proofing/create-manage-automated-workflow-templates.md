---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 자동화된 워크플로우 템플릿 만들기 및 관리
description: Adobe Workfront 관리자는 조직의 컨텐츠 검토 프로세스가 자주 반복되거나 동일한 사람이 컨텐츠를 자주 검토하는 경우, 지정하는 증명 역할과 알림 설정을 가진 검토자가 포함된 자동화된 워크플로우 템플릿을 생성할 수 있습니다. 자동화된 워크플로우 템플릿은 한 명 또는 두 명의 검토자만 사용하여 간단하거나 여러 단계 및 종속성이 있는 복잡할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# 자동화된 워크플로우 템플릿 만들기 및 관리

Adobe Workfront 관리자는 조직의 컨텐츠 검토 프로세스가 자주 반복되거나 동일한 사람이 컨텐츠를 자주 검토하는 경우, 지정하는 증명 역할과 알림 설정을 가진 검토자가 포함된 자동화된 워크플로우 템플릿을 생성할 수 있습니다. 자동화된 워크플로우 템플릿은 한 명 또는 두 명의 검토자만 사용하여 간단하거나 여러 단계 및 종속성이 있는 복잡할 수 있습니다.

자동화된 워크플로우 템플릿을 사용하면 자동화된 워크플로우를 통해 증명을 쉽게 만들 수 있습니다. 사용자가 증명을 만들 때 필요한 템플릿을 선택하기만 하면 됩니다.

언제든지 자동 워크플로우 템플릿을 변경하거나 검토자와 단계를 추가하거나 제거할 수 있습니다. 또한 템플릿을 사용하는 증명 작성자는 증명에 대한 검토자를 추가하거나 제거할 수 있습니다.

자동화된 워크플로우 템플릿을 사용할 때는 다음 사항을 고려하십시오.

1. 자동화된 워크플로우 템플릿의 설정은 증명을 위해 자동화된 워크플로우를 사용하여 수행할 수 있는 작업을 결정합니다. 예를 들어 템플릿에서 스테이지 추가 단추가 비활성화된 경우 증명의 자동화된 워크플로우 설정을 사용하여 작업할 때에는 표시되지 않습니다.
1. 사용자가 자동화된 워크플로우 템플릿의 용지에 추가되지만, 증명에 검토자로 이미 있으면 템플릿을 적용하면 검토자가 스테이지에서 제거됩니다. 스테이지에 다른 검토자를 추가하지 않으면 메시지를 통해 검토자를 추가하라는 메시지가 표시됩니다.
1. 자동화된 워크플로우 템플릿을 수정하는 기능은 에 설명된 대로 Workfront 관리자가 구성한 템플릿 설정에 따라 다릅니다. 템플릿을 수정하는 기능이 비활성화되어 있으면 템플릿 소유자만 수정할 수 있습니다.

자동화된 워크플로우에 대한 자세한 내용은 [자동화된 워크플로우 개요](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Premium 또는 선택</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>증명 권한 프로필에서 관리자를 선택해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">사용자의 언어 교정 액세스 구성</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 자동화된 워크플로우 템플릿 만들기

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스
1. 클릭 **워크플로우** 왼쪽 패널에 표시됩니다.
1. 설정 **워크플로우** 탭, **새로 만들기** > **새 템플릿**.

1. 에서 **세부 사항** 섹션에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 이름</td> 
      <td>(필수) 템플릿의 이름을 입력합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 소유자</td> 
      <td>템플릿을 관리할 Workfront 관리자 또는 Workfront 증명 관리자를 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 그룹</td> 
      <td> <p> 조직의 자동화된 워크플로우가 그룹으로 구성되어 있는 경우 그룹 이름을 선택할 수 있습니다. 자세한 내용은 <a href="#create-automated-workflow-template-groups" class="MCXref xref">자동화된 워크플로우 템플릿 그룹 만들기</a> 자세한 내용은 이 문서의 뒷부분에 나와 있습니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">템플릿 시간대 </td> 
      <td> <p>템플릿의 기본 시간대는 작업 중인 시간대입니다. 템플릿을 사용할 증명 작성자 및 검토자의 시간대가 다른 경우 여기에서 변경하여 해당 사용자에 대해 적절한 시간에 스테이지 마감일이 설정되도록 할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">허용</td> 
      <td> <p>템플릿으로 증명을 만들 때 사용할 스테이지 활동을 선택할 수 있습니다.</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 에서 **단계** 섹션에서 자동화된 워크플로우 템플릿의 각 단계를 구성합니다.

   여러 단계를 추가하고 이 단계 간에 만들 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>스테이지 이름은 Workflow 섹션 맨 위의 Automated Workflow 다이어그램, 증명 세부 정보 페이지 및 검토자에게 전송된 전자 메일 알림에 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 활성화</td> 
      <td> <p>스테이지를 자동으로 활성화할지 또는 수동으로 활성화할지 지정합니다. 첫 번째 단계에 대해 <strong>증명 작성 시</strong>, <strong>특정 날짜 및 시간에</strong>, 또는 <strong>수동으로</strong>.</p> <p>다른 옵션은 상위 스테이지를 선택해야 하므로 두 번째 스테이지를 추가할 때 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음 기간에서 계산된 기한</td> 
      <td> <p>기한을 계산하는 방법을 지정합니다.</p> 
       <ul> 
        <li> <p><strong>증명 만들기</strong>: 아래의 드롭다운 목록에서 <strong>기한(업무일 이상)</strong>를 선택합니다. 증명 생성 날짜에 추가할 영업일 수를 선택하여 증명의 마감일을 자동으로 설정합니다.</p> </li> 
        <li><strong>스테이지가 시작될 때</strong>: 아래의 드롭다운 목록에서 <strong>기한(업무일 이상)</strong>를 클릭하고, 단계 활성화 날짜에 추가할 비즈니스 일수를 선택하여 증명의 최종 기한을 자동으로 설정합니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">스테이지 잠금</td> 
      <td>설명을 위해 스테이지를 잠글 수 있도록 허용할지 여부를 지정합니다. 다음 단계가 시작될 때 또는 상위 단계에서 모든 결정을 내릴 때 수동으로 또는 자동으로 스테이지를 잠그는 옵션이 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">주요 의사 결정자</td> 
      <td> <p>사용 가능한 의사 결정자는 스테이지에 검토자를 추가한 후에만 목록에 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 결정은 단 하나입니다.</td> 
      <td>단계 검토 프로세스는 의사 결정권자 중 한 명이 결정을 내리자마자 완료될 것입니다. 자세한 내용은 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront 증명의 증명 설정 구성</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">비공개 단계</td> 
      <td>스테이지에 추가되지 않거나 Workfront 관리자가 아닌 사용자로부터 댓글 및 결정을 숨깁니다&lt;!&gt;— FLARE에서 초안 작성: 감독자 및 이상

       -->. 자세한 내용은 &lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>자동화된 워크플로우 개요 를 참조하십시오&lt;/a>.&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">이 단계를 삭제할 수 없습니다.</td> 
      <td> <p>스테이지를 필수 항목으로 설정합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 이 템플릿을 사용할 증명이 항상 스테이지에서 동일한 사람에게 전송되는 경우 사용자가 증명을 만들 때마다 증명을 추가할 필요가 없도록 여기에 추가합니다.

   각 사용자 선택 **역할** 이 템플릿과 을 사용할 증명 **이메일 경고** 이 템플릿을 사용하는 증명을 작업할 때 사용자가 받게 합니다.

   증명의 역할에 대한 자세한 내용은 [기본 언어 교정 역할 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). 증명 이메일 경고에 대한 자세한 내용은 섹션을 참조하십시오 [사용자에 대한 증명 기본값 구성](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) 기사  [Workfront 증명의 이메일 알림 설정 구성](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   각 사용자는 한 단계에만 추가할 수 있습니다. 스테이지에 원하는 만큼 사용자를 추가할 수 있습니다.

   >[!TIP]
   >
   >단계 다이어그램의 단계 간에 검토자 이름을 끌어다 놓을 수 있습니다. 사용 가능한 단계는 파란색으로 강조 표시됩니다.

1. 템플릿에 추가하려는 다른 단계에 대해 이전 두 단계를 반복합니다.

   맨 위에 **워크플로우** 섹션에서 설정하는 자동화된 워크플로우의 다이어그램을 볼 수 있습니다. 단계를 계속 추가할 때 다이어그램에 단계 간 종속성이 표시된 줄이 나타납니다. 다이어그램에서 스테이지를 클릭하여 해당 스테이지의 설정을 볼 수 있습니다.

   다이어그램을 볼 필요가 없는 경우 **다이어그램 숨기기**.

1. 에서 **서식 파일 공유** 섹션에서 옵션을 클릭하여(템플릿이 전체 조직과 아직 공유되지 않은 경우) 템플릿을 사용할 수 있는 사용자를 지정합니다.

   기본적으로 새로운 자동화된 워크플로우 템플릿은 조직의 모든 사람과 공유됩니다.

1. Click **Create**.

## 자동화된 워크플로우 템플릿 수정

Workfront 증명 관리자는 자동화된 워크플로우 템플릿을 수정할 수 있습니다. 변경 사항은 자동으로 저장됩니다.

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스
1. 클릭 **워크플로우** 왼쪽 패널에 표시됩니다.
1. 에서 **워크플로우 템플릿** 목록이 표시되면 수정할 템플릿을 클릭합니다.
1. 에서 **세부 사항** 섹션에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 이름</td> 
      <td>(필수) 템플릿의 이름을 입력합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 소유자</td> 
      <td>템플릿을 관리할 Workfront 관리자 또는 Workfront 증명 관리자를 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 그룹</td> 
      <td> <p> 조직의 자동화된 워크플로우가 그룹으로 구성되어 있는 경우 그룹 이름을 선택할 수 있습니다. 자세한 내용은 <a href="#create-automated-workflow-template-groups" class="MCXref xref">자동화된 워크플로우 템플릿 그룹 만들기</a> 자세한 내용은 이 문서의 뒷부분에 나와 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 시간대 </td> 
      <td> <p>템플릿의 기본 시간대는 작업 중인 시간대입니다. 템플릿을 사용할 증명 작성자 및 검토자의 시간대가 다른 경우 여기에서 변경하여 해당 사용자에 대해 적절한 시간에 스테이지 마감일이 설정되도록 할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">허용</td> 
      <td> <p>템플릿을 사용하여 증명을 만드는 사람이 사용할 수 있도록 할 단계 활동을 선택합니다. </p> <p><b>경고</b>: 단계 추가 및 단계에 사람 추가 옵션을 선택하지 않으면 이 템플릿을 사용하는 증명 소유자 또는 템플릿 소유자가 스테이지를 추가하거나 증명을 공유할 수 없습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 에서 **워크플로우** 섹션에서 스테이지의 이름을 변경하고 설정을 확장합니다. ![](assets/arrow-button.png) 필요한 변경 작업을 수행하려면 다음을 수행하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">다음 기간에서 계산된 기한</td> 
      <td> <p>기한을 계산하는 방법을 지정합니다.</p> 
       <ul> 
        <li> <p><strong>증명 생성에서 계산된 기한</strong>: 에서 <strong>단계 최종 기한 설정</strong> 드롭다운 목록에서 증명 생성 날짜에 추가할 업무 일수를 선택하여 증명의 마감일을 자동으로 설정합니다.</p> </li> 
        <li><strong>단계 활성화에서 계산된 기한</strong>: 에서 <strong>단계 최종 기한 설정</strong> 드롭다운 목록에서 단계 활성화 날짜에 추가할 비즈니스 일수를 선택하여 증명의 최종 기한을 자동으로 설정합니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 활성화</td> 
      <td> <p>스테이지를 자동으로 활성화할지 또는 수동으로 활성화할지 지정합니다. 첫 번째 단계에 대해 <strong>증명 작성 시</strong>, <strong>특정 날짜 및 시간에</strong>, 또는 <strong>수동으로</strong>.</p> <p>다른 옵션은 상위 스테이지를 선택해야 하므로 두 번째 스테이지를 추가할 때 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">스테이지 잠금</td> 
      <td>설명을 위해 스테이지를 잠글 수 있도록 허용할지 여부를 지정합니다. 다음 단계가 시작될 때 또는 상위 단계에서 모든 결정을 내릴 때 수동으로 또는 자동으로 스테이지를 잠그는 옵션이 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정</td> 
      <td>의사 결정자 중 한 명이 그들의 결정을 제출한 첫 번째 단계를 끝냅니다. 자세한 내용은 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront 증명의 증명 설정 구성</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">개인 정보 보호</td> 
      <td>스테이지에 추가되지 않거나 계정 관리자가 아닌 사용자로부터 의견 및 결정을 숨깁니다. 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">자동화된 워크플로우 개요</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 삭제</td> 
      <td>스테이지를 필수 항목으로 설정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기타 <img src="assets/more-icon.png"></td> 
      <td>스테이지에 검토자를 추가하거나 스테이지를 삭제합니다.<p>특정 단계에서 각 증명을 동일한 사람에게 보낼 경우 증명을 만들 때마다 증명을 추가할 필요가 없도록 여기에 증명 이름을 지정할 수 있습니다. 스테이지에 추가할 사용자 이름을 입력하고 선택한 다음 추가합니다 <strong>역할</strong> 증명서에 <strong>이메일 경고</strong> 사용자에 대한 설정입니다. 언어 교정 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">기본 언어 교정 역할 구성</a>. 증명 이메일 경고에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">사용자에 대한 증명 기본값 구성</a> 기사 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Workfront 증명의 이메일 알림 설정 구성</a>.</p><p>스테이지에 원하는 만큼 사용자를 추가할 수 있습니다</p><p>팁: 단계 다이어그램의 단계 간에 검토자 이름을 끌어다 놓을 수 있습니다. 사용 가능한 단계는 파란색으로 강조 표시됩니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 템플릿에 추가할 다른 단계에 대해 단계를 반복합니다.

   맨 위에 **워크플로우** 섹션에서 설정하는 자동화된 워크플로우의 다이어그램을 볼 수 있습니다. 단계를 계속 추가할 때 다이어그램에 단계 간 종속성이 표시된 줄이 나타납니다. 다이어그램에서 스테이지를 클릭하여 해당 스테이지의 설정을 볼 수 있습니다.

   다이어그램을 볼 필요가 없는 경우 **다이어그램 숨기기**.

1. 에서 **공유 대상** 섹션에서 사용자를 삭제하려면 ![](assets/more-icon.png) 오른쪽에 있는 버튼을 클릭한 다음 **제거**.

## 자동화된 워크플로우 템플릿 그룹 만들기 {#create-automated-workflow-template-groups}

Workfront 관리자는 조직 계정의 모든 자동화된 워크플로우 템플릿을 보고 관리할 수 있습니다. 템플릿을 그룹으로 구성하는 것이 도움이 될 수 있습니다.

자동화된 워크플로우 템플릿 그룹을 생성하려면 다음을 수행합니다.

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스
1. 클릭 **워크플로우** 왼쪽 패널에 표시됩니다.
1. 설정 **워크플로우** 탭, **새로 만들기** > **새 템플릿 그룹**.
1. 새 템플릿 그룹을 설명하는 이름을 입력한 다음 키를 누릅니다 **Enter 키**.

끌어서 놓아 그룹 간에 템플릿을 이동할 수 있습니다.

## 자동화된 워크플로우 템플릿 관리

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스

1. Workfront 증명의 왼쪽 패널에서 **워크플로우**.
1. 설정 **워크플로우** 표시되는 페이지에서 다음 중 하나를 수행합니다.

   * 새 템플릿 추가
   * 새 템플릿 그룹 추가
   * 템플릿 그룹을 하나 이상 삭제
   * 템플릿 세부 정보 액세스
   * 템플릿을 다른 템플릿 그룹으로 드래그합니다.
