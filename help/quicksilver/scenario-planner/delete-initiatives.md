---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 계획자에서 이니셔티브 삭제
description: 생성한 계획이나 다른 사용자가 사용자와 공유한 계획에 대한 이니셔티브를 삭제할 수 있습니다. 삭제한 이니셔티브는 복구할 수 없습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# 에서 이니셔티브 삭제 [!DNL Scenario Planner]

생성한 계획이나 다른 사용자가 사용자와 공유한 계획에 대한 이니셔티브를 삭제할 수 있습니다. 삭제한 이니셔티브는 복구할 수 없습니다.

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
   <td> <p>[!DNL Adobe Workfront]<b> 라이센스*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td><b>제품</b> </td> 
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다. </p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!UICONTROL Scenario Planner]를 사용하는 데 필요한 액세스</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>[!UICONTROL Edit] 액세스 이상의 [!DNL Scenario Planner]</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>계획에 대한 [!UICONTROL Manage] 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 이니셔티브 삭제

이니셔티브를 삭제할 때 다음 사항을 고려하십시오.

* 이니셔티브를 삭제하면 필요한 작업 역할과 이니셔티브와 연관된 비용 정보가 계획에서 제거됩니다.
* 프로젝트를 가져와서 만든 이니셔티브를 삭제하면 이니셔티브와 연결된 프로젝트가 삭제되지 않습니다.
* 프로젝트에 한 번 이상 게시된 이니셔티브를 삭제하면 다음과 같은 결과가 발생합니다.

   * 이니셔티브가 시나리오에서 삭제되지만 [!DNL Scenario Planner] 영역은 [!UICONTROL 프로젝트 세부 사항] 섹션을 참조하십시오.
   * 삭제한 이니셔티브가 시나리오에서 유일한 게시된 이니셔티브인 경우 계획이 게시되었다는 표시자도 제거됩니다.

      프로젝트에 이니셔티브 게시에 대한 자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      프로젝트를 가져와서 이니셔티브를 만드는 방법에 대한 자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

한 번에 하나의 이니셔티브를 삭제하거나 여러 이니셔티브를 일괄적으로 삭제할 수 있습니다.

* [하나의 이니셔티브 삭제](#delete-one-initiative)
* [이니셔티브 일괄 삭제](#delete-initiatives-in-bulk)

### 하나의 이니셔티브 삭제 {#delete-one-initiative}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

   계획 목록이 표시됩니다.

1. 계획 이름을 눌러 연 다음 삭제할 이니셔티브를 찾습니다.
1. 다음 중 하나를 수행하십시오.

   * 을(를) 클릭합니다. **[!UICONTROL 추가 메뉴]** ![](assets/more-menu.png) 이니셔티브 이름의 오른쪽으로 이동한 다음 **[!UICONTROL 삭제]** > **[!UICONTROL 예, 삭제합니다]**.

   * 이니셔티브 왼쪽에 있는 상자를 선택한 다음 **[!UICONTROL 삭제]** 계획 하단에 나타나는 부동 메뉴에서 **[!UICONTROL 예, 삭제합니다]**.

   계획 및 해당 작업 역할과 비용 정보가 계획에서 삭제됩니다.

1. 클릭 **[!UICONTROL 계획 저장]** 변경 사항을 저장하려면 을 클릭합니다.

### 이니셔티브 일괄 삭제 {#delete-initiatives-in-bulk}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

   계획 목록이 표시됩니다.

1. 계획 이름을 눌러 연 다음 삭제할 이니셔티브를 찾습니다.
1. 삭제할 이니셔티브 왼쪽에 있는 상자를 선택한 다음 **[!UICONTROL 삭제]** 계획 하단에 나타나는 메뉴에서 **[!UICONTROL 예, 삭제합니다.]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   계획에서 이니셔티브 및 해당 직무 및 비용 정보가 삭제됩니다.

1. 클릭 **[!UICONTROL 계획 저장]** 변경 사항을 저장하려면 을 클릭합니다.
