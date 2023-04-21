---
title: 시나리오 플래너에 대한 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 레벨을 사용하여 시나리오 플래너에 대한 사용자의 액세스를 정의할 수 있습니다.
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

Adobe Workfront 관리자는 액세스 레벨을 사용하여 다음에 설명된 대로 시나리오 플래너에 대한 사용자의 액세스를 정의할 수 있습니다 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

시나리오 플래너에 액세스할 수 있을 뿐만 아니라 비 시스템 관리자 액세스 수준을 가진 사용자도 재무 데이터에 액세스할 수 있어야 예산, 비용 및 작업 역할 비율과 같은 계획에 포함된 재무 정보를 볼 수 있습니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

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
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상 자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 시나리오 플래너에 대한 추가 라이센스를 구매해야 합니다.</p> <p>Workfront 시나리오 플래너를 가져오는 방법에 대한 자세한 내용은 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">시나리오 플래너를 사용하는 데 필요한 액세스</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>시나리오 플래너에 대한 액세스 또는 상위 보기</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> <p>계획에 대한 권한 보기 이상</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">시나리오 플래너의 계획에 대한 액세스 요청</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 정의 액세스 레벨을 사용하여 시나리오 플래너에 대한 사용자 액세스 구성

1. 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 오른쪽 옵션을 클릭합니다. **시나리오 플래너** 이 액세스 수준에 사용할 수 있습니다.

   >[!NOTE]
   >
   >요청 또는 외부 라이선스 유형에서는 시나리오 플래너에 대한 보기 또는 편집 액세스를 허용하지 않습니다.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 다음 문서에 나열된 문서 중 하나를 계속 사용합니다. [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), 예 [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 완료되면 를 클릭합니다 **저장**.

## 라이선스 유형별로 시나리오 플래너에 액세스

각 액세스 레벨의 사용자가 시나리오 계획자로 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [시나리오 플래너 영역](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 액세스 수준 설정별 시나리오 플래너 액세스

다음 정보는 액세스 수준 설정을 사용하여 Workfront 시나리오 플래너의 정보에 대한 사용자의 액세스를 제어하는 방법을 이해하는 데 도움이 될 수 있습니다.

* [액세스 권한 없음](#no-access)
* [액세스 권한 보기](#view-access)
* [액세스 편집](#edit-access)

### 액세스 권한 없음 {#no-access}

시나리오 플래너에 액세스할 수 없는 사용자는 레이아웃 템플리트에 추가될 때 기본 메뉴에서 시나리오 아이콘을 볼 수 없으며, 해당 사용자와 공유된 계획 및 이니셔티브를 볼 수 없습니다. 계획 링크가 시나리오 계획자에 액세스할 수 없는 사용자와 공유되는 경우 사용자는 계획을 보거나 편집할 수 없습니다.

### 액세스 권한 보기 {#view-access}

시나리오 계획자에 대한 보기 액세스 권한이 있는 사용자는 다음을 수행할 수 있습니다.

* 기본 메뉴에서 시나리오 아이콘을 참조하십시오 ![](assets/esp-icon-in-main-menu.png)하지만 사용자가 다른 사용자가 공유하는 계획 링크를 클릭하지 않으면 계획 영역이 비어 있습니다.
* 다른 사용자가 해당 링크를 공유할 때 계획을 확인합니다.

   여기에는 계획에 있는 모든 작업 역할 정보가 포함됩니다.

   또한, 수신자 사용자가 재무 데이터에도 액세스할 수 있는 경우 계획에 대한 작업 역할 비율 및 비용 정보가 포함됩니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### 액세스 편집 {#edit-access}

시나리오 플래너에 대한 편집 액세스 권한이 있는 사용자는 다음을 수행할 수 있습니다.

* 기본 메뉴에서 시나리오 아이콘을 참조하십시오 ![](assets/esp-icon-in-main-menu.png) 계획 데이터에 액세스하는 데 사용합니다.
* 계획을 만듭니다.
* 계획 생성, 편집 및 삭제
* 공유 링크를 사용하여 액세스하는 다른 사용자의 계획을 보고 편집하고 삭제합니다.

   여기에는 계획의 모든 작업 역할 정보가 포함됩니다.

   또한, 수신자 사용자가 재무 데이터에 액세스할 수 있는 경우 계획에 대한 작업 역할 비율 및 비용 정보가 포함됩니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
