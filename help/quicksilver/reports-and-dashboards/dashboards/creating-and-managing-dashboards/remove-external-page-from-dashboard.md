---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드에서 외부 페이지 제거
description: 더 이상 필요하지 않은 경우 대시보드에서 외부 페이지를 제거할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# 대시보드에서 외부 페이지 제거

<!-- Audited: 1/2025 -->

더 이상 필요하지 않은 경우 대시보드에서 외부 페이지를 제거할 수 있습니다.

그러나 외부 페이지는 Adobe Workfront에서 만든 후에는 삭제할 수 없습니다. API를 사용해야만 외부 페이지를 삭제할 수 있습니다. Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md)을 참조하세요. 외부 페이지 만들기에 대한 자세한 내용은 [외부 웹 페이지를 대시보드에 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스</strong></td> 
   <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>플랜</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>대시보드에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 대시보드에서 외부 페이지 제거

1. 삭제할 외부 페이지가 포함된 대시보드로 이동합니다.

1. **대시보드 작업**&#x200B;을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   ![](assets/unshimmed-edit-dashboard.png)

1. 화면 오른쪽에서 제거할 외부 페이지를 찾은 다음 **삭제** 아이콘 ![](assets/delete.png)을(를) 클릭합니다.

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 왼쪽 아래에서 **저장 + 닫기**&#x200B;를 클릭합니다.

   이렇게 하면 선택한 대시보드에서 외부 페이지가 제거됩니다. 외부 페이지는 Workfront에 유지되며 보고서에서 액세스할 수 있습니다. 자세한 내용은 [대시보드에 외부 웹 페이지 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) 문서의 &quot;보고서에서 외부 페이지 보기&quot; 섹션을 참조하십시오.
