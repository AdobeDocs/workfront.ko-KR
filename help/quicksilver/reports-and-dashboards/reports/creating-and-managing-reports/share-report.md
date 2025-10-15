---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Adobe Workfront에서 보고서 공유
description: Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 보고서를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 문제에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 보고서, 대시보드 및 달력에 대한 액세스 권한 부여를 참조하십시오.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 1%

---

# Adobe Workfront에서 보고서 공유

<!-- Audited: 11/2024 -->

Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 보고서를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 문제에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [보고서, 대시보드 및 일정에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)를 참조하십시오.

사용자에게 부여된 액세스 수준과 함께 공유할 액세스 권한이 있는 특정 보고서를 보거나 관리할 수 있는 권한을 부여할 수도 있습니다. 액세스 수준 및 사용 권한에 대한 자세한 내용은 [액세스 수준 및 사용 권한이 함께 작동하는 방법](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)을 참조하세요.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아닌 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
      <p>라이트</p>
      <p>검토</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한 이상 보기</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 이상 보기</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보고서 공유에 대한 고려 사항

아래 고려 사항 외에 [보고서, 대시보드 및 일정 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)도 참조하십시오.

* 만든 보고서를 다른 개인, 팀, 그룹, 작업 역할 또는 회사와 공유할 수 있습니다. 다른 사용자가 만들고 공유한 보고서를 공유할 수도 있습니다.
* 전체 조직과 공유하거나 공개로 설정할 수도 있습니다. 보고서를 공개하면 다른 사용자와 공유할 수 있는 URL이 생성됩니다.
* 개별 보고서를 공유하거나 보고서 목록에서 여러 보고서를 공유할 수 있습니다.

## 보고서를 공유하는 방법

다음과 같은 방법으로 Workfront에서 보고서를 공유할 수 있습니다.

* 아래 [보고서 공유](#share-a-report) 섹션에 설명된 대로 수동으로 실행하십시오.
* 공유된 보고서가 포함된 대시보드에서 보기 권한을 상속하여 자동으로 수행합니다. 개체에 상속된 사용 권한을 보는 방법에 대한 자세한 내용은 [개체에 상속된 사용 권한 보기](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)를 참조하십시오.

## 보고서 공유 {#share-a-report}

목록에서 하나 이상의 보고서를 공유하는 것은 동일합니다.

1. 보고서 목록으로 이동하여 하나 이상의 보고서를 선택한 다음 **공유**&#x200B;를 클릭합니다.

   또는

   한 보고서의 이름을 클릭한 다음 **보고서 작업 >****공유**&#x200B;를 클릭합니다.

   ![](assets/unshimmed-report-actions-sharing.png)

1. 표시되는 상자에서 **사람, 팀, 역할, 그룹 또는 회사 추가..** 필드에 보고서를 공유할 사용자, 팀, 작업 역할, 그룹 또는 회사의 이름을 입력한 다음 이름이 표시되면 **Enter**&#x200B;를 누릅니다.

1. 추가한 이름에 대한 액세스 수준을 조정하려면 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 아래 옵션 중 하나를 선택하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보기</td> 
      <td> <p>받는 사람이 <strong>보고서</strong> 영역에서 보고서를 보고 실행할 수 있도록 허용합니다.</p> <p><strong>고급 설정</strong>을 클릭하여 사용자 또는 사용자가 시스템 내의 모든 사용자와 이 설정을 <strong>공유</strong>할 수 있게 할지 여부를 지정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리함</td> 
      <td> <p>수신자가 보고서에 대한 전체 편집 액세스 권한을 가질 수 있도록 허용합니다.</p> <p><strong>고급 설정</strong>을 클릭하여 사용자 또는 사용자가 시스템에서 보고서를 <strong>삭제</strong>하고 시스템의 모든 사용자와 <strong>공유</strong>할 수 있도록 할지 여부를 지정할 수 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 앞의 2단계를 반복하여 다른 이름을 목록에 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) 공유 상자에서 **초대된 사람만 액세스할 수 있음** 드롭다운 메뉴를 클릭한 후 다음 옵션 중 하나를 선택합니다.

   * **초대된 사람만 액세스할 수 있습니다** 보고서에 대한 액세스 권한이 부여된 사용자만 볼 수 있도록 이 옵션을 선택하십시오.

   * **시스템의 모든 사용자가 볼 수 있습니다** 보고서에 대한 액세스 권한이 있는 모든 Workfront 사용자가 보고서를 볼 수 있도록 이 옵션을 선택하십시오.

1. (선택 사항) 공유 상자의 오른쪽 위 모서리에 있는 **톱니바퀴** 아이콘 ![톱니바퀴 아이콘 설정](assets/gear-icon-settings-with-dn-arrow.jpg)을 클릭한 다음 선택적으로 다음 옵션을 선택합니다.

   * **외부 사용자에게 공개하기** 다른 사용자와 공유할 수 있는 URL을 생성하려면 이 옵션을 선택하십시오. URL이 있는 사람은 Adobe Workfront 라이선스가 없어도 보고서에 액세스할 수 있습니다.

     >[!CAUTION]
     >
     >외부 사용자와 기밀 정보가 포함된 오브젝트를 공유할 때는 주의하는 것이 좋습니다. 이를 통해 Workfront 사용자 또는 조직의 일부가 아니더라도 정보를 볼 수 있습니다.

     >[!NOTE]
     >
     >보고서에 프롬프트가 있고 공개적으로 공유하는 경우 공개 공유 링크를 통해 보고서를 실행하는 사용자는 프롬프트를 사용하여 보고서를 실행할 수 없습니다. Workfront에 로그인하지 않고 공개 공유 링크를 사용하지 않고 보고서에 액세스하지 않으면 보고서에 적용된다는 프롬프트 없이 보고서가 표시됩니다. 프롬프트가 있는 보고서를 공유하는 제한 사항에 대한 자세한 내용은 문서 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports)의 [프롬프트 보고서 공유 제한](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) 섹션을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.
