---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 기본 문제 유형 사용자 지정
description: 조직에서 사용하는 용어와 더 잘 일치하도록 각 기본 문제 유형의 레이블을 사용자 지정할 수 있습니다. 문제 유형은 문제 상태를 사용자 정의하고 요청 대기열을 만드는 데 유용합니다.
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

문제 유형은 다음과 같은 경우에 유용합니다.

* [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)에 설명된 대로 문제 상태를 사용자 지정할 때.
* [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)에 설명된 대로 요청 큐를 만들 때.

조직에서 사용하는 용어와 더 잘 일치하도록 각 기본 문제 유형의 레이블을 사용자 지정할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 문제 유형

[!DNL Adobe Workfront] [!UICONTROL 관리자] 액세스 권한이 있는 경우 구성하고 이름을 바꿀 수 있는 4가지 기본 문제 유형이 있습니다.

* **[!UICONTROL 버그 보고서]** 시스템에서 보고된 버그를 추적하는 데 사용됩니다.
* **[!UICONTROL 순서 변경]** 업데이트 또는 수정이 필요한 문제를 추적하는 데 사용됩니다.
* **[!UICONTROL 문제]** [!DNL Workfront]의 개체로, 예기치 않은 작업, 발생한 문제 또는 작업을 계속하려면 해결해야 하는 문제를 전달합니다.
* **[!UICONTROL 요청]** 사용자가 Workfront에서 요청하는 요청 대기열에 적용되는 문제 유형입니다.

![](assets/default-issue-types.png)

## 문제 유형 사용자 정의

문제 유형 사용자 지정에 대한 다음 사항을 고려하십시오.

* 문제 유형에 대한 레이블을 수정할 수 있지만, 해당 기능은 변경할 수 없습니다.
* 추가 문제 유형을 만들 수 없습니다.
* 문제 유형 이름에 대한 필터 값을 변경할 수 없습니다. 따라서 문제 보고서에 필터를 만드는 경우 필터(키)의 값이 문제 유형의 사용자 정의 이름을 반영하지 않습니다.
* 세 가지 기본 상태가 각 문제 유형과 연결되어 있습니다. [!UICONTROL 새로 만들기], [!UICONTROL 진행 중], [!UICONTROL 닫힘]. 이러한 상태를 삭제하거나 문제 유형에서 제거할 수는 없지만 이름을 바꿀 수는 있습니다.
* 각 문제 유형에 대해 드롭다운 메뉴에 표시되는 옵션의 순서를 변경할 수 있습니다.

문제 유형을 사용자 정의하려면 다음을 수행하십시오.

1. [!DNL Adobe Workfront]의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 상태]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 문제]** 탭을 클릭합니다.
1. 다음 중 하나를 수행합니다.

   * 사용자 지정할 문제 유형 위로 마우스를 가져간 후 맨 오른쪽에 나타나는 [!UICONTROL 편집] 아이콘 ![](assets/edit-icon.png)을(를) 클릭한 다음 문제 유형의 새 이름을 입력하십시오.

     ![](assets/customize-issue-type.png)

   * [!UICONTROL 문제 유형]을(를) 클릭하여 연결된 상태를 나열한 다음 마우스로 가리키면 표시되는 핸들을 드래그하여 사용자의 문제 **[!UICONTROL 상태]** 드롭다운 메뉴에 표시할 순서대로 놓습니다.
