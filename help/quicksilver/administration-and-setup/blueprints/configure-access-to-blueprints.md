---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트에 대한 액세스 구성
description: 시스템 관리자는 요청을 저장할 요청 대기열을 설정하여 사용자가 블루프린트 설치를 요청할 수 있도록 액세스 권한을 활성화할 수 있습니다. 여기에서 요청을 추적하고 업데이트할 수 있는 단일 위치가 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 블루프린트에 대한 액세스 구성

모든 [!DNL Adobe Workfront]명의 사용자가 블루프린트 카탈로그를 검색할 수 있습니다.

시스템 관리자는 다음 작업을 수행할 수 있습니다.

* 레이아웃 템플릿의 기본 메뉴에 [!UICONTROL 블루프린트]를 추가하고 사용자 또는 그룹에 레이아웃 템플릿을 할당하십시오. 자세한 내용은 [레이아웃 템플릿을 사용하여 [!UICONTROL 주 메뉴 사용자 지정] 및 ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)레이아웃 템플릿에 사용자 할당[을 참조하십시오.](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

  >[!NOTE]
  >
  >* 레이아웃 템플릿이 할당되지 않은 사용자에게는 [!UICONTROL 기본 메뉴]에 [!UICONTROL 블루프린트] 아이콘이 표시됩니다.
  >* 새 레이아웃 템플릿을 만들 때 기본적으로 [!UICONTROL 기본 메뉴]에 대한 [!UICONTROL 활성 항목] 목록에 [!UICONTROL 블루프린트] 아이콘이 포함됩니다.


* 요청을 저장할 요청 대기열을 설정하여 사용자가 블루프린트 설치를 요청할 수 있도록 액세스 권한을 활성화합니다. 여기에서 요청을 추적하고 업데이트할 수 있는 단일 위치가 있습니다. 자세한 내용은 아래 절차를 따르십시오.
* 블루프린트를 설치합니다. 자세한 내용은 [블루프린트 설치](../../administration-and-setup/blueprints/blueprints-install.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>Workfront 관리자 </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건 {#prerequisites}

* 블루프린트 요청을 저장하려면 기존 요청 대기열을 사용해야 합니다. 프로젝트는 요청 대기열로 저장해야 하며 [!UICONTROL 현재] 상태여야 합니다.
* 요청 대기열은 공개 상태여야 합니다. 요청 대기열 세부 정보에서 &quot;[!UICONTROL 이 대기열에 요청을 추가할 수 있는 사용자는 누구입니까?]&quot;은(는) **[!UICONTROL 모든 사용자]**(으)로 설정해야 합니다.

>[!TIP]
>
>블루프린트 요청에 대한 새 요청 대기열을 만들려면 블루프린트 액세스를 구성하기 전에 새로 만들어야 합니다. 요청 대기열을 만드는 방법에 대한 자세한 내용은 [요청 대기열 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.

## 블루프린트 요청을 저장할 요청 대기열 선택

사용자가 블루프린트 설치를 요청하려면 먼저 해당 요청에 대한 요청 대기열을 선택해야 합니다. 요청 대기열이 정의될 때까지 사용자는 블루프린트 카탈로그만 검색할 수 있습니다.

{{step1-to-blueprints}}

1. 카탈로그 화면의 오른쪽 상단에서 **[!UICONTROL 블루프린트 요청 구성]**&#x200B;을 클릭합니다.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. **[!UICONTROL 블루프린트 구성]** 대화 상자에서 활성 요청 대기열의 이름을 입력한 다음 검색 결과에 나타나면 선택하십시오.

   >[!IMPORTANT]
   >
   >공개 요청 대기열만 이 목록에 표시됩니다. 요청 대기열을 공개하려면 위의 [필수 구성 요소](#prerequisites) 섹션을 참조하십시오.

   요청 대기열 기본 설정이 지정되었으며 사용자는 이제 블루프린트 설치를 요청할 수 있습니다.

   ![요청 큐 구성](assets/Blueprints_access_setup_request_queue.png)

1. (선택 사항) 실제 요청 대기열을 변경하려면 **[!UICONTROL 이 요청 대기열 편집]**&#x200B;을 클릭합니다.

   요청 대기열 프로젝트는 새 브라우저 탭에서 열리며 필요에 따라 업데이트할 수 있습니다.

1. (선택 사항) 요청 대기열에 주제 그룹 또는 대기열 주제가 포함되어 있는 경우 목록에서 해당 항목을 선택할 수 있습니다.
1. 블루프린트 카탈로그로 돌아가려면 **[!UICONTROL 닫기]**&#x200B;를 클릭하십시오.

>[!NOTE]
>
>요청된 블루프린트를 설치할 때 요청자가 알림을 받을 수 있도록 문제 상태를 요청 큐에서 **[!UICONTROL 닫힘]** 또는 **[!UICONTROL 해결됨]**(으)로 변경해야 합니다. 블루프린트 설치에 대한 자세한 내용은 [블루프린트 설치](../../administration-and-setup/blueprints/blueprints-install.md)를 참조하십시오.
