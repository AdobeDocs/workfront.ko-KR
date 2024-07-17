---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 이니셔티브 삭제
description: 자신이 생성한 계획이나 다른 사람이 나와 공유한 계획에서 이니셔티브를 삭제할 수 있습니다. 삭제한 이니셔티브는 복구할 수 없습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# [!DNL Scenario Planner]에서 이니셔티브 삭제

자신이 생성한 계획이나 다른 사람이 나와 공유한 계획에서 이니셔티브를 삭제할 수 있습니다. 삭제한 이니셔티브는 복구할 수 없습니다.

## 액세스 요구 사항

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 계획*</b> </p> </td> 
   <td>[!UICONTROL Business] 이상</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 라이선스*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td><b>제품</b> </td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 [!DNL Adobe Workfront Scenario Planner]에 대한 추가 라이선스를 구입해야 합니다. </p> <p>[!DNL Workfront Scenario Planner]을(를) 얻는 방법에 대한 자세한 내용은 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!UICONTROL Scenario Planner]</a>을(를) 사용하는 데 필요한 액세스 권한을 참조하십시오. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 이상: [!DNL Scenario Planner]</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> <p>플랜에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">플랜에 대한 액세스 요청 [!DNL Scenario Planner]</a>을(를) 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 이니셔티브 삭제

이니셔티브를 삭제할 때는 다음 사항을 고려하십시오.

* 이니셔티브를 삭제하면 필요한 작업 역할의 양과 이니셔티브와 관련된 비용 정보가 계획에서 제거됩니다.
* 프로젝트를 가져와서 만든 이니셔티브를 삭제해도 이니셔티브와 연결된 프로젝트는 삭제되지 않습니다.
* 프로젝트에 게시된 이니셔티브를 한 번 이상 삭제하면 다음과 같은 결과가 발생합니다.

   * 이니셔티브가 시나리오에서 삭제되었지만 [!DNL Scenario Planner] 영역은 [!UICONTROL 프로젝트 세부 정보] 섹션에 남아 있습니다.
   * 삭제한 이니셔티브가 시나리오에 게시된 유일한 이니셔티브인 경우 플랜이 게시되었다는 표시기도 제거됩니다.

     프로젝트에 이니셔티브를 게시하는 방법에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.

     프로젝트를 가져와서 이니셔티브를 만드는 방법에 대한 자세한 내용은 [의 플랜에 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) 를 참조하십시오.

한 번에 하나의 이니셔티브를 삭제하거나 여러 이니셔티브를 일괄적으로 삭제할 수 있습니다.

* [이니셔티브 하나 삭제](#delete-one-initiative)
* [일괄 이니셔티브 삭제](#delete-initiatives-in-bulk)

### 1개의 이니셔티브 삭제 {#delete-one-initiative}

1. **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 [!UICONTROL 시나리오]를 클릭합니다.

   계획 목록이 표시됩니다.

1. 계획명을 눌러 계획을 연 다음 삭제할 이니셔티브를 찾습니다.
1. 다음 중 하나를 수행하십시오.

   * 이니셔티브 이름의 오른쪽에 있는 **[!UICONTROL 추가 메뉴]** ![](assets/more-menu.png)를 클릭한 다음 **[!UICONTROL 삭제]** > **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   * 이니셔티브 왼쪽에 있는 상자를 선택한 다음, 플랜 하단에 나타나는 부동 메뉴에서 **[!UICONTROL 삭제]**&#x200B;를 클릭한 다음, **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   이니셔티브와 해당 작업 역할 및 비용 정보가 플랜에서 삭제됩니다.

1. 변경 내용을 저장하려면 **[!UICONTROL 계획 저장]**&#x200B;을 클릭하세요.

### 일괄 이니셔티브 삭제 {#delete-initiatives-in-bulk}

1. **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 [!UICONTROL 시나리오]를 클릭합니다.

   계획 목록이 표시됩니다.

1. 계획명을 눌러 계획을 연 다음 삭제할 이니셔티브를 찾습니다.
1. 삭제할 이니셔티브의 왼쪽에 있는 상자를 선택한 다음, 플랜 하단에 나타나는 메뉴에서 **[!UICONTROL 삭제]**&#x200B;를 클릭한 다음, **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   이니셔티브와 해당 작업 역할 및 비용 정보가 계획에서 삭제됩니다.

1. 변경 내용을 저장하려면 **[!UICONTROL 계획 저장]**&#x200B;을 클릭하세요.
