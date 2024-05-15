---
title: 구성 [!DNL Workfront] 및 [!DNL Frame.io] 통합
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: (으)로 [!DNL Adobe Workfront] 관리자, [!DNL Workfront] 포함 [!DNL Frame.io] 또한 조직에서 에셋을 검토하고 승인할 수 있는 원활한 방법을 제공합니다.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# 구성 [!DNL Workfront] 및 [!DNL Frame.io] 통합

Workfront 관리자는 설정 영역에서 기본 Frame.io 계정을 구성한 다음 Workfront에서 Frame.io 사용자를 지정하여 Workfront과 Frame.io 간을 통합할 수 있습니다. 이를 통해 프로젝트 코디네이터는 Workfront 프로젝트를 사용하여 작업을 계획하고 시작하고, 워크플로를 검토 및 승인할 수 있습니다.


## 액세스 요구 사항

>[!IMPORTANT]
>
>이 기능은 (으)로 온보딩된 조직에서만 사용할 수 있습니다. [!DNL Adobe Admin Console].

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 플랜</strong>
   </td>
   <td>임의
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 라이선스</strong>
   </td>
   <td>현재: [!UICONTROL Plan] <br>
   새로운 기능: [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong>액세스 수준 구성</strong>
   </td>
   <td>다음이어야 합니다: [!DNL Workfront] 관리자.
   </td>
  </tr>

</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 기본 구성 [!DNL Frame.io] account [!BADGE 곧 출시 예정]{type=Informative}

한 번 기본값 [!DNL Frame.io] 계정이에 프로젝트가 생성됨 [!DNL Workfront] frame.io에서 미러 프로젝트가 생성되었습니다.

>[!IMPORTANT]
>
>이 기능은 곧 제공될 예정입니다. 현재 Frame.io 계정은 Workfront 팀에서 수동으로 추가합니다. 도움이 필요하면 Adobe 계정 담당자에게 문의하십시오.

## Workfront 그룹으로 단일 Frame.io 계정 구성

단일 Workfront 그룹을 기본 계정과 다른 단일 Frame.io 계정과 연결할 수 있습니다.

Workfront 그룹으로 단일 Frame.io 계정을 구성하려면 다음 작업을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**.
1. 기존 그룹을 선택하거나 **그룹 만들기**.
1. 왼쪽 패널에서 **Frame.io에 연결**.
1. API 개발자 토큰을 입력합니다.
1. 클릭 **연결 시작**.
1. (조건부) 둘 이상의 Frame.io 계정의 관리자인 경우 사용할 계정을 선택합니다.

## Frame.io 사용자 활성화

Frame.io를 정기적으로 사용하는 Workfront 사용자는 Frame.io 사용자로 표시되어야 합니다. Workfront 관리자는 Workfront 사용자 프로필에서 Frame.io 사용자를 지정할 수 있습니다.

>[!TIP]
>
>크리에이티브 도구에서 정기적으로 작업하고 검토 및 승인을 위해 에셋을 업로드하는 사용자를 Frame.io 사용자로 활성화하는 것이 좋습니다.

사용자가 Workfront에서 Frame.io 사용자로 표시되고 프로젝트에 추가되면 다음과 같이 됩니다.

* Frame.io에서 공동 작업자로 추가됩니다. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* 정식 검토 및 승인을 위해 Frame.io에서 Workfront으로 자산을 전송할 수 있습니다.
* Workfront의 단방향 동기화 폴더에서 정보를 볼 수 있습니다. [!BADGE 곧 출시 예정]{type=Informative}

Frame.io 사용자를 활성화하려면:

{{step-1-to-users}}

1. 사용자를 한 명 이상 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png).
1. Access 섹션에서 Frame.io의 프로젝트에 추가 확인란을 활성화한 다음 을 선택합니다 **예** 을 클릭하여 제품에서 사용할 수 있습니다.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >이 상자를 선택 취소하면 사용자는 이전 할당에 대한 액세스 권한을 유지하고 앞으로 Frame.io 프로젝트에 추가됩니다.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->

