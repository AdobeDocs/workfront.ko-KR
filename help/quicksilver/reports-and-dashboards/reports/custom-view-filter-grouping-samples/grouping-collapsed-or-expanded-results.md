---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 텍스트 모드를 사용하여 그룹화 결과를 축소할지 또는 확장할지 표시'
description: '그룹화: 텍스트 모드를 사용하여 그룹화 결과를 축소할지 또는 확장할지 여부를 나타냅니다.'
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# 그룹화: 텍스트 모드를 사용하여 그룹화 결과를 축소할지 또는 확장할지 여부를 나타냅니다.

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

표준 Report Builder를 사용하여 그룹화의 결과가 목록 또는 보고서에 축소되거나 확장되어 표시되어야 하는지 여부를 나타낼 수 있습니다. 그룹화의 결과는 기본적으로 확장되어 표시됩니다. 그룹화 만들기에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)를 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* 목록을 볼 때 수동으로 그룹화를 조정하면 Adobe Workfront은 로그아웃하기 전까지 수동 기본 설정을 기억합니다. 다시 로그인하면 이 설정에 따라 목록이 표시됩니다.
>* 차트 요소에서 액세스한 후 그룹화 결과는 항상 확장되어 표시됩니다.
>

텍스트 모드를 사용하여 그룹화를 확장할지 축소할지 여부를 나타낼 수도 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 텍스트 모드를 사용하여 그룹화 결과를 축소할지 또는 확장할지 여부를 나타냅니다

1. 개체 목록으로 이동합니다.
1. **그룹화**&#x200B;드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. 그룹화를 추가한 다음 **텍스트 모드로 전환**&#x200B;을 클릭합니다.

   또는

   그룹화가 이미 텍스트 모드에 있는 경우 축소하여 표시할 그룹화 수준에 다음 코드를 추가합니다.

   `group.0.iscollapsed=true`

1. (선택 사항) 그룹화를 확장하여 표시하려면 다음 코드를 해당 그룹화 수준에 추가합니다.

   `group.0.iscollapsed=false`

1. **완료**&#x200B;를 클릭한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 그룹화 이름을 업데이트한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
