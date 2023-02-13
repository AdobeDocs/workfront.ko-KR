---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Adobe Workfront에서 보고서 공유
description: Adobe Workfront 관리자는 사용자에게 액세스 수준을 할당할 때 보고서를 보거나 편집할 수 있는 액세스 권한을 부여합니다. 문제에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 보고서, 대시보드 및 달력에 대한 액세스 권한 부여 를 참조하십시오.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Adobe Workfront에서 보고서 공유

Adobe Workfront 관리자는 사용자에게 액세스 수준을 할당할 때 보고서를 보거나 편집할 수 있는 액세스 권한을 부여합니다. 문제에 대한 액세스 권한 부여에 대한 자세한 내용은 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

사용자에게 부여된 액세스 수준과 함께 사용자에게 공유 액세스 권한이 있는 특정 보고서를 보거나 관리할 권한을 부여할 수도 있습니다. 액세스 수준 및 권한에 대한 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방법](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아니더라도 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

## 액세스 요구 사항

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 또는 그 이상의 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서 보기 권한 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 보고서 공유에 대한 고려 사항

아래 고려 사항 외에 다음을 참조하십시오 [보고서, 대시보드 및 달력 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* 만든 보고서를 다른 개인, 팀, 그룹, Job 역할 또는 회사와 공유할 수 있습니다. 다른 사용자가 만들고 사용자와 공유한 보고서를 공유할 수도 있습니다.
* 전체 조직과 공유하거나 공개할 수도 있습니다. 보고서를 공개하면 다른 사용자와 공유할 수 있는 URL이 생성됩니다.
* 개별 보고서를 공유하거나 보고서 목록에서 여러 보고서를 공유할 수 있습니다.

## 보고서를 공유하는 방법

다음과 같은 방법으로 Workfront에서 보고서를 공유할 수 있습니다.

* 에 설명된 대로 수동으로 [보고서 공유](#share-a-report) 섹션을 참조하십시오.
* 공유된 보고서가 포함된 대시보드에서 보기 권한을 상속하여 자동으로 사용됩니다. 객체에 대한 상속된 권한 보기에 대한 자세한 내용은 [객체에 대한 상속된 권한 보기](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## 보고서 공유 {#share-a-report}

목록에서 한 보고서나 여러 보고서를 공유하는 것은 동일합니다.

1. 보고서 목록으로 이동하고 하나 이상의 보고서를 선택한 다음 **공유**.

   또는

   한 보고서의 이름을 클릭한 다음 **보고서 작업 > ****공유**.

   ![](assets/qs-report-actions-sharing.png)

1. 표시되는 상자에서 **사람, 팀, 역할, 그룹 또는 회사 추가...** 필드에서 보고서를 공유할 사용자, 팀, 작업 역할, 그룹 또는 회사의 이름을 입력하고 키를 누릅니다 **Enter 키** 가 표시되는 경우입니다.

1. 추가한 이름에 대한 액세스 수준을 조정하려면 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 아래 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보기</td> 
      <td> <p>수신자가에 있는 보고서를 볼 수 있도록 합니다. <strong>보고서</strong> <img src="assets/reports-in-main-menu.png"> 영역 및 실행</p> <p>을(를) 클릭합니다 <strong>고급 설정</strong> 사용자 또는 사용자가 <strong>공유</strong> 시스템에 있는 누구와도 함께 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리함</td> 
      <td> <p>수신자가 보고서에 대한 전체 편집 액세스를 허용합니다.</p> <p>을(를) 클릭합니다 <strong>고급 설정</strong> 사용자 또는 사용자가 <strong>삭제</strong> 시스템 및 <strong>공유</strong> 시스템에 있는 누구와도 함께 합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 이전 두 단계를 반복하여 목록에 다른 이름을 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) **기어** 아이콘 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 공유 상자의 오른쪽 상단 모서리에서 다음 옵션 중 하나를 선택합니다.

   * **외부 사용자에게 공개합니다.** 다른 사용자와 공유할 수 있는 URL을 생성하려면 이 옵션을 선택합니다. URL을 가진 모든 사용자는 Adobe Workfront 라이센스가 없는 보고서에 액세스할 수 있습니다.

      >[!CAUTION]
      >
      >외부 사용자와 기밀 정보가 포함된 개체를 공유할 때는 주의해야 합니다. 이를 통해 Workfront 사용자 또는 조직의 구성원이 아니더라도 정보를 볼 수 있습니다.

      >[!NOTE]
      >
      >보고서에 프롬프트가 있고 공개적으로 공유하는 경우 보고서를 실행하는 사용자가 프롬프트를 사용하여 보고서를 실행할 수 있으려면 Workfront에 로그인해야 합니다. Workfront에 로그인할 수 없으면 메시지가 적용되지 않은 보고서가 표시됩니다. 프롬프트를 통해 보고서를 공유하는 제한 사항에 대한 자세한 내용은 섹션을 참조하십시오 [메시지 보고서 공유 제한](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) 기사 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **시스템 전체에 표시:** 보고서에 대한 액세스 권한이 있는 Workfront의 모든 사람이 보고서를 볼 수 있도록 이 옵션을 선택합니다.

1. **저장**&#x200B;을 클릭합니다.
