---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드에서 외부 페이지 제거
description: 외부 페이지가 더 이상 필요하지 않으면 대시보드에서 제거할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 대시보드에서 외부 페이지 제거

외부 페이지가 더 이상 필요하지 않으면 대시보드에서 제거할 수 있습니다.

그러나 외부 페이지는 Adobe Workfront에서 만든 후에는 삭제할 수 없습니다. API만 사용하여 외부 페이지를 삭제할 수 있습니다. Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md). 외부 페이지 만들기에 대한 내용은 [대시보드에 외부 웹 페이지 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>대시보드에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 대시보드에서 외부 페이지 제거

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 **대시보드**.
1. 외부 페이지를 제거할 대시보드를 선택한 다음 를 클릭합니다 **편집** ![](assets/edit-icon.png).

   ![편집 아이콘을 선택합니다.](assets/nwe-editdashboard2021-350x188.png)

1. 화면의 오른쪽에서 제거할 외부 페이지를 찾아 **삭제** 아이콘 ![](assets/delete.png).

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 클릭 **저장 + 닫기** 왼쪽 아래 모퉁이에 있습니다.

   그러면 선택한 대시보드에서 외부 페이지가 제거됩니다. 외부 페이지는 Workfront에 남아 있으며 보고서에서 액세스할 수 있습니다. 자세한 내용은 문서의 &quot;보고서에서 외부 페이지 보기&quot; 섹션을 참조하십시오 [대시보드에 외부 웹 페이지 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
