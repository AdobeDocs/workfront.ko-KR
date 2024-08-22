---
title: ' [!DNL Workfront] 및 [!DNL Frame.io] 통합 구성'
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: ' [!DNL Adobe Workfront] 관리자로서  [!DNL Workfront] 과(와)  [!DNL Frame.io] 을(를) 통합하고 조직에 자산을 검토하고 승인할 수 있는 원활한 방법을 제공할 수 있습니다.'
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# [!DNL Workfront] 및 [!DNL Frame.io] 통합 구성

Workfront 관리자는 설정 영역에서 기본 Frame.io 계정을 구성한 다음 Workfront에서 Frame.io 사용자를 지정하여 Workfront과 Frame.io 간을 통합할 수 있습니다. 이를 통해 프로젝트 코디네이터는 Workfront 프로젝트를 사용하여 작업을 계획하고 시작하고, 워크플로를 검토 및 승인할 수 있습니다.


## 액세스 요구 사항

>[!IMPORTANT]
>
>이 기능은 [!DNL Adobe Admin Console]에 온보딩된 조직에서만 사용할 수 있습니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table>
  <tr>
   <td>[!DNL Adobe Workfront] 플랜</td>
   <td>임의</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] 라이선스
   </td>
   <td><p>현재: [!UICONTROL Plan]</p>
   <p>새로운 기능: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>액세스 수준 구성
   </td>
   <td>[!DNL Workfront] 관리자여야 합니다.
   </td>
  </tr>

</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기본 [!DNL Frame.io] 계정 구성 [!BADGE 준비 중]{type=Informative}

기본 [!DNL Frame.io] 계정이 설정되면 [!DNL Workfront]에서 만든 모든 프로젝트에 Frame.io에서 만든 미러 프로젝트가 있습니다.

>[!IMPORTANT]
>
>이 기능은 곧 제공될 예정입니다. 현재 Frame.io 계정은 Workfront 팀에서 수동으로 추가합니다. 도움이 필요하면 Adobe 계정 담당자에게 문의하십시오.

## Workfront 그룹으로 단일 Frame.io 계정 구성

단일 Workfront 그룹을 기본 계정과 다른 단일 Frame.io 계정과 연결할 수 있습니다.

Workfront 그룹으로 단일 Frame.io 계정을 구성하려면 다음 작업을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭합니다.
1. 기존 그룹을 선택하거나 **그룹 만들기**&#x200B;를 클릭하세요.
1. 왼쪽 패널에서 **Frame.io에 연결**&#x200B;을 클릭합니다.
1. API 개발자 토큰을 입력합니다.
1. **연결 시작**&#x200B;을 클릭합니다.
1. (조건부) 둘 이상의 Frame.io 계정의 관리자인 경우 사용할 계정을 선택합니다.

## Frame.io 사용자 활성화

Frame.io를 정기적으로 사용하는 Workfront 사용자는 Frame.io 사용자로 표시되어야 합니다. Workfront 관리자는 Workfront 사용자 프로필에서 Frame.io 사용자를 지정할 수 있습니다.

>[!TIP]
>
>크리에이티브 도구에서 정기적으로 작업하고 검토 및 승인을 위해 에셋을 업로드하는 사용자를 Frame.io 사용자로 활성화하는 것이 좋습니다.

사용자가 Workfront에서 Frame.io 사용자로 표시되고 프로젝트에 추가되면 다음과 같이 됩니다.

* Frame.io에서 공동 작업자로 추가됩니다. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* 정식 검토 및 승인을 위해 Frame.io에서 Workfront으로 자산을 전송할 수 있습니다.
* Workfront의 단방향 동기화 폴더에서 정보를 볼 수 있습니다. [!BADGE 준비 중]{type=Informative}

Frame.io 사용자를 활성화하려면:

{{step-1-to-users}}

1. 사용자를 한 명 이상 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.
1. 액세스 섹션에서 Frame.io의 프로젝트에 추가 확인란을 활성화한 다음 드롭다운 메뉴에서 **예**를 선택합니다.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >이 상자를 선택 취소하면 사용자는 이전 할당에 대한 액세스 권한을 유지하고 앞으로 Frame.io 프로젝트에 추가됩니다.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
