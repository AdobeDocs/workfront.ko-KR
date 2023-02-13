---
title: 감사 로그 보기 및 내보내기
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 시스템에서 모든 감사 로그 또는 특정 필터링 기준을 충족하는 감사 로그를 볼 수 있습니다. 감사 로그를 내보낼 수도 있습니다. 감사 로그는 지난 90일 동안 시스템에서 트리거된 사용자 변경 사항을 나열합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 감사 로그 보기 및 내보내기

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

시스템에서 모든 감사 로그 또는 특정 필터링 기준을 충족하는 감사 로그를 볼 수 있습니다. 감사 로그를 내보낼 수도 있습니다.

감사 로그는 지난 90일 동안 시스템에서 트리거된 사용자 변경 사항을 나열합니다.

모든 감사 로그 유형 및 이를 생성하는 항목에 대한 자세한 내용은 [감사 로그](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>플랜 </p> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 감사 로그 보기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **시스템 > 감사 로그**.
1. 에서 **로그 유형** 드롭다운 메뉴에서 보려는 감사 로그 유형을 선택합니다.

   **모든 로그 유형** 기본적으로 선택되어 있습니다.

   볼 수 있는 모든 감사 로그 유형 목록과 이러한 유형에 포함된 정보는 를 참조하십시오. [감사 로그](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (선택 사항) 사용 가능한 필터를 설정합니다.

   >[!NOTE]
   >
   >작업 유형 드롭다운 메뉴의 옵션은 선택한 감사 로그에 따라 다릅니다.

   ![](assets/audit-logs.jpg)

1. 클릭 **적용**.
1. (선택 사항) **필터 지우기** 를 눌러 필터에 대한 변경 사항을 재설정합니다.

## 감사 로그 내보내기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **시스템 > 감사 로그**.

1. 에서 **로그 유형** 드롭다운 메뉴에서 감사 로그를 선택합니다.

   **모든 로그 유형** 기본적으로 선택되어 있습니다.

1. 사용 가능한 필터를 설정한 다음 **적용**.

   >[!IMPORTANT]
   >
   >한 번에 50,000개 이상의 로그를 내보낼 수 없습니다. Workfront은 페이지에 표시되는 로그 수가 아니라 설정한 필터에 따라 로그를 내보냅니다. 페이지의 오른쪽 아래 모서리에서 필터링된 로그의 총 수를 볼 수 있습니다.

1. 클릭 **내보내기**.
