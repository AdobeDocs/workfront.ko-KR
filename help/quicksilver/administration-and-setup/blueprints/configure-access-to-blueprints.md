---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트에 대한 액세스 구성
description: 시스템 관리자는 요청을 저장하기 위한 요청 큐를 설정하여 사용자가 블루프린트 설치를 요청할 수 있는 액세스 권한을 활성화할 수 있습니다. 여기에서 요청을 추적하고 업데이트할 단일 위치가 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 블루프린트에 대한 액세스 구성

모두 [!DNL Adobe Workfront] 사용자는 청사진 카탈로그를 찾아볼 수 있습니다.

시스템 관리자는 다음을 수행할 수 있습니다.

* 추가 [!UICONTROL 블루프린트] 레이아웃 템플릿의 기본 메뉴에 레이아웃 템플릿을 지정하고 사용자 또는 그룹에 레이아웃 템플릿을 할당합니다. 자세한 내용은 [사용자 지정 [!UICONTROL 기본 메뉴] 레이아웃 템플릿 사용](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) 및 [레이아웃 템플릿에 사용자 할당](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* 레이아웃 템플릿이 할당되지 않은 사용자에게는 [!UICONTROL 블루프린트] 아이콘( [!UICONTROL 기본 메뉴].
   >* 새 레이아웃 템플릿을 만들면 [!UICONTROL 블루프린트] 아이콘이 [!UICONTROL 활성 항목] 목록 [!UICONTROL 기본 메뉴] 기본적으로 제공됩니다.



* 사용자가 요청을 저장하기 위해 요청 큐를 설정하여 블루프린트 설치를 요청할 수 있도록 액세스를 활성화합니다. 여기에서 요청을 추적하고 업데이트할 단일 위치가 있습니다. 자세한 내용은 아래 절차를 따르십시오.
* 블루프린트를 설치합니다. 자세한 내용은 [블루프린트 설치](../../administration-and-setup/blueprints/blueprints-install.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p> 모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건 {#prerequisites}

* 블루프린트 요청을 저장하려면 기존 요청 큐를 사용해야 합니다. 프로젝트를 요청 큐로 저장해야 하며 다음 위치에 있어야 합니다. [!UICONTROL 현재] 상태.
* 요청 큐는 공개여야 합니다. 요청 큐 세부 정보에서 &quot;[!UICONTROL 누가 이 큐에 요청을 추가할 수 있습니까?]&quot; 을(를) 로 설정해야 합니다. **[!UICONTROL 누구든]**.

>[!TIP]
>
>블루프린트 요청에 대한 새 요청 큐를 만들려면 Blueprint 액세스를 구성하기 전에 먼저 구성해야 합니다. 요청 큐 만들기에 대한 내용은 [요청 큐 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 블루프린트 요청을 저장할 요청 큐를 선택합니다

사용자가 Blueprint를 설치하도록 요청하려면 먼저 해당 요청에 대한 요청 큐를 선택해야 합니다. 요청 큐가 정의될 때까지 사용자는 블루프린트 카탈로그만 검색할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 블루프린트]**.
1. 클릭 **[!UICONTROL 블루프린트 요청 구성]** 카탈로그 화면의 오른쪽 위에 표시됩니다.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. 설정 **[!UICONTROL 블루프린트 구성]** 대화 상자에서 활성 요청 큐의 이름을 입력하고 검색 결과에 이 대기열이 나타나면 선택합니다.

   >[!IMPORTANT]
   >
   >이 목록에는 공개 요청 큐만 표시됩니다. 요청 큐를 공개하려면 [전제 조건](#prerequisites) 섹션에 있는 마지막 항목이 될 필요가 없습니다.

   요청 큐 기본 설정이 설정되고 사용자는 이제 블루프린트 설치를 요청할 수 있습니다.

   ![요청 큐 구성](assets/Blueprints_access_setup_request_queue.png)

1. (선택 사항) 실제 요청 큐를 변경하려면 **[!UICONTROL 이 요청 큐 편집]**.

   요청 큐 프로젝트가 새 브라우저 탭에서 열리고, 필요에 따라 업데이트할 수 있습니다.

1. (선택 사항) 요청 큐에 주제 그룹이나 큐 주제가 포함되어 있으면 목록에서 선택할 수 있습니다.
1. 블루프린트 카탈로그로 돌아가려면 **[!UICONTROL 닫기]**.

>[!NOTE]
>
>요청된 블루프린트를 설치할 때 문제 상태를 로 변경해야 합니다 **[!UICONTROL 닫힘]** 또는 **[!UICONTROL 해결됨]** 요청 큐에서 요청자에게 알림하도록 요청자에게 알립니다. 블루프린트 설치에 대한 자세한 내용은 [블루프린트 설치](../../administration-and-setup/blueprints/blueprints-install.md).
