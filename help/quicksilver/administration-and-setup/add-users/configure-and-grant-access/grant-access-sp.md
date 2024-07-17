---
title: 시나리오 플래너에 대한 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 시나리오 플래너에 대한 사용자의 액세스 권한을 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 시나리오 플래너에 대한 액세스 권한 부여

[액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 Adobe Workfront 관리자는 액세스 수준을 사용하여 시나리오 플래너에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

Scenario Planner에 대한 액세스 권한 외에도 시스템 관리자가 아닌 액세스 레벨의 사용자는 계획에 포함된 예산, 비용 및 작업 역할 비율과 같은 재무 정보를 볼 수 있도록 재무 데이터에 대한 액세스 권한도 보유해야 합니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>비즈니스 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상. 자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">라이선스 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 시나리오 플래너에 대한 추가 라이선스를 구입해야 합니다.</p> <p>Workfront 시나리오 플래너를 얻는 방법에 대한 자세한 내용은 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">시나리오 플래너를 사용하는 데 필요한 액세스</a>를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>시나리오 플래너에 대한 액세스 권한 이상 보기</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> <p>플랜에 대한 권한 이상 보기</p> <p>플랜에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">시나리오 플래너의 플랜에 대한 액세스 요청</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 액세스 수준을 사용하여 시나리오 플래너에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 이 액세스 수준에 사용할 **시나리오 플래너** 오른쪽에 있는 옵션을 클릭합니다.

   >[!NOTE]
   >
   >요청 또는 외부 라이선스 유형에서는 시나리오 플래너에 대한 보기 또는 편집 액세스를 허용하지 않습니다.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. 완료되면 **저장**&#x200B;을 클릭하세요.

## 라이선스 유형별 시나리오 플래너에 액세스

각 액세스 수준의 사용자가 시나리오 플래너로 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)의 [시나리오 플래너 영역](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) 섹션을 참조하십시오.

## 액세스 수준 설정별 시나리오 플래너 액세스

다음 정보는 액세스 수준 설정을 사용하여 Workfront Scenario Planner의 정보에 대한 사용자 액세스를 제어하는 방법을 이해하는 데 도움이 됩니다.

* [액세스 권한 없음](#no-access)
* [액세스 보기](#view-access)
* [액세스 권한 편집](#edit-access)

### 액세스 권한 없음 {#no-access}

시나리오 플래너에 대한 액세스 권한이 없는 사용자는 레이아웃 템플릿에 추가될 때 기본 메뉴에서 시나리오 아이콘을 볼 수 없고 시나리오 플래너와 공유되는 계획 및 이니셔티브를 볼 수 없습니다. 계획 링크가 시나리오 플래너에 대한 액세스 권한이 없는 사용자와 공유되는 경우, 사용자는 계획을 보거나 편집할 수 없습니다.

### 액세스 권한 보기 {#view-access}

시나리오 플래너에 대한 보기 액세스 권한이 있는 사용자는 다음을 수행할 수 있습니다.

* 다른 사용자가 공유한 계획 링크를 클릭하지 않는 한 계획 영역이 비어 있더라도 기본 메뉴 ![](assets/esp-icon-in-main-menu.png)에서 시나리오 아이콘을 봅니다.
* 다른 사용자가 플랜에 대한 링크를 공유할 때 플랜을 봅니다.

  여기에는 플랜에 있는 모든 작업 역할 정보가 포함됩니다.

  또한 수신자 사용자도 재무 데이터에 액세스할 수 있는 경우 플랜에 대한 작업 역할 비율 및 비용 정보가 포함됩니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

### 액세스 권한 편집 {#edit-access}

시나리오 플래너에 대한 편집 액세스 권한이 있는 사용자는 다음을 수행할 수 있습니다.

* 메인 메뉴 ![](assets/esp-icon-in-main-menu.png)에서 시나리오 아이콘을 보고 이를 사용하여 계획 데이터에 액세스합니다.
* 계획을 만듭니다.
* 자신이 생성하는 계획을 보고, 편집하고, 삭제합니다.
* 공유 링크를 사용하여 액세스하는 다른 사용자의 계획을 보고, 편집하고, 삭제합니다.

  여기에는 플랜에 모든 작업 역할 정보가 포함됩니다.

  또한 수신자 사용자가 재무 데이터에 액세스할 수 있는 경우 플랜에 대한 작업 역할 비율 및 비용 정보도 포함됩니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.
