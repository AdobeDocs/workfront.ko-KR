---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 시스템 업데이트 구성
description: Workfront은 개체의 자동 시스템 업데이트를 생성합니다 [!UICONTROL 업데이트] 영역에 사용자가 객체에 대해 수행하는 변경 사항을 기록합니다. 로서의 [!DNL Workfront] 관리자는 어떤 객체 필드와 작업을 구성할 수 있습니다 [!DNL Workfront] 시스템 업데이트를 기록하도록 추적합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# 시스템 업데이트 구성

[!DNL Adobe Workfront] 개체의 자동 시스템 업데이트 생성 [!UICONTROL 업데이트] 영역에 다음 이벤트를 기록합니다.

* 사용자가 개체 필드에서 수행하는 변경 사항
* 사용자가 개체에 대해 수행하는 작업

이러한 시스템 업데이트에는 변경된 내용, 변경한 사용자의 이름, 변경 시간 및 날짜가 포함됩니다.

로서의 [!DNL Workfront] 관리자는 어떤 객체 필드와 작업을 구성할 수 있습니다 [!DNL Workfront] 시스템 업데이트를 기록하도록 추적합니다.

예를 들어 [!DNL Workfront] 사용자가 시스템 전체에서 문제 이름에 대한 모든 변경 사항을 추적합니다. 그러면 문제 이름 변경이 문제 [!UICONTROL 업데이트] 영역.

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

## 어떤 필드를 결정합니다 [!DNL Workfront] 개체 유형에 대한 추적

어떤 정보를 알 수 있습니다 [!DNL Workfront] 사용자가 전체 페이지에서 특정 개체 유형과 관련된 정보를 변경하면 추적합니다 [!DNL Workfront] 인터페이스. 원하는 필드를 추가하거나 제거하여 수행합니다 [!DNL Workfront] 를 눌러 해당 객체 유형을 추적합니다.

>[!NOTE]
>
>* [!DNL Workfront] 계산된 사용자 지정 필드에 대한 업데이트를 추적하고 기록할 수 없습니다.
>* 프로젝트, 작업, 문제, 포트폴리오, 프로그램 및 사용자에 대한 시스템 업데이트를 사용자 정의할 수 있습니다. 템플릿, 문서 또는 작업표에 대한 시스템 업데이트를 사용자 지정할 수는 없지만 [!DNL Workfront] 는 이러한 객체에 대한 시스템 업데이트를 기록합니다.
>




* [원하는 필드 추가 [!DNL Workfront] 추적하려면](#add-fields-you-want-workfront-to-track)
* [추적하지 않을 필드 제거](#remove-fields-that-you-don-t-want-tracked)

### 원하는 필드 추가 [!DNL Workfront] 추적하려면 {#add-fields-you-want-workfront-to-track}

원하는 필드를 추가할 수 있습니다 [!DNL Workfront] 를 통해 특정 유형의 객체를 추적하려면 [!DNL Workfront] 인터페이스. 사용자가 해당 필드의 정보를 변경하면 [!DNL Workfront] 변경 내용은 [!UICONTROL 업데이트] 영역의 매개 변수입니다.

>[!NOTE]
>
>업데이트 피드에서 최대 300개의 기본 제공 및 사용자 지정 필드를 추적할 수 있습니다. 최대 필드 수를 추적하고 에 표시되지 않는 추가 필드를 추적하려는 경우 [!UICONTROL 모든 필드] 하위 탭에서 새 필드를 추적하려면 먼저 추적된 필드 일부를 제거해야 합니다. 업데이트 필드에서 필드를 제거하는 방법에 대한 자세한 내용은 [추적하지 않을 필드 제거](#remove-fields-that-you-don-t-want-tracked).

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽의 패널에서 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.

1. &#x200B; 클릭 **[!UICONTROL 필드 추가]**&#x200B;을 클릭한 다음 추적할 개체를 클릭합니다.

1. 에서 **[!UICONTROL 피드 업데이트]** 상자가 표시되면 개체의 기본 제공(표준) 필드나 사용자 정의 필드를 입력한 다음 목록에 표시될 때 클릭하여 선택합니다.

   If [!DNL Workfront] 가 이미 필드를 추적하고 있으므로 목록에서 두 번째로 추가할 수 없습니다.

1. 원하는 필드를 모두 추가한 후 [!DNL Workfront] 추적하려면 **[!UICONTROL 필드 추가]**.

   추가한 기본 제공 필드는 **[!UICONTROL 기본 제공 필드]** 하위 탭.

   추가한 사용자 정의 필드는 **[!UICONTROL 사용자 지정 필드]** 하위 탭.

   다음 **[!UICONTROL 모든 필드]** 하위 탭에는 기본 제공 및 추적 중인 사용자 지정 필드가 모두 표시됩니다.

### 추적하지 않을 필드 제거 {#remove-fields-that-you-don-t-want-tracked}

시스템에서 특정 유형의 객체에 대해 추적하지 않으려는 필드를 [!DNL Workfront] 인터페이스.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.

1. 설정 **[!UICONTROL 추적된 필드]** 탭에서 을 선택합니다 **[!UICONTROL 모든 필드]** 하위 탭.

   여기에는 현재 추적 중인 기본 제공 및 사용자 지정 필드가 모두 표시됩니다.

1. 추적을 중지할 필드를 선택한 다음 **[!UICONTROL 제거]**.

1. 에서 **[!UICONTROL 필드 제거]** 표시되는 상자를 클릭합니다. **[!UICONTROL 예, 제거합니다.]** 확인합니다.

이전에 추적한 필드에 대한 모든 업데이트는 [!UICONTROL 업데이트] 그들이 기록된 지역.

## 어떤 작업을 결정합니다 [!DNL Workfront] 개체 유형에 대한 추적

다음을 수행할 수 있습니다 [!DNL Workfront] 사용자가 전체 개체에서 수행할 수 있는 다음 작업을 추적합니다 [!DNL Workfront] 인터페이스.

예를 들어 다음과 같은 [!DNL Workfront] 사용자가 작업 또는 문제에 대한 할당을 변경할 때마다 업데이트를 기록합니다. 그러면 변경 사항이 [!UICONTROL 업데이트] 작업 또는 문제에 대한 영역입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>개 액션</strong> </th> 
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
   <td> <p>비활성화</p> </td> 
  </tr> 
  <tr> 
   <td>청구 레코드가 생성되거나 삭제됩니다</td> 
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

원하는 작업을 구성하려면 [!DNL Workfront] 추적하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.

1. 을(를) 클릭합니다. **[!UICONTROL 작업]** 탭.

1. 활성화할 작업을 선택하거나 작업을 선택 취소하여 비활성화합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

작업을 비활성화하면 해당 작업에 대해 이전에 기록된 모든 업데이트가 [!UICONTROL 업데이트] 기록된 지역.
