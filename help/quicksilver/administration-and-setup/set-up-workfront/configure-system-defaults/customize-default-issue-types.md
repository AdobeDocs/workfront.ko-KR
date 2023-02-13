---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 기본 문제 유형 사용자 지정
description: 조직에서 사용하는 용어와 더 잘 일치하도록 각 기본 문제 유형에 대한 레이블을 사용자 지정할 수 있습니다. 문제 유형은 문제 상태를 사용자 지정하고 요청 큐를 만드는 데 유용합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 기본 문제 유형 사용자 지정

문제 유형은 다음 상황에서 유용합니다.

* 에 설명된 대로 문제 상태를 사용자 지정할 때 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* 에 설명된 대로 요청 큐를 만들 때 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

조직에서 사용하는 용어와 더 잘 일치하도록 각 기본 문제 유형에 대한 레이블을 사용자 지정할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 문제 유형

만약 [!DNL Adobe Workfront] [!UICONTROL 관리자] access에는 다음과 같이 구성하고 이름을 바꿀 수 있는 네 가지 기본 문제 유형이 있습니다.

* **[!UICONTROL 버그 보고서]** 시스템에서 보고된 버그를 추적하는 데 사용됩니다.
* **[!UICONTROL 순서 변경]** 업데이트하거나 수정해야 하는 문제를 추적하는 데 사용됩니다.
* **[!UICONTROL 문제]** 의 개체 [!DNL Workfront] 예상치 못한 작업, 발생되는 문제 또는 작업을 계속 진행하기 위해 해결해야 하는 문제를 전달하는 것입니다.
* **[!UICONTROL 요청]** 사용자가 Workfront에서 요청을 하는 요청 큐에 적용되는 문제 유형입니다.

![](assets/default-issue-types.png)

## 문제 유형 사용자 지정

문제 유형 사용자 지정에 대해서는 다음 사항을 고려하십시오.

* 문제 유형에 대한 레이블을 수정할 수 있지만 해당 함수를 변경할 수 없습니다.
* 추가 문제 유형을 만들 수 없습니다.
* 문제 유형의 이름은 필터 값을 변경할 수 없습니다. 따라서 문제 보고서에 필터를 만드는 경우 필터(키)의 값이 문제 유형의 사용자 지정 이름을 반영하지 않습니다.
* 다음 세 가지 기본 상태가 각 문제 유형과 연결됩니다. [!UICONTROL 새로 만들기], [!UICONTROL 진행 중], 및 [!UICONTROL 닫힘]. 이러한 상태를 삭제하거나 문제 유형에서 제거할 수 없지만 이름을 바꿀 수 있습니다.
* 각 문제 유형에 대한 드롭다운 메뉴에 나타나는 옵션을 다시 정렬할 수 있습니다.

문제 유형을 사용자 지정하는 방법은 다음과 같습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 상태]**.

1. 을(를) 클릭합니다. **[!UICONTROL 문제]** 탭.
1. 다음 중 하나를 수행합니다.

   * 사용자 지정할 문제 유형을 마우스로 가리킨 다음 [!UICONTROL 편집] 아이콘 ![](assets/edit-icon.png) 맨 오른쪽에 표시되는 문제 유형에 새 이름을 입력합니다.

      ![](assets/customize-issue-type.png)

   * 클릭 [!UICONTROL 문제 유형] 연결된 상태를 나열하려면 마우스를 위에 놓을 때 나타나는 핸들을 끌어서 사용자 문제에 표시할 순서대로 놓습니다 **[!UICONTROL 상태]** 드롭다운 메뉴
