---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너의 이니셔티브 복사
description: 기존 이니셔티브를 복사하여 이니셔티브를 생성할 수 있습니다. 사용자가 생성하는 계획이나 누군가가 사용자와 공유하는 계획에 대한 이니셔티브를 복사할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 에서 이니셔티브 복사 [!DNL Scenario Planner]

기존 이니셔티브를 복사하여 이니셔티브를 생성할 수 있습니다. 사용자가 생성하는 계획이나 누군가가 사용자와 공유하는 계획에 대한 이니셔티브를 복사할 수 있습니다.

## 액세스 요구 사항

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 플랜*</b> </p> </td> 
   <td>[!UICONTROL Business] 이상</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 라이선스</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td><b>제품</b> </td> 
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다.</p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>[!UICONTROL Edit] 액세스 이상의 [!DNL Scenario Planner]</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>계획에 대한 [!UICONTROL Manage] 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 이니셔티브 복사

이니셔티브를 복사할 때 다음 사항을 고려하십시오.

* 이니셔티브를 복사하면 원본 이니셔티브와 동일한 계획에 복사본이 배치됩니다.
* 이니셔티브 복사본을 복사하고 원래 이니셔티브의 다음 정보를 새 이니셔티브에 추가합니다.

   * [!UICONTROL 기간]
   * [!UICONTROL 작업 역할]
   * [!UICONTROL 사람] 및 [!UICONTROL 고정 비용]
   * [!UICONTROL 계획된 이익]

* 이니셔티브를 복사하면 원래 이니셔티브에 대한 정보가 있는 경우 계획에 대해 다음 정보를 수정할 수 있습니다.

   * 필수 작업 역할 양
   * [!UICONTROL 비용]
   * [!UICONTROL 계획 활용률]
   * 작업 역할 사용률
   * [!UICONTROL 순 가치]

* 프로젝트를 가져와서 만들었거나 프로젝트에 한 번 이상 게시된 이니셔티브를 복사하면 다음과 같은 결과가 발생합니다.

   * 이니셔티브와 연관된 프로젝트는 복제되지 않습니다.
   * 복사한 이니셔티브를 프로젝트에 연결하지 않습니다.
   * 이 변수는 [!DNL Scenario Planner] 섹션에 있는 마지막 항목이 될 필요가 없습니다.

   프로젝트에 이니셔티브 게시에 대한 자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   프로젝트를 가져와서 이니셔티브를 만드는 방법에 대한 자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## 이니셔티브 복사

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

   계획 목록이 표시됩니다.

1. 계획을 열 계획명을 클릭한 다음 복사할 이니셔티브를 찾습니다.
1. 복사할 이니셔티브 또는 이니셔티브 왼쪽에 있는 상자를 선택한 다음 **[!UICONTROL 복사]** 계획 하단에 나타나는 메뉴에서

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] 이니셔티브를 즉시 복사하고 마지막으로 선택한 이니셔티브 아래에 배치합니다.

   복사된 이니셔티브의 이름은 다음과 같습니다 *[!UICONTROL 의 사본]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >새 이니셔티브를 삽입하는 위치에 따라 기존 이니셔티브 수가 변경될 수 있습니다.

1. 복사된 이니셔티브의 이름을 업데이트합니다.

   >[!TIP]
   >
   >다시 복사하려는 경우 혼동하지 않도록 항상 이니셔티브 이름을 업데이트하는 것이 좋습니다.

1. (선택 사항) 새로 생성된 이니셔티브의 우선순위를 업데이트합니다.

   이니셔티브 우선 순위에 대한 자세한 내용은 [에서 이니셔티브 우선 순위 업데이트 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. 클릭 **[!UICONTROL 계획 저장]** 변경 사항을 저장하려면 을 클릭합니다.
