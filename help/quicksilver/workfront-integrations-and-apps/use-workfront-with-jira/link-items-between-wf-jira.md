---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront] 과(와) [!DNL Jira] 사이의 항목 연결'
description: ' [!DNL Jira] 문제를  [!DNL Adobe Workfront] 작업 또는 문제에 자동 또는 수동으로 연결할 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 0%

---

# [!DNL Adobe Workfront]과(와) [!DNL Jira] 사이의 항목 연결

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Jira용 Workfront 통합을 사용할 수 없습니다.
>
>Jira와 조직의 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>공통 워크플로우를 복제하고 구현을 가속화하는 데 도움이 되는 8개의 Jira용 Workfront 자동화 및 통합 템플릿을 8월까지 사용할 수 있습니다. 템플릿은 특정 비즈니스 요구 사항을 충족하도록 완전히 맞춤화할 수 있으며 요구 사항이 발전함에 따라 확장될 수 있습니다.
> 
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Jira용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Jira 소프트웨어 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)을 참조하십시오.

[!DNL Jira] 문제를 [!DNL Adobe Workfront] 작업 또는 문제에 자동 또는 수동으로 연결할 수 있습니다.

[!DNL Workfront]의 항목 하나만 [!DNL Jira]의 항목 하나에 연결할 수 있습니다. 하나의 [!DNL Workfront] 항목을 여러 [!DNL Jira] 문제에 연결하거나 하나의 [!DNL Jira] 문제를 여러 [!DNL Workfront] 항목에 연결할 수 없습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] 플랜]</a></td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 라이선스 개요</a></td> 
   <td> 
   <p>새로운 기능: 표준<p>
   <p>또는</p>
   <p>현재: 플랜 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p><b>중요 사항</b>

사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 [!DNL Jira] 및 [!DNL Workfront]에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 사용하는 것이 좋습니다.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. [!DNL Workfront] 관리자에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>를 참조하십시오.</p> <p><b>메모</b>

아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Workfront]에서 [!DNL Jira] 사이의 항목을 연결하려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront]에 대해 [!DNL Jira]을(를) 설치합니다.

  자세한 내용은 [Jira용 Adobe Workfront 설치](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)를 참조하십시오.

* Jira에 대해 [!DNL Workfront]을(를) 구성합니다.

  자세한 내용은 [Jira용 Adobe Workfront 구성](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)을 참조하십시오.

## [!DNL Workfront]개 항목을 [!DNL Jira]개 문제에 자동으로 연결

[!DNL Workfront] 관리자는 [!DNL Jira]의 작업 또는 문제에 대해 특정 조건이 충족될 때마다 [!DNL Workfront]에서 문제를 자동으로 만드는 트리거를 정의할 수 있습니다. Workfront 및 [!DNL Jira]개 항목이 연결됩니다.

Jira에 대한 [!DNL Workfront]의 구성을 완료한 후 트리거와 일치하도록 [!DNL Workfront]에서 항목을 만들거나 업데이트하면 [!DNL Jira]에서 새 항목이 자동으로 만들어집니다.

Workfront 항목을 만들고 업데이트하는 Workfront 사용자는 [!DNL Jira]에서 항목 만들기를 트리거하기 위해 [!DNL Jira] 라이선스가 필요하지 않습니다.

자세한 내용은 [Jira용 구성 [!DNL Adobe Workfront] 을 참조하십시오](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>템플릿을 프로젝트에 연결하여 [!DNL Jira]개 항목을 자동으로 만들 수 있습니다. 템플릿에 [!DNL Jira] 트리거를 충족하는 할당이 있는 작업이 포함된 경우 새 작업에서 새 [!DNL Jira] 문제가 발생합니다.

[!DNL Workfront] 문제를 [!DNL Jira] 문제에 자동으로 연결하는 것은 [!DNL Workfront] 작업을 [!DNL Jira] 문제에 자동으로 연결하는 것과 동일합니다.

[!DNL Workfront] 작업을 [!DNL Jira] 문제에 자동으로 연결하려면 다음 작업을 수행하십시오.

1. [!DNL Jira]개 항목이 할당될 때 [!DNL Jira] 시스템 관리자가 [!DNL Workfront] 문제를 자동으로 만들기 위한 트리거를 구성했는지 확인한 다음, 작업을 만들 수 있는 액세스 수준으로 [!DNL Workfront]에 로그인하십시오.

   작업 액세스에 대한 자세한 내용은 [작업에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)를 참조하십시오.

{{step1-to-projects}}

1. **프로젝트** 페이지에서 프로젝트를 선택하십시오.

1. 프로젝트 왼쪽 패널에서 **[!UICONTROL 작업]**&#x200B;을(를) 선택합니다.

1. **+ 새 작업**&#x200B;을(를) 클릭합니다.

   >[!NOTE]
   >
   >기존 Workfront 항목을 Jira 문제에 연결하려면 해당 항목의 **자세히** **추가 아이콘** 메뉴에서 ![편집](assets/more-icon.png)을(를) 선택하십시오.

1. 작업에 사용할 수 있는 필드를 지정하거나 업데이트합니다.
1. **[!UICONTROL 할당]** 필드에서 [!DNL Jira] 통합에서 트리거로 지정된 사용자, 역할 또는 팀을 검색하고 선택합니다.

1. **작업 만들기**&#x200B;를 클릭합니다. 작업이 Workfront에서 만들어지고 작업의 **업데이트** 탭에 새 댓글이 표시되어 [!DNL Jira]에서도 새 문제가 만들어졌음을 나타냅니다.

1. (선택 사항) 작업 또는 문제 헤더의 **[!UICONTROL 세부 정보]** 섹션의 **[!UICONTROL 통합]** 영역에서 **[!UICONTROL Jira로 이동]** 링크를 클릭하여 Jira에서 문제를 엽니다.

   시스템 또는 그룹 관리자가 작업 또는 문제 헤더에 표시하려면 [!UICONTROL 통합] 필드를 레이아웃 템플릿에 추가해야 합니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

   [!DNL Jira] 사용자는 [!DNL Workfront]에서 자동으로 만든 항목에 대한 작업을 즉시 시작할 수 있으며, [!DNL Workfront]에 대한 라이선스가 없어도 해당 업데이트가 [!DNL Workfront]&#x200B;(으)로 전송됩니다.

   [!DNL Workfront] 추가 기능을 설정하는 동안 [!DNL Workfront] 관리자인 필드만 업데이트됩니다.

   Workfront과 Jira 간의 필드 동기화에 대한 자세한 내용은 [Jira용 Adobe Workfront 구성](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)의 Jira용 Workfront 구성 섹션을 참조하십시오.

   >[!NOTE]
   >
   >Workfront에서 자동으로 만들어지는 경우 [!DNL Jira] 문제는 [!DNL Jira]의 누구에게도 할당되지 않습니다.

## [!DNL Jira] 문제를 [!DNL Workfront]개 항목에 수동으로 연결

[!DNL Jira] 및 [!DNL Workfront]에서 항목을 서로 독립적으로 만든 후에는 [!DNL Jira] 문제를 기존 [!DNL Workfront] 작업 또는 문제에 수동으로 연결할 수 있습니다.

[!DNL Workfront]의 [!DNL Workfront] 항목을 기존 [!DNL Jira] 항목에 수동으로 연결할 수 없습니다.

>[!NOTE]
>
>[!DNL Jira] 문제가 [!DNL Workfront] 통합에서 트리거로 식별되지 않은 프로젝트에 없는 경우 [!DNL Jira] 온-프레미스와 통합을 사용할 때 이를 Workfront 항목에 수동으로 연결할 수 없습니다.\
>Workfront에서 Jira로의 트리거 설정에 대한 자세한 내용은 [Workfront 항목을 Jira 문제에 자동으로 연결](#automatically-link-workfront-items-to-jira-issues)을 참조하십시오.

[!DNL Workfront] 및 [!DNL Jira] 항목이 연결된 경우 한 항목의 특정 필드가 다른 항목에서 자동으로 업데이트될 수 있습니다.\
연결된 항목 업데이트에 대한 자세한 내용은 [Jira와 Adobe Workfront 간에 연결된 항목 업데이트](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md)를 참조하십시오.

[!DNL Jira] 문제를 [!DNL Workfront] 항목에 수동으로 연결하려면:

1. (조건부) [!DNL Workfront]에 로그인하고 [!DNL Jira] 문제에 연결할 문제 또는 작업을 찾습니다.
1. (조건부) **작업 세부 정보** 또는 **문제 세부 정보** 탭의 **기본 정보** 섹션에서 Workfront에 있는 항목의 **[!UICONTROL 참조 번호]**&#x200B;를 복사합니다.

   또는

   항목의 주소 표시줄에서 Workfront에 있는 항목의 **URL**&#x200B;을(를) 복사합니다.

   >[!IMPORTANT]
   >
   >조직이 Adobe 통합 경험에 온보딩된 경우 Workfront 항목을 Jira에 연결하려면 **참조 번호**&#x200B;를 사용해야 합니다. (URL 옵션을 사용할 수 있지만 이 옵션을 사용하면 오류가 반환됩니다.) 통합 경험에 대한 자세한 내용은 [Workfront용 Adobe 통합 경험](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.
   >
   >Adobe 통합 경험을 기반으로 하지 않는 조직의 경우 URL이 변경될 수 있으므로 URL 옵션을 사용하지 않는 것이 좋습니다.

   >[!NOTE]
   >
   >[!DNL Workfront]에 로그인하려면 [!DNL Workfront] 라이선스가 있어야 합니다. 그렇지 않으면 [!DNL Workfront] 사용자가 이 정보를 제공해야 합니다.

1. [!DNL Jira]에서 [!DNL Workfront] 항목에 수동으로 연결할 문제로 이동합니다.
1. [!DNL Workfront] 오른쪽 패널에 연결할 **[!UICONTROL 항목의]**&#x200B;참조 번호&#x200B;**또는** URL[!DNL Workfront]을(를) 붙여 넣습니다.

1. **[!UICONTROL 링크]**&#x200B;를 클릭합니다. 두 항목이 연결되고 [!DNL Workfront] 오른쪽 패널이 [!DNL Workfront] 항목의 정보로 채워집니다.

   기본적으로 다음 [!DNL Workfront] 필드가 [!DNL Jira] 오른쪽 패널의 [!DNL Workfront]에 표시됩니다.

   * 항목의 **[!UICONTROL 이름]**&#x200B;입니다. 패널에서 이름을 클릭하여 [!DNL Workfront] 항목에 액세스할 수 있습니다.
   * **[!UICONTROL 프로젝트 이름]**&#x200B;입니다.
   * 항목의 **[!UICONTROL 상태]**&#x200B;입니다.
   * 항목의 **[!UICONTROL 우선 순위]**&#x200B;입니다.
   * [!DNL Workfront]에 만든 날짜입니다.
   * 항목의 **[!UICONTROL 계획된 시간]**&#x200B;입니다.
   * **[!UICONTROL 참조 번호]**&#x200B;입니다. 패널의 [!DNL Workfront]참조 번호&#x200B;**을(를) 클릭하여** 항목에 액세스할 수 있습니다.

   오른쪽 패널에 표시할 추가 필드를 활성화하는 방법에 대한 자세한 내용은 [!DNL Jira]구성[!DNL Workfront]에서 [과(와)  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)개 항목 간의 필드 동기화 구성 섹션을 참조하십시오. 통합과 연결된 [!DNL Workfront] 관리자의 댓글이 **[!DNL Workfront]** 문제의 [!DNL Jira] 탭에 게시되어 새 [!DNL Jira] 항목이 생성되었는지 확인합니다. 댓글에 [!DNL Jira] 문제에 대한 링크가 포함되어 있습니다.

## [!DNL Jira]과(와) [!DNL Workfront] 사이의 항목 연결 해제

[!DNL Jira]에서 [!DNL Workfront] 사이의 연결된 항목은 [!DNL Jira]에서 수동으로 연결 해제할 수 있습니다. [!DNL Workfront]의 해당 [!DNL Jira]에서 [!DNL Workfront] 항목의 연결을 해제할 수 없습니다.

수동으로 연결된 항목에 대한 연결을 해제하려면 다음 액세스 권한이 필요합니다.

* 항목을 수동으로 연결한 사용자입니다.
* [!DNL Jira] 시스템 관리자입니다.

>[!NOTE]
>
>[!DNL Workfront] 관리자만 자동으로 연결된 항목의 연결을 해제할 수 있습니다.

[!DNL Jira] 항목에서 [!DNL Workfront] 문제의 연결을 해제하려면:

1. Jira에 로그인합니다.
1. [!DNL Workfront] 작업 또는 문제에 연결된 문제로 이동합니다.
1. **Workfront** 오른쪽 패널로 이동합니다.
1. **[!UICONTROL 연결 해제]** 아이콘을 클릭한 다음 **[!UICONTROL 연결 해제]**&#x200B;을 클릭합니다. 이전에 연결된 [!DNL Jira]개 및 [!DNL Workfront]개 항목의 연결이 해제되었습니다.

   필드, 주석 또는 나중에 업데이트되는 문서는 다른 애플리케이션의 이전 상대가 업데이트하지 않습니다.
