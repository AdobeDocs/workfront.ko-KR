---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 이니셔티브 우선순위 업데이트
description: 이니셔티브 우선 순위는 이니셔티브가 계획에 나열된 순서로 계획에서 직무 역할과 예산 자원을 받기 때문에 중요합니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 에서 이니셔티브 우선 순위 업데이트 [!DNL Scenario Planner]

이니셔티브 우선 순위는 이니셔티브가 계획에 나열된 순서로 계획에서 직무 역할과 예산 자원을 받기 때문에 중요합니다.

생성된 계획이나 누군가 사용자와 공유한 계획에 따라 이니셔티브의 우선순위를 정할 수 있습니다.

계획 생성에 대한 자세한 내용은 [에서 계획 생성 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

이니셔티브 만들기에 대한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다.</p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]</a>. </p> </td> 
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

## 이니셔티브 우선 순위 업데이트

이니셔티브 우선순위를 변경할 때 계획에서 목록 순서를 수정합니다.

계획의 맨 위에 더 긴급한 이니셔티브를 배치하고, 더 유동적인 이니셔티브, 즉 언제, 그리고 리소스를 이용할 수 있는 경우에만 할 수 있는 더 많은 계획을 계획 맨 아래에 배치하는 것을 권장합니다.

>[!NOTE]
>
>[!DNL Workfront] 계획 자원을 계획에 나열된 순서로 이니셔티브에 할당합니다.
>
>예를 들어, 이 계획에 3명의 가용 엔지니어 및 이니셔티브 1과 이니셔티브 2가 각각 2명의 엔지니어가 완료되어야 하고 두 엔지니어가 모두 동일한 기간 동안 예약된 경우, Workfront은 2명의 엔지니어를 Initiative 1과 연결하며 Initiative 2의 남은 엔지니어 1명을 연결합니다. 이 경우 Initiative 2는 하나의 엔지니어가 없으므로 충돌이 있는 것으로 표시됩니다. 경우에 따라, 여러분의 이니셔티브의 우선순위를 변경하는 것이 계획에서의 충돌을 피할 수 있는 유일한 방법입니다.

이니셔티브 우선순위를 갱신하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

   계획 목록이 표시됩니다.

1. 계획 이름을 클릭하여 연 다음 우선 순위를 지정할 이니셔티브를 찾습니다.
1. 하나 이상의 이니셔티브 이름 왼쪽에 있는 상자를 클릭하고 다음 중 하나를 수행합니다.

   * 선택한 이니셔티브 이름 중 왼쪽에 있는 핸들을 클릭한 다음 목록에서 위 또는 아래로 끌어 이니셔티브의 우선순위를 변경합니다.

      Workfront에 선택한 이니셔티브 수가 표시됩니다.

      ![](assets/multi-select-initiative-number.png)

   * 을(를) 클릭합니다. **[!UICONTROL 우선 순위 지정]** 계획 하단의 상자를 선택한 다음 다음 옵션 중에서 선택합니다.

      * **[!UICONTROL 상단]**: 선택한 이니셔티브를 이니셔티브 목록의 맨 위로 이동합니다. 선택한 이니셔티브가 계획에 먼저 나열됩니다.
      * **[!UICONTROL 아래쪽]**: 선택한 이니셔티브를 이니셔티브 목록의 맨 아래로 이동합니다. 선택한 이니셔티브가 계획에 마지막으로 나열됩니다.
      * **[!UICONTROL 숫자 선택]**: 여기에서 표시하는 이니셔티브 뒤에 선택한 이니셔티브를 이동합니다.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] 선택한 이니셔티브를 지정한 위치에 즉시 배치하고 모든 이니셔티브 수를 그에 따라 업데이트합니다.


1. 클릭 **[!UICONTROL 계획 저장]** 변경 사항을 저장하려면 을 클릭합니다.
