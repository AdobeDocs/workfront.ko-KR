---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 상위 작업 표시'
description: 아래 작업 필터를 적용하여 작업 작업을 표시할 수 있습니다. 작업 작업은 독립적으로 작업할 수 있는 작업이며 다른 작업의 상위 작업이 아닙니다. 한 예에서 필터는 상위 자신일 수 있는 하위 작업을 식별합니다. 이 경우 작업이 아닙니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 필터: 상위 작업 표시

아래 작업 필터를 적용하여 작업 작업을 표시할 수 있습니다. 작업 작업은 독립적으로 작업할 수 있는 작업이며 다른 작업의 상위 작업이 아닙니다. 한 예에서 필터는 상위 자신일 수 있는 하위 작업을 식별합니다. 이 경우 작업이 아닙니다.

>[!TIP]
>
>* 보고서에 필터를 두 개 이상 추가하는 것이 좋다면 Report Builder 인터페이스를 사용하여 모든 필터를 추가하고, 다른 필터 규칙이 모두 추가된 후 텍스트 모드로 전환을 클릭하는 것이 좋습니다. 그런 다음 위에 언급된 대로 상위 작업 필터에 대한 코드를 추가할 수 있습니다. 
* 또한 보고서를 읽기 쉽게 하려면 프로젝트 이름에 대한 그룹화를 추가하는 것이 좋습니다. 보고서에 그룹화를 추가하는 방법에 대한 자세한 내용은 문서 를 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>필터 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 하위 항목이 없는 작업 표시(상위 항목이 있을 수 있음)

다음 필터를 작업 보고서에 적용하여 하위 항목이 없는 작업을 표시할 수 있습니다. 그들은 그들 자신의 부모를 가질 수 있고 다른 과제의 자식이 될 수 있다.

1. 다음에서 **메인 메뉴** ![](assets/main-menu-icon.png), 클릭 **보고서.**

1. 클릭 **새 보고서**.
1. 선택 **작업 보고서**.
1. 클릭 **필터**.
1. 클릭 **필터 규칙 추가**.
1. 다음에서 **필드 이름을 입력하세요...** 줄, 입력 시작 **하위 수**.

1. 선택 **같음(대/소문자 구분)** 수정자에 대해 을 입력한 다음 **0** 자녀 수.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   또는

   클릭 **텍스트 모드로 전환**&#x200B;를 클릭하고 텍스트 편집 창에서 다음 텍스트를 복사하여 붙여넣습니다. 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 클릭 **저장 + 닫기**.

   이렇게 하면 시스템에서 작업 중인 모든 작업에 대한 보고서를 가져옵니다. 이러한 작업 중 일부는 상위 항목을 가질 수 있지만 상위 작업 자체는 아닙니다.

## 부모와 함께 작업 표시(자녀가 있을 수 있음)

작업 보고서에 다음 필터를 적용하여 상위 작업(하위 작업)을 표시할 수 있습니다. 단, 이러한 작업은 필터가 하위 항목을 제외하지 않으므로 하위 항목도 가질 수 있습니다. 다른 작업의 부모가 되는 하위 작업은 작업 작업으로 간주되지 않습니다.

1. 다음에서 **메인 메뉴** ![](assets/main-menu-icon.png)**보고서)를 클릭합니다.
1. 클릭 **새 보고서**.
1. 선택 **작업 보고서**.
1. 클릭 **필터**.
1. 클릭 **필터 규칙 추가**.
1. 다음에서 **필드 이름을 입력하세요...** 줄, 입력 시작 **상위 ID**.
1. 선택 **비어 있지 않음** 수정자.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   또는

   클릭 **텍스트 모드로 전환**&#x200B;를 클릭하고 텍스트 편집 창에서 다음 텍스트를 복사하여 붙여넣습니다. 

   `parentID_Mod=notblank`

1. 클릭 **저장 + 닫기**.

   이렇게 하면 상위가 있고 해당 상위의 하위 작업이 있는 시스템의 모든 작업에 대한 보고서를 가져옵니다. 이러한 작업 중 일부는 상위 자체가 될 수 있습니다.

## 하위 항목과 상위 항목이 없는 작업 표시(독립 실행형 작업)

다음 필터를 작업 보고서에 적용하여 독립형 작업 작업을 표시할 수 있습니다. 이러한 작업에는 상위가 없으며 자신의 하위 항목도 없습니다.

1. 다음에서 **메인 메뉴** ![](assets/main-menu-icon.png), 클릭 **보고서.**
1. 클릭 **새 보고서**.
1. 선택 **작업 보고서**.
1. 클릭 **필터**.
1. 클릭 **필터 규칙 추가** 및 **필드 이름을 입력하세요...** 줄 시작 입력 **하위 수** 선택 **같음(대/소문자 구분)** 수정자에 대해 을 입력한 다음 **0** 자녀 수.
1. 클릭 **다른 필터 규칙 추가** 및 **필드 이름을 입력하세요...** 줄 시작 입력 **상위 ID**&#x200B;을 선택한 다음 을 선택합니다. **비어 있음**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   또는

   6~7단계 대신 **텍스트 모드로 전환** 텍스트 편집 창에서 다음 텍스트를 복사하여 붙여넣습니다. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 클릭 **저장 + 닫기**.

   이렇게 하면 상위 항목이나 하위 항목이 없는 시스템의 모든 작업에 대한 보고서를 가져옵니다. 독립 실행형 작업 작업입니다.
