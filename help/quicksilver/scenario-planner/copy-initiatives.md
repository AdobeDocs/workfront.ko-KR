---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 이니셔티브 복사
description: 기존 이니셔티브를 복사하여 이니셔티브를 생성할 수 있습니다. 사용자가 생성한 계획이나 다른 사용자가 사용자와 공유하는 계획에 이니셔티브를 복사할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# [!DNL Scenario Planner]에서 이니셔티브 복사

<!--Audited: 07/2024-->

기존 이니셔티브를 복사하여 이니셔티브를 생성할 수 있습니다. 사용자가 생성한 계획이나 다른 사용자가 사용자와 공유하는 계획에 이니셔티브를 복사할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 플랜*</p> </td> 
   <td> <ul></li>
   <li><p>새로운 기능: Ultimate </p></li>
   <p>새 Workfront Select 또는 Workfront Prime 플랜에는 시나리오 플래너를 사용할 수 없습니다. </p>
   <li><p>현재: [!UICONTROL Business] 이상</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td> <p>새로운 기능: 밝게 또는 높음</p> 
   <p>현재: [!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td>제품* </td> 
   <td> <ul><li><p>새로운 Workfront 플랜의 경우:</p><p> Adobe Workfront</li></p>
   <li><p>현재 Workfront 플랜의 경우: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront 시나리오 플래너</p></li></ul>

<p>자세한 내용은 [!DNL Scenario Planner]</a>을(를) 사용하는 데 필요한 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">액세스를 참조하십시오. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 </td> 
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 권한: [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> <p>플랜에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">플랜에 대한 액세스 요청 [!DNL Scenario Planner]</a>을(를) 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 이니셔티브 복사

이니셔티브를 복사할 때에는 다음 사항을 고려하십시오.

* 이니셔티브를 복사하면 복사본이 원래 이니셔티브와 동일한 계획에 배치됩니다.
* 이니셔티브를 복사하면 원래 이니셔티브에서 새 이니셔티브에 다음 정보가 복사되고 추가됩니다.

   * [!UICONTROL 기간]
   * [!UICONTROL 작업 역할]
   * [!UICONTROL 사람] 및 [!UICONTROL 고정 비용]
   * [!UICONTROL 계획된 혜택]

* 이니셔티브가 최초 이니셔티브에 있는 경우 이니셔티브를 복사하면 계획에 대한 다음 정보를 수정할 수 있습니다.

   * 필요한 작업 역할 양
   * [!UICONTROL 비용]
   * [!UICONTROL 계획 사용률]
   * 작업 역할 사용률
   * [!UICONTROL 순 값]

* 프로젝트를 가져와서 만들었거나 프로젝트에 한 번 이상 게시한 이니셔티브를 복사하면 다음과 같은 의미가 있습니다.

   * 이니셔티브와 연계된 프로젝트와 중복되지 않습니다.
   * 복사된 이니셔티브가 프로젝트에 연결되지 않습니다.
   * 한 번 이상 게시된 프로젝트의 [!DNL Scenario Planner] 섹션은 수정되지 않습니다.

  프로젝트에 이니셔티브를 게시하는 방법에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.

  프로젝트를 가져와서 이니셔티브를 만드는 방법에 대한 자세한 내용은 [프로젝트를  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)의 플랜에 가져오기 를 참조하십시오.

## 이니셔티브 복사

{{step1-to-scenario-planner}}

계획 목록이 표시됩니다.

1. 계획명을 눌러 계획을 연 다음 복사할 이니셔티브를 찾습니다.
1. 복사할 이니셔티브 또는 이니셔티브의 왼쪽에 있는 상자를 선택한 다음, 플랜 하단에 나타나는 메뉴에서 **[!UICONTROL 복사]**&#x200B;를 클릭합니다.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront]이(가) 이니셔티브를 즉시 복사하고 마지막으로 선택한 이니셔티브 아래에 배치합니다.

   복사된 이니셔티브의 이름은 *[!UICONTROL 복사본]`<Name of original initiative>`*&#x200B;입니다.

   >[!NOTE]
   >
   >새 이니셔티브를 삽입하는 위치에 따라 기존 이니셔티브의 수가 변경될 수 있습니다.

1. 복사된 이니셔티브의 이름을 업데이트합니다.

   >[!TIP]
   >
   >다시 복사하려는 경우 혼동을 피하기 위해 항상 이니셔티브의 이름을 업데이트하는 것이 좋습니다.

1. (선택 사항) 새로 생성된 이니셔티브의 우선 순위를 업데이트합니다.

   이니셔티브 우선 순위에 대한 자세한 내용은 [이니셔티브 우선 순위 업데이트 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md)를 참조하십시오.

1. 변경 내용을 저장하려면 **[!UICONTROL 계획 저장]**&#x200B;을 클릭하세요.
