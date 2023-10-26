---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 시스템 업데이트 구성
description: Workfront은 오브젝트의 [!UICONTROL 업데이트] 사용자가 개체에서 수행하는 변경 사항을 기록하는 영역입니다. 로서의 [!DNL Workfront] 관리자는 어떤 객체 필드와 작업을 구성할 수 있습니다 [!DNL Workfront] 시스템 업데이트를 기록합니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 7%

---

# 시스템 업데이트 구성

[!DNL Adobe Workfront] 는 개체의 자동 시스템 업데이트를 생성합니다. [!UICONTROL 업데이트] 다음 이벤트를 기록할 영역:

* 사용자가 오브젝트 필드에서 변경한 사항
* 사용자가 객체에 대해 수행하는 작업

이러한 시스템 업데이트에는 다음 유형의 정보가 포함됩니다.

* 변경된 내용
* 변경한 사용자의 이름
* 변경 시간 및 날짜

시스템 업데이트에 대한 자세한 내용은 [시스템 추적 업데이트](../system-tracked-update-feeds/system-tracked-update-feeds.md).

로서의 [!DNL Workfront] 관리자는 어떤 객체 필드와 작업을 구성할 수 있습니다 [!DNL Workfront] 시스템 업데이트를 기록합니다.

예를 들어 다음과 같은 작업을 수행할 수 있습니다 [!DNL Workfront] 사용자가 시스템 전체에서 문제 이름에 적용한 모든 변경 사항을 추적합니다. 문제 이름 변경 사항이 문제의 시스템 업데이트로 표시됩니다. [!UICONTROL 업데이트] 영역입니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음이어야 합니다: [!DNL Workfront] 관리자.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 필드 확인 [!DNL Workfront] 오브젝트 유형 추적

정보를 확인할 수 있습니다 [!DNL Workfront] 사용자가 전체에서 특정 오브젝트 유형과 연관된 정보를 변경하면 추적합니다 [!DNL Workfront] 인터페이스. 원하는 필드를 추가하거나 제거하면 됩니다 [!DNL Workfront] 를 입력하여 해당 객체 유형을 추적할 수 있습니다.

>[!NOTE]
>
>* [!DNL Workfront] 계산된 사용자 정의 필드에 대한 업데이트를 추적하고 기록할 수 없습니다.
>* 프로젝트, 작업, 문제, 포트폴리오, 프로그램 및 사용자에 대한 시스템 업데이트를 사용자 지정할 수 있습니다. 템플릿, 문서 또는 타임시트에 대한 시스템 업데이트를 사용자 지정할 수 없지만 [!DNL Workfront] 는 이러한 객체에 대한 시스템 업데이트를 기록합니다.
>



* [원하는 필드 추가 [!DNL Workfront] 추적하기](#add-fields-you-want-workfront-to-track)
* [추적하지 않을 필드 제거](#remove-fields-that-you-don-t-want-tracked)

### 원하는 필드 추가 [!DNL Workfront] 추적하기 {#add-fields-you-want-workfront-to-track}

원하는 필드를 추가할 수 있습니다. [!DNL Workfront] 를 사용하여 전체에서 특정 유형의 객체를 추적합니다. [!DNL Workfront] 인터페이스. 사용자가 해당 필드의 정보를 변경할 때 [!DNL Workfront] 변경 내용에 대한 정보를 시스템 업데이트로 [!UICONTROL 업데이트] 객체의 영역입니다.

>[!NOTE]
>
>업데이트 피드에서 최대 300개의 기본 제공 및 사용자 지정 필드를 추적할 수 있습니다. 최대 필드 수를 추적하고 에서에 표시되지 않는 추가 필드를 추적하려는 경우 [!UICONTROL 모든 필드] 하위 탭에서는 새 필드를 추적하려면 먼저 추적된 필드 일부를 제거해야 합니다. 업데이트 필드에서 필드를 제거하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [추적하지 않을 필드 제거](#remove-fields-that-you-don-t-want-tracked).

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽의 패널에서 을 클릭합니다. **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.

1. &#x200B; 클릭 **[!UICONTROL 필드 추가]**&#x200B;를 클릭한 다음 추적할 개체를 클릭합니다.

1. 다음에서&#x200B;: **[!UICONTROL 피드 업데이트]** 표시되는 상자에서 객체에 대한 기본 제공(표준) 필드 또는 사용자 정의 필드를 입력한 다음, 목록에 표시될 때 클릭하여 선택합니다.

   If [!DNL Workfront] 은(는) 이미 필드를 추적하고 있으므로 목록에서 해당 필드를 두 번 추가할 수 없습니다.

1. 원하는 필드를 모두 추가한 후 [!DNL Workfront] 추적하려면 **[!UICONTROL 필드 추가]**.

   추가한 기본 제공 필드는 **[!UICONTROL 기본 제공 필드]** 하위 탭.

   추가한 사용자 정의 필드는 **[!UICONTROL 사용자 정의 필드]** 하위 탭.

   다음 **[!UICONTROL 모든 필드]** 하위 탭에는 추적 중인 기본 제공 필드와 사용자 지정 필드가 모두 표시됩니다.

### 추적하지 않을 필드 제거 {#remove-fields-that-you-don-t-want-tracked}

에서 특정 유형의 객체에 대해 시스템에서 추적하지 않으려는 필드를 제거할 수 있습니다. [!DNL Workfront] 인터페이스.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.

1. 다음에서 **[!UICONTROL 추적된 필드]** 탭에서 **[!UICONTROL 모든 필드]** 하위 탭.

   이 보고서는 기본 제공 필드와 현재 추적 중인 사용자 정의 필드를 모두 표시합니다.

1. 추적을 중지할 필드를 선택한 다음 **[!UICONTROL 제거]**.

1. 다음에서 **[!UICONTROL 필드 제거]** 나타나는 상자에서 **[!UICONTROL 예, 제거합니다.]** 확인할 수 있습니다.

이전에 추적한 필드에 대한 모든 업데이트는에서 유지됩니다. [!UICONTROL 업데이트] 기록된 영역입니다.

## 작업 결정 [!DNL Workfront] 오브젝트 유형 추적

다음을 수행할 수 있습니다. [!DNL Workfront] 에서 사용자가 개체에 대해 수행할 수 있는 다음 작업을 추적합니다. [!DNL Workfront] 인터페이스.

예를 들어 다음과 같은 작업을 수행할 수 있습니다 [!DNL Workfront] 사용자가 작업 또는 문제에 대한 할당을 변경할 때마다 업데이트를 기록합니다. 그런 다음 변경 사항이 [!UICONTROL 업데이트] 작업 또는 문제에 대한 영역입니다.

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

원하는 작업을 구성하려면 [!DNL Workfront] 추적하려면:

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.

1. 다음을 클릭합니다. **[!UICONTROL 작업]** 탭.

1. 활성화할 액션을 선택하거나 비활성화할 액션을 선택 취소합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

작업을 비활성화하면 해당 작업에 대해 이전에 기록된 모든 업데이트가 [!UICONTROL 업데이트] 기록된 영역입니다.
