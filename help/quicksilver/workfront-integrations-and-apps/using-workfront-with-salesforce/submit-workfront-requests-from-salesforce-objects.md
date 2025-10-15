---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: ' [!DNL Adobe Workfront] 개체에서  [!DNL Salesforce] 요청 제출'
description: ' [!DNL Adobe Workfront] 기회 및 계정의  [!DNL Salesforce], you can submit [!DNL Workfront] for [!DNL Salesforce] 요청을 설치한 후. 이 기능은 Classic 및 Lightning Experience 프레임워크 모두에 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 개체에서 [!DNL Salesforce] 요청 제출

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Salesforce용 Workfront 통합을 사용할 수 없습니다.
>
>조직의 Salesforce 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Salesforce용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Salesforce 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)을 참조하십시오.

[!DNL Adobe Workfront for Salesforce]을(를) 설치한 후 [!DNL Workfront]개의 영업 기회 및 계정에서 [!DNL Salesforce]개의 요청을 제출할 수 있습니다. 이 기능은 [!DNL Classic] 및 [!DNL Lightning Experience] 프레임워크 모두에 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
   <p>플랜</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Workfront] 영업 기회 또는 계정에서 [!DNL Salesforce] 요청을 제출하려면 환경에 다음 항목이 있는지 확인하십시오.

* [!DNL Workfront] 관리자가 [!DNL Workfront for Salesforce]을(를) 설치했습니다.\
   [!DNL Workfront for Salesforce] 설치에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)를 참조하십시오

* [!DNL Workfront] 관리자가 [!DNL Workfront]기회[!UICONTROL &#x200B; 및 &#x200B;]계정[!UICONTROL &#x200B; 페이지 레이아웃에 &#x200B;] 섹션을 추가했습니다.\
   페이지 레이아웃에 [!DNL Workfront] 섹션을 추가하는 방법에 대한 자세한 내용은 [사용자를 위한  [!DNL Adobe Workfront] 섹션 구성 [!DNL Salesforce] 을 참조하십시오](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* [!DNL Workfront] 계정이 있으며 Opportunity 또는 Account 내의 [!DNL Workfront] 섹션에서 로그인할 수 있습니다.\
   로그인하면 [!UICONTROL 새 요청] 탭이 표시되어 요청 입력을 시작할 수 있습니다.

## [!DNL Workfront]에서 [!DNL Salesforce]개 요청 제출

1. Salesforce의 Opportunity 또는 Account 로 이동합니다.
1. [!DNL Workfront] 섹션으로 이동합니다.
1. **[!UICONTROL 새 요청]** 탭의 **[!UICONTROL 요청 유형 선택]** 드롭다운 메뉴에서 요청 유형을 선택합니다.

   Workfront에서 볼 수 있는 액세스 권한이 있는 것과 동일한 요청 대기열을 볼 수 있습니다.

1. 요청에 사용할 수 있는 필드를 입력하십시오.

   [!DNL Salesforce]에서 요청을 제출하는 것은 [!DNL Workfront] 웹 응용 프로그램에서 요청을 제출하는 것과 동일합니다.

   >[!NOTE]
   >
   >[!DNL Workfront]에서 [!DNL Salesforce] 플러그인을 사용하여 문서를 업로드할 수 없습니다.

   [만들기 및 제출 [!DNL Adobe Workfront] 요청](../../manage-work/requests/create-requests/create-submit-requests.md)에 설명된 단계를 계속 수행합니다.

1. **[!UICONTROL 제출을 클릭합니다]**.

## [!DNL Workfront]개 요청 보기

1. [!DNL Salesforce]의 영업 기회 또는 계정으로 이동합니다.
1. **[!DNL Workfront]** 섹션으로 이동합니다.

   >[!NOTE]
   >
   >[!DNL Workfront] 관리자가 이 섹션을 구성한 방법에 따라 다른 이름을 사용할 수 있습니다.

1. **[!UICONTROL 제출된 요청]** 탭을 선택합니다.

   이 탭에서 사용자 또는 다른 사용자가 이 영업 기회 또는 계정에서 제출한 모든 요청을 볼 수 있습니다. 웹 응용 프로그램의 이 요청 대기열에 제출한 요청은 [!DNL Salesforce]의 이 목록에 표시되지 않습니다.

   >[!NOTE]
   >
   >웹 애플리케이션의 이 요청 대기열에 제출된 요청은 Salesforce의 이 목록에 표시되지 않습니다.

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   제출된 요청에 대한 다음 정보를 볼 수 있습니다.

   * 요청 이름([!UICONTROL 제목] 열)
   * 참조 번호
   * 요청 유형
   * 상태
   * 제출된 날짜
   * 요청한 사람 이름
   * 이름에 할당됨\

     [!DNL Workfront]에서 이 정보가 업데이트되면 이 목록에서도 업데이트됩니다.

1. (선택 사항) 요청 이름을 클릭하여 [!DNL Workfront]에서 엽니다.

1. (선택 사항) **[!UICONTROL 이동[!DNL Salesforce]]**&#x200B;을(를) 클릭하여 Workfront의 다음 영역에서 문제가 발생한 영업 기회 또는 계정에 액세스합니다.

   * 문제의 [!UICONTROL 세부 정보] 섹션에서
   * 목록에서 문제를 선택할 때 요약 패널에서 목록의 도구 모음에서 [!UICONTROL 요약 열기] ![요약 패널 아이콘](assets/summary-panel-icon.png)을 클릭합니다.
   * 문제 헤더에서 [!UICONTROL 통합] 필드를 사용할 수 있는 경우. 시스템 또는 그룹 관리자가 [!UICONTROL 통합] 필드를 레이아웃 템플릿에 추가하여 문제 헤더에서 Salesforce으로 이동 링크를 확인해야 합니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

   >[!NOTE]
   >
   >[!UICONTROL Salesforce으로 이동] 링크가 문제를 볼 수 있는 모든 [!DNL Workfront] 사용자에게 표시됩니다. 문제가 기록된 [!DNL Salesforce] 영업 기회 또는 계정으로 이동하려면 [!DNL Salesforce] 계정이 있어야 합니다.
