---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 그룹화 결과를 텍스트 모드를 사용하여 축소하거나 확장해야 하는지 여부를 나타냅니다.'
description: '그룹화: 그룹화 결과를 텍스트 모드를 사용하여 축소하거나 확장해야 하는지 여부를 나타냅니다.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 그룹화: 텍스트 모드를 사용하여 그룹화 결과를 축소하거나 확장해야 하는지 여부를 나타냅니다

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

표준 Report Builder를 사용하여 그룹화 결과가 목록이나 보고서에 축소되거나 확장되어야 하는지 여부를 나타낼 수 있습니다. 기본적으로 그룹화 표시의 결과가 확장됩니다. 그룹 생성에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* 목록을 볼 때 수동으로 그룹화를 조정하면 Adobe Workfront은 로그아웃할 때까지 수동 환경 설정을 기억합니다. 다시 로그인하면 이 설정에 따라 목록이 표시됩니다.
>* 그룹 결과는 차트 요소에서 액세스한 후 항상 확장되어 표시됩니다.
>


텍스트 모드를 사용하여 그룹화를 확장할지 또는 축소할지 여부를 나타낼 수도 있습니다.

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

## 텍스트 모드를 사용하여 그룹화 결과를 축소하거나 확장해야 하는지 여부를 나타냅니다

1. 개체 목록으로 이동합니다.
1. 에서 **그룹화**&#x200B;드롭다운 메뉴에서 **새 그룹화**.

1. 그룹을 추가하고 을(를) 클릭합니다. **텍스트 모드로 전환**.

   또는

   그룹화가 이미 텍스트 모드인 경우 표시할 그룹화 수준에 다음 코드를 추가합니다.

   ```
   group.0.iscollapsed=true
   ```

1. (선택 사항) 그룹을 확장하려면 다음 코드를 해당 그룹화 수준에 추가합니다.

   ```
   group.0.iscollapsed=false
   ```

1. 클릭 **완료**, 그런 다음 **그룹화 저장**.
