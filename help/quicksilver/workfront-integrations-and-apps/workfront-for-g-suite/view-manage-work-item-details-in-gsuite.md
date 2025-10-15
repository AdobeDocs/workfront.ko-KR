---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Google Workspace에서  [!DNL Adobe Workfront] 개체 세부 정보 보기 및 관리
description: Google Workspace에서 나가지 않고도 작업 항목의 세부 정보를 보고 관리할 수 있습니다. 예를 들어, Google Workspace의 경우  [!DNL Adobe Workfront]  내에서 작업의 설명을 읽고, 상위 개체를 보고, 상태를 변경하고, 완료로 표시할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 0f15b05f-3b4a-4f0b-9d9a-21a0f97de1ea
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# [!DNL Adobe Workfront]에서 [!DNL Google Workspace] 개체 세부 정보 보기 및 관리

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 다음 Google Workspace용 Workfront 기능은 **2026년 2월 28일** 이후에 사용할 수 없습니다.
>
>* Workfront 내에서 Google Workspace 기능 액세스
>
>* Gmail 또는 Google Calendar 사이트 패널에서 Workfront 작업 보기 및 관리
>
>조직의 Google Workspace 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Google Workspace용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Gmail 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) 및 [Google 달력 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)을 참조하십시오.

[!DNL Google Workspace]에서 나가지 않고 작업 항목의 세부 정보를 보고 관리할 수 있습니다. 예를 들어 [!DNL Adobe Workfront for Google Workspace] 내에서 작업의 설명을 읽고, 상위 개체를 보고, 상태를 변경하고, 완료로 표시할 수 있습니다.

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
   <td> <p>표준</p><p>작업 이상</p>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Google Workspace]에서 작업 항목 세부 정보를 보고 관리하려면 먼저 다음을 수행해야 합니다

* [!DNL Workfront for Google Workspace] 설치\
   지침은 [설치 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)를 참조하십시오.

## [!DNL Google Workspace]에서 작업 항목 세부 정보 보기 및 관리

1. [!UICONTROL Google용 Workfront Workspace] 패널이 표시되지 않으면 페이지의 오른쪽 끝에 있는 [!DNL Workfront] 추가 기능 사이드바에서 ![&#x200B; 아이콘 &#x200B;](assets/wf-lion-icon.png)Workfront 아이콘[!DNL Google Workspace]을 클릭하십시오.
1. [!DNL Workfront]의 [!DNL Google Workspace]Access[Home [!DNL Adobe Workfront] [!UICONTROL &#x200B; 콘텐츠에 설명된 대로 &#x200B;] 내의  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md) 작업 또는 문제로 이동합니다.

   작업 또는 문제를 선택하면 **[!UICONTROL 세부 정보]** 탭이 열립니다. **[!UICONTROL 세부 정보]** 탭 위의 영역에는 상위 개체의 이름, 작업 또는 문제의 이름, [!UICONTROL 기한]&#x200B;(작업인 경우) 또는 [!UICONTROL 우선 순위 날짜]&#x200B;(문제인 경우)가 표시됩니다.


   [!DNL Google Workspace]을(를) 종료하지 않고 이 탭에서 다음을 포함한 다양한 작업을 수행할 수 있습니다.

   * 개체의 **[!UICONTROL 설명]**&#x200B;과(와) 개체에 할당된 사용자, **[!UICONTROL 우선 순위]**, 요청자, **[!UICONTROL 계획된 완료 일자]**, 개체에 첨부된 사용자 정의 필드 및 양식과 같은 기타 세부 정보를 봅니다.

     사용자 정의 양식은 정보가 추가된 필드만 표시합니다.

   * 상위 개체의 세부 정보를 보려면 **[!UICONTROL 상위 프로젝트]** 영역을 클릭하십시오.

     >[!TIP]
     >
     >이 기능은 동일한 이름의 작업 및 문제가 있고 이를 구분해야 할 때 유용합니다.

   * **[!UICONTROL 작업]**&#x200B;을 클릭하여 할당된 작업을 수락합니다.
   * **[!UICONTROL 완료]** 옵션, **[!UICONTROL 상태]**, **[!UICONTROL 완료율]** 등 다양한 옵션을 편집합니다.

     **[!UICONTROL 완료율]**&#x200B;에 숫자와 백분율 기호(%)를 입력하여 항목에 대한 진행 상황을 나타냅니다.
   * 소유자, 크기 및 첨부 파일을 포함하여 승인 요청에 대한 정보를 봅니다.
   * **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]** 승인 요청 및 문서.

   * **[!UICONTROL 액세스 요청을 승인]** 또는 **[!UICONTROL 무시]**&#x200B;합니다.

1. (선택 사항) **[!UICONTROL 의 현재 작업 항목으로 이동하려면[!DNL Workfront]]**&#x200B;의 [!DNL Workfront]보기를 클릭합니다.

* [!UICONTROL 에서 &#x200B;]업데이트[!DNL Workfront for Google Workspace] 탭을 사용하는 방법에 대한 자세한 내용은 [개체 업데이트 [!DNL Adobe Workfront] 를 참조하십시오. [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md)
* [!UICONTROL 에서 &#x200B;]문서[!DNL Workfront for Google Workspace] 탭을 사용하는 방법에 대한 자세한 내용은 [[!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md)에서 문서 보기 및 관리를 참조하십시오.
