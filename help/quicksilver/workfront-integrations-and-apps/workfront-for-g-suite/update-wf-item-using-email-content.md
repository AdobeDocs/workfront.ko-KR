---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: 이메일 콘텐츠를 사용하여 Google Workspace에서  [!DNL Adobe Workfront] 항목 업데이트
description: Adobe Workfront이 아닌 이메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# 전자 메일 콘텐츠를 사용하여 [!DNL Adobe Workfront]에서 [!DNL Google Workspace] 항목 업데이트

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

[!DNL Adobe Workfront]이(가) 아닌 전자 메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 전제 조건

[!DNL Workfront]의 전자 메일 콘텐츠를 사용하여 [!DNL Google Workspace] 항목을 업데이트하려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront for Google Workspace] 설치\
   지침은 [설치 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)를 참조하십시오.

## [!DNL Workfront]의 전자 메일 콘텐츠를 사용하여 [!DNL Google Workspace] 항목 업데이트

1. [!UICONTROL Google Workspace용 Workfront] 패널이 표시되지 않으면 페이지의 오른쪽 끝에 있는 ![ 추가 기능 사이드바에서 Workfront 아이콘 ](assets/wf-lion-icon.png)Workfront 아이콘[!DNL Google Workspace]을 클릭하십시오.
1. [!DNL Google Workspace]에 전자 메일 메시지를 연 상태에서 **[!UICONTROL 패널에서]**&#x200B;새 업데이트로 게시[!DNL Google Workspace]를 클릭합니다.
1. **[!UICONTROL Type]**&#x200B;에서 드롭다운 화살표를 클릭한 다음 업데이트를 추가할 개체 형식을 클릭합니다.
1. **[!UICONTROL 검색]** 옵션을 클릭하고 업데이트를 추가할 개체 이름을 입력한 다음 아래 목록에 나타나는 항목을 선택합니다.

   이 옵션은 3단계에서 선택한 항목에 따라 다릅니다. **[!UICONTROL 프로젝트 검색]**, **[!UICONTROL 작업 검색]** 또는 **[!UICONTROL 문제 검색]**&#x200B;일 수 있습니다.

   >[!NOTE]
   >
   >작업 이름을 입력할 때 Ad Hoc Personal 작업은 아래 표시되는 이름 목록에서 제외됩니다.

1. 다음 옵션 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 업데이트]</td> 
      <td>이메일의 제목 줄 및 본문 텍스트에서 가져온 이 텍스트의 일부를 편집합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 이메일 첨부 파일 포함]</td> 
      <td><p>이메일에 첨부 파일이 하나 이상 포함된 경우에만 사용할 수 있습니다. 작업 또는 문제에 대한 [!UICONTROL 문서] 탭에서 첨부 파일을 저장하려면 이 옵션을 클릭합니다. </p><p>첨부 파일을 저장하지 않으려면 이름 오른쪽에 있는 X를 클릭합니다. </p><p>전자 메일에 [!DNL Google Drive]의 문서에 대한 링크가 포함된 경우 해당 링크는 만들고 있는 작업 또는 문제의 [!UICONTROL 개요] 탭에 저장됩니다. </p><p>중요: <span style="color: #ff1493;"><span style="color: #000000;">이 작업을 수행하려면 </span></span>[!DNL Workfront] 관리자<span style="color: #ff1493;"><span style="color: #000000;">가 [!DNL Google Drive]에서 작업할 수 있도록 [!DNL Workfront]</span></span>을(를) 승인해야 합니다.</p>
      <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 변환하는 다른 이메일에 대해 활성화된 상태로 유지됩니다.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">알림</td> 
      <td><strong>[!UICONTROL 알림]</strong>을(를) 클릭하고 표시되는 <strong>[!UICONTROL 사용자 또는 팀 검색]</strong> 옵션을 클릭한 다음 사용자 또는 팀의 이름을 입력하고 아래 목록에 나타나면 클릭합니다. 추가하려는 각 사용자 및 팀에 대해 이 작업을 반복한 다음 <strong>[!UICONTROL 저장]</strong>을(를) 클릭합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 업데이트]**&#x200B;를 클릭합니다.

   브라우저를 새로 고치면 [!DNL Workfront for Google Workspace] 패널 아래쪽에 링크가 있는 메시지가 표시되어 전자 메일을 업데이트로 전환했음을 확인합니다.

   링크를 클릭하여 4단계에서 지정한 개체에 대한 [!UICONTROL 의 &#x200B;]업데이트[!DNL Workfront] 탭으로 이동할 수 있습니다.

   이 단계를 반복하여 업데이트, 작업 및 문제로 같은 전자 메일을 변환할 수 있습니다([Adobe Workfront 문제 만들기 [!DNL Google Workspace] 전자 메일 콘텐츠 사용](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md) 참조). 브라우저를 새로 고치거나 다른 시간에 전자 메일로 돌아가면 전자 메일에 대해 만든 모든 링크가 [!UICONTROL Google Workspace용 Workfront] 패널 하단에 나열됩니다.

1. (선택 사항) 다음을 수행하여 [!DNL Workfront] 추가 기능 패널에서 업데이트 작업을 계속합니다.

   * **[!UICONTROL 업데이트]** 탭에서 다른 업데이트를 추가하려면 **[!UICONTROL 새 업데이트 시작]**&#x200B;을 클릭하고 정보를 입력하십시오.

   * **[!UICONTROL 업데이트]** 탭에서 업데이트에 회신하려면 **[!UICONTROL 회신]**&#x200B;을 클릭하고 회신을 입력하세요.

     위의 두 옵션 모두에 대해 **[!UICONTROL 알림]**&#x200B;을 클릭하여 5단계에서와 같이 회신에 대한 수신자를 지정할 수 있습니다. 준비가 되면 **[!UICONTROL 게시]**&#x200B;를 클릭하여 업데이트 또는 회신을 추가합니다.

   * 새 프로젝트, 작업 또는 문제에 대한 세부 정보를 보려면 **[!UICONTROL 세부 정보]** 탭을 클릭하십시오.
