---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 상위 작업 표시'
description: 아래 작업 필터를 적용하여 작업 작업을 표시할 수 있습니다. 작업 작업은 독립적으로 작업할 수 있고 다른 작업의 상위 작업이 아닌 작업입니다. 한 예에서 필터는 부모 자신이 될 수 있는 하위 작업을 식별합니다. 이 경우 작업 중이 아닙니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 필터: 상위 작업 표시

아래 작업 필터를 적용하여 작업 작업을 표시할 수 있습니다. 작업 작업은 독립적으로 작업할 수 있고 다른 작업의 상위 작업이 아닌 작업입니다. 한 예에서 필터는 부모 자신이 될 수 있는 하위 작업을 식별합니다. 이 경우 작업 중이 아닙니다.

>[!TIP]
>
>* 보고서에 두 개 이상의 필터를 추가하는 것이 적절할 경우 Report Builder 인터페이스를 사용하여 모든 필터를 추가하고 다른 모든 필터 규칙이 추가된 후 텍스트 모드로 전환 을 클릭하는 것이 좋습니다. 그런 다음 위에 언급된 대로 상위 작업 필터의 코드를 추가할 수 있습니다. 
* 보고서를 더 쉽게 읽을 수 있도록 프로젝트 이름에 대한 그룹을 추가하는 것이 좋습니다. 보고서에 그룹화를 추가하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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

## 하위 항목이 없는 작업 표시(상위 작업 가능)

다음 필터를 작업 보고서에 적용하여 하위 항목이 없는 작업을 표시할 수 있습니다. 부모가 알아서 하고, 자식도 될 수 있다.

1. 에서 **기본 메뉴** ![](assets/main-menu-icon.png)를 클릭합니다. **보고서.**

1. 클릭 **새 보고서**.
1. 선택 **작업 보고서**.
1. 클릭 **필터**.
1. 클릭 **필터 규칙 추가**.
1. 에서 **필드 이름 입력 시작..** 줄, 입력 시작 **하위 수**.

1. 선택 **같음(대/소문자 구분)** 수정자에 대해 을 입력한 다음 **0** 하위 항목 수.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   또는

   클릭 **텍스트 모드로 전환**, 텍스트 편집 창에서 다음 텍스트를 복사하여 붙여넣습니다. 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 클릭 **저장 + 닫기**.

   시스템에서 작업 중인 모든 작업에 대한 보고서를 가져옵니다. 이러한 작업 중 일부는 상위 작업을 가질 수 있지만, 상위 작업 자체는 아닙니다.

## 상위 작업 표시(하위 항목이 있을 수 있음)

다음 필터를 작업 보고서에 적용하여 상위 작업이 있는 작업을 표시할 수 있습니다. 즉, 하위 작업입니다. 하지만 이 필터는 해당 하위 항목을 제외하지 않으므로 이러한 작업은 자체 하위 항목도 가질 수 있습니다. 다른 작업의 부모인 하위 작업은 작업 작업으로 간주되지 않습니다.

1. 에서 **기본 메뉴** ![](assets/main-menu-icon.png)를 ** 보고서 를 클릭합니다.
1. 클릭 **새 보고서**.
1. 선택 **작업 보고서**.
1. 클릭 **필터**.
1. 클릭 **필터 규칙 추가**.
1. 에서 **필드 이름 입력 시작..** 줄, 입력 시작 **상위 ID**.
1. 선택 **비어 있지 않음** 수정자.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   또는

   클릭 **텍스트 모드로 전환**, 텍스트 편집 창에서 다음 텍스트를 복사하여 붙여넣습니다. 

   `parentID_Mod=notblank`

1. 클릭 **저장 + 닫기**.

   이렇게 하면 상위 및 해당 부모의 하위 작업이 있는 시스템의 모든 작업에 대한 보고서가 가져옵니다. 이러한 작업 중 일부는 부모 자신들이 될 수 있습니다.

## 1차 하위 구성요소 및 상위 항목 없이 작업 표시(독립형 작업)

작업 보고서에 다음 필터를 적용하여 독립 실행형 작업 작업을 표시할 수 있습니다. 이러한 작업은 상위 항목이 없고 자신의 하위 항목이 없습니다.

1. 에서 **기본 메뉴** ![](assets/main-menu-icon.png)를 클릭합니다. **보고서.**
1. 클릭 **새 보고서**.
1. 선택 **작업 보고서**.
1. 클릭 **필터**.
1. 클릭 **필터 규칙 추가** 그리고 **필드 이름 입력 시작..** 라인 시작 입력 **하위 수** 선택 **같음(대/소문자 구분)** 수정자에 대해 을 입력한 다음 **0** 하위 항목 수.
1. 클릭 **다른 필터 규칙 추가** 그리고 **필드 이름 입력 시작..** 라인 시작 입력 **상위 ID**&#x200B;를 선택하고 을 선택합니다. **비어 있음**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   또는

   6-7단계 대신 **텍스트 모드로 전환** 텍스트 편집 창에서 다음 텍스트를 복사하여 붙여넣습니다. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 클릭 **저장 + 닫기**.

   부모나 자식이 없는 시스템의 모든 작업에 대한 보고서를 가져옵니다. 독립형 작업 작업입니다.
