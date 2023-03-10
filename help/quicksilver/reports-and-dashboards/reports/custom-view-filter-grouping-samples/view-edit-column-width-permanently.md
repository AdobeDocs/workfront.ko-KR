---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 열 너비를 영구적으로 편집'
description: 원하는 너비와 일치하도록 여백을 드래그하여 놓아 열 너비를 일시적으로 수정할 수 있습니다. 자세한 내용은 열 너비 및 순서 수정을 참조하십시오.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 보기: 열 너비를 영구적으로 편집

원하는 너비와 일치하도록 여백을 드래그하여 놓아 열 너비를 일시적으로 수정할 수 있습니다. 자세한 내용은 [열 너비 및 순서 수정](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

보기를 편집할 때 열에서 텍스트 모드를 사용하여 모든 뷰의 열 너비를 영구적으로 변경할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 열 너비를 영구적으로 편집

>[!IMPORTANT]
>
>문서의 &quot;임시 열 너비 및 순서 수정&quot; 섹션에 설명된 대로 열의 너비를 수동으로 수정하는 경우 [열 너비 및 순서 수정](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 열 너비를 영구적으로 수정하면 열 너비가 수동 크기 조정에 따라 유지되며 다음 단계에 따라 업데이트된 열 너비를 덮어씁니다. 캐시를 지우거나 다른 브라우저에서 로그인한 후 다음 단계에서 정의한 너비에 따라 열을 볼 수 있습니다.

1. 개체 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 클릭 **열 추가** 새 열을 추가하려면

   또는

   기존 열의 열 헤더를 클릭합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역을 마우스로 가리킨 다음 **텍스트를 편집하려면 클릭하십시오.**.
1. 열의 텍스트 모드에 다음 코드를 추가합니다.

   ```
   width=200
   usewidths=true
   ```

   대상 **너비** 선을 그리려면 열에 표시할 너비를 나타내는 숫자(픽셀 단위)를 지정합니다.

1. 클릭 **저장**, 그런 다음 **보기 저장**.
