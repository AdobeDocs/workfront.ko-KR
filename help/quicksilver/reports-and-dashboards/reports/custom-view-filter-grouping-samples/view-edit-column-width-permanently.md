---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열의 너비를 영구적으로 편집'
description: 원하는 너비와 일치하도록 여백을 드래그 앤 드롭하여 열의 너비로 일시적으로 수정할 수 있습니다. 자세한 내용은 열 너비 및 순서 수정을 참조하십시오.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 보기: 열의 너비를 영구적으로 편집

<!-- Audited: 1/2024 -->

원하는 너비와 일치하도록 여백을 드래그 앤 드롭하여 열의 너비로 일시적으로 수정할 수 있습니다. 자세한 내용은 [열 너비 및 순서 수정](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

뷰의 열 너비를 영구적으로 변경하려면 뷰를 편집할 때 열에서 텍스트 모드를 사용해야 합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>신규:<ul><li>보기를 수정하는 기여자</li><li>보고서를 수정하는 표준</li></ul></p><p>또는</p>현재:<ul><li>보기 수정 요청</li><li>보고서 수정 계획</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 열의 너비를 영구적으로 편집

>[!IMPORTANT]
>
>섹션에 설명된 대로 열의 너비를 수동으로 수정하는 경우 [임시로 열 너비 및 순서 수정](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) 이 문서에서 [열 너비 및 순서 수정](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 열 너비를 영구적으로 수정한 후에는 수동 크기 조정에 따라 열 너비가 유지됩니다. 이 경우 다음 단계에 따라 업데이트된 열의 너비를 덮어씁니다. 캐시를 지우거나 다른 브라우저에서 로그인한 후 다음 단계에 정의된 너비에 따라 열을 볼 수 있습니다.
>
>텍스트 모드 인터페이스를 사용할 때 열의 너비를 사용자 정의하는 방법에 대한 자세한 내용은 [Adobe Workfront 용어 목록](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. 개체 목록으로 이동합니다.
1. 다음에서 **보기** 드롭다운 메뉴, 클릭 **새 보기**.

1. 클릭 **열 추가** 새 열을 추가합니다.

   또는

   기존 열의 열 헤더를 클릭합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 열의 텍스트 모드에 다음 코드를 추가합니다.

   ```
   width=200
   usewidths=true
   ```

   의 경우 **폭** 행에서 열에 표시할 너비를 나타내는 숫자(픽셀 단위)를 지정합니다.

1. 클릭 **저장**, 그런 다음 **보기 저장**.


