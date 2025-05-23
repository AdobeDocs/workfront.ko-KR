---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 시스템 업데이트 구성
description: Workfront은 개체의 [!UICONTROL 업데이트] 영역에 자동 시스템 업데이트를 생성하여 사용자가 개체에서 수행하는 변경 내용을 기록합니다.  [!DNL Workfront] 관리자는 시스템 업데이트를 기록할 개체 필드 및 작업 [!DNL Workfront] 트랙을 구성할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 8%

---

# 시스템 업데이트 구성

[!DNL Adobe Workfront]은(는) 다음 이벤트를 기록하기 위해 개체의 [!UICONTROL 업데이트] 영역에서 자동 시스템 업데이트를 생성합니다.

* 사용자가 오브젝트 필드에서 변경한 사항
* 사용자가 객체에 대해 수행하는 작업

이러한 시스템 업데이트에는 다음 유형의 정보가 포함됩니다.

* 변경된 내용
* 변경한 사용자의 이름
* 변경 시간 및 날짜

시스템 업데이트에 대한 자세한 내용은 [시스템 추적 업데이트](../system-tracked-update-feeds/system-tracked-update-feeds.md)를 참조하십시오.

[!DNL Workfront] 관리자는 시스템 업데이트를 기록하기 위해 [!DNL Workfront]에서 추적하는 개체 필드와 작업을 구성할 수 있습니다.

예를 들어 [!DNL Workfront]에서 사용자가 시스템 전체에서 문제 이름에 적용한 모든 변경 내용을 추적할 수 있습니다. 문제 이름이 변경되면 해당 문제의 [!UICONTROL 업데이트] 영역에 시스템 업데이트로 나타납니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 개체 유형에 대해 [!DNL Workfront]에서 추적하는 필드 확인

사용자가 전체 [!DNL Workfront] 인터페이스에서 특정 개체 형식과 관련된 정보를 변경할 때 [!DNL Workfront]에서 추적하는 정보를 확인할 수 있습니다. [!DNL Workfront]에서 해당 개체 유형에 대해 추적할 필드를 추가하거나 제거하면 됩니다.

>[!NOTE]
>
>* [!DNL Workfront]이(가) 계산된 사용자 정의 필드에 대한 업데이트를 추적하고 기록할 수 없습니다.
>* 프로젝트, 작업, 문제, 포트폴리오, 프로그램 및 사용자에 대한 시스템 업데이트를 사용자 지정할 수 있습니다. 템플릿, 문서 또는 타임시트에 대한 시스템 업데이트를 사용자 지정할 수 없지만 [!DNL Workfront]은(는) 이러한 개체에 대한 시스템 업데이트를 기록합니다.
>



* [ [!DNL Workfront] 추적할 필드 추가](#add-fields-you-want-workfront-to-track)
* [추적하지 않을 필드 제거](#remove-fields-that-you-don-t-want-tracked)

### [!DNL Workfront]에서 추적할 필드 추가 {#add-fields-you-want-workfront-to-track}

[!DNL Workfront] 인터페이스 전체에서 특정 개체 유형에 대해 [!DNL Workfront]이(가) 추적할 필드를 추가할 수 있습니다. 사용자가 해당 필드의 정보를 변경하면 [!DNL Workfront]은(는) 해당 개체에 대한 [!UICONTROL 업데이트] 영역에 시스템 업데이트로 변경 내용을 기록합니다.

>[!NOTE]
>
>업데이트 피드에서 최대 300개의 기본 제공 및 사용자 지정 필드를 추적할 수 있습니다. 최대 필드 수를 추적하고 [!UICONTROL 모든 필드] 하위 탭에 표시되지 않는 추가 필드를 추적하려면 새 필드를 추적하려면 먼저 추적된 필드 일부를 제거해야 합니다. 업데이트 필드에서 필드를 제거하는 방법에 대한 자세한 내용은 [추적하지 않을 필드 제거](#remove-fields-that-you-don-t-want-tracked)를 참조하십시오.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. 왼쪽 패널에서 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**&#x200B;를 클릭합니다.

1. {&#x200B;0}필드 추가&#x200B;**를 클릭한 다음 추적할 개체를 클릭합니다.**

1. 표시되는 {&#x200B;0}피드 업데이트&#x200B;**상자에서 개체에 대한 기본 제공(표준) 필드 또는 사용자 지정 필드를 입력한 다음 목록에 표시될 때 클릭하여 선택합니다.**

   [!DNL Workfront]이(가) 이미 필드를 추적하는 경우 목록에서 두 번 추가할 수 없습니다.

1. [!DNL Workfront]에서 추적할 모든 필드를 추가한 후 **[!UICONTROL 필드 추가]**&#x200B;를 클릭합니다.

   추가한 기본 제공 필드는 **[!UICONTROL 기본 제공 필드]** 하위 탭 아래에 표시됩니다.

   추가한 사용자 정의 필드는 **[!UICONTROL 사용자 정의 필드]** 하위 탭 아래에 표시됩니다.

   **[!UICONTROL 모든 필드]** 하위 탭에는 추적 중인 기본 제공 필드와 사용자 지정 필드가 모두 표시됩니다.

### 추적하지 않을 필드 제거 {#remove-fields-that-you-don-t-want-tracked}

[!DNL Workfront] 인터페이스 전체에서 특정 개체 유형에 대해 시스템에서 추적하지 않으려는 필드를 제거할 수 있습니다.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 추적된 필드]** 탭에서 **[!UICONTROL 모든 필드]** 하위 탭을 선택합니다.

   이 보고서는 기본 제공 필드와 현재 추적 중인 사용자 정의 필드를 모두 표시합니다.

1. 추적을 중지할 필드를 선택한 다음 **[!UICONTROL 제거]**&#x200B;를 클릭합니다.

1. 표시되는 **[!UICONTROL 필드 제거]** 상자에서 **[!UICONTROL 예, 제거]**&#x200B;를 클릭하여 확인합니다.

이전에 추적한 필드에 대한 모든 업데이트는 해당 필드가 기록된 [!UICONTROL 업데이트] 영역에서 유지됩니다.

## 개체 유형에 대해 [!DNL Workfront]에서 추적하는 작업 확인

[!DNL Workfront]에서 사용자가 [!DNL Workfront] 인터페이스 전체에서 개체에 대해 수행할 수 있는 다음 작업을 추적할 수 있습니다.

예를 들어 [!DNL Workfront]에서 사용자가 작업 또는 문제로 할당을 변경할 때마다 업데이트를 기록할 수 있습니다. 그러면 작업 또는 문제에 대한 [!UICONTROL 업데이트] 영역에 변경 내용이 시스템 업데이트로 나타납니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>작업</strong> </th> 
   <th><strong>오브젝트</strong> </th> 
   <th><strong>기본 상태</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>할당이 변경됨</td> 
   <td>작업, 문제</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>기준선이 삭제됩니다.</td> 
   <td>프로젝트</td> 
   <td> <p>비활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>청구 기록이 생성 또는 삭제되었습니다.</td> 
   <td>프로젝트</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>문서가 생성 또는 삭제되었습니다.</td> 
   <td>프로젝트, 작업, 문제, 포트폴리오, 프로그램</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>비용이 생성 또는 삭제됨</td> 
   <td>프로젝트, 작업</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>시간이 기록되거나 삭제됨</td> 
   <td>프로젝트, 작업, 문제</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>문제가 삭제되었습니다.</td> 
   <td>프로젝트</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>작업이 삭제됨</td> 
   <td>프로젝트</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>누군가의 액세스가 변경됨</td> 
   <td>프로젝트, 작업, 문제, 문서, 포트폴리오, 프로그램</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
  <tr> 
   <td>주석 오브젝트 구독</td> 
   <td>프로젝트, 작업, 문제</td> 
   <td> <p>활성화됨</p> </td> 
  </tr> 
 </tbody> 
</table>

[!DNL Workfront]이(가) 추적할 작업을 구성하려면 다음을 수행하십시오.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 작업]** 탭을 클릭합니다.

1. 활성화할 액션을 선택하거나 비활성화할 액션을 선택 취소합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

작업을 사용하지 않도록 설정하면 해당 작업에 대해 이전에 기록된 모든 업데이트가 기록된 [!UICONTROL 업데이트] 영역에 유지됩니다.
