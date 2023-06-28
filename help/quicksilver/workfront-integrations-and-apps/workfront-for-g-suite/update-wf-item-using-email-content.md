---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: 업데이트 [!DNL Adobe Workfront] 이메일 콘텐츠를 사용하는 G Suite의 항목
description: Adobe Workfront이 아닌 이메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 업데이트 [!DNL Adobe Workfront] 항목 출처: [!DNL G Suite] 이메일 콘텐츠 사용

>[!NOTE]
>
>Google용 Adobe Workfront 플러그인의 최신 버전은 2023년 6월 26일에 릴리스되었습니다.

기존 프로젝트, 작업 또는 문제를 비-의 정보로 업데이트할 수 있습니다.[!DNL Adobe Workfront] 이메일.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 전제 조건

을(를) 업데이트하기 전에 [!DNL Workfront] 이메일 콘텐츠를 사용하는 항목 [!DNL G Suite], 다음을 수행해야 합니다.

* 설치 [!DNL Workfront for G suite]\
   자세한 내용은 [설치 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 업데이트 [!DNL Workfront] 이메일 콘텐츠를 사용하는 항목 [!DNL G Suite]

1. 다음과 같은 경우 [!UICONTROL Workfront for G Suite] 패널이 표시되지 않으면 Workfront 아이콘을 클릭합니다 ![](assets/wf-lion-icon.png) 다음에서 [!DNL G Suite] 페이지 오른쪽 끝에 있는 추가 기능 사이드바.
1. 에서 이메일 메시지가 열려 있는 상태 [!DNL G Suite], 클릭 **[!UICONTROL 새 업데이트로 게시]** 다음에서 [!DNL G Suite] 패널.
1. 아래 **[!UICONTROL 유형]**&#x200B;을 클릭하고 드롭다운 화살표를 클릭한 다음, 업데이트를 추가할 오브젝트 유형을 클릭합니다.
1. 다음을 클릭합니다. **[!UICONTROL 검색 대상]** 옵션을 사용하여 업데이트를 추가할 개체 이름을 입력한 다음 아래 목록에 나타나는 항목을 선택합니다.

   이 옵션은 3단계에서 선택한 항목에 따라 다릅니다. 다음과 같을 수 있습니다 **[!UICONTROL 프로젝트 검색]**, **[!UICONTROL 작업 검색]**, 또는 **[!UICONTROL 문제 검색]**.

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
      <td><p>이메일에 첨부 파일이 하나 이상 포함된 경우에만 사용할 수 있습니다. 작업 또는 문제에 대한 [!UICONTROL 문서] 탭에서 첨부 파일을 저장하려면 이 옵션을 클릭합니다. </p><p>첨부 파일을 저장하지 않으려면 이름 오른쪽에 있는 X를 클릭합니다. </p><p>이메일에 문서에 대한 링크가 포함된 경우 [!DNL Google Drive], 링크는 만들고 있는 작업 또는 문제의 [!UICONTROL 개요] 탭에 저장됩니다. </p><p>중요 사항: <span style="color: #ff1493;"><span style="color: #000000;">이 작업을 수행하려면 다음을 수행하십시오.</span></span>[!DNL Workfront] 관리자<span style="color: #ff1493;"><span style="color: #000000;"> 승인 필요 [!DNL Google Drive] 로 작업하기 [!DNL Workfront]</span></span></p>
      <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 변환하는 다른 이메일에 대해 활성화된 상태로 유지됩니다.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">알림</td> 
      <td>클릭 <strong>[!UICONTROL Notify]</strong>를 클릭하고 <strong>[!UICONTROL 사용자 또는 팀 검색]</strong> 표시되는 옵션을 선택한 다음 개인 또는 팀의 이름을 입력하고 아래 목록에 나타나면 클릭합니다. 추가하려는 각 사용자 및 팀에 대해 이 작업을 반복한 다음 <strong>[!UICONTROL 저장]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 업데이트]**.

   브라우저를 새로 고치면 맨 아래에 링크가 있는 메시지가 표시됩니다. [!DNL Workfront for G Suite] 패널은 이메일을 업데이트로 전환했음을 확인합니다.

   링크를 클릭하여 [!UICONTROL 업데이트] 의 탭 [!DNL Workfront] 4단계에서 지정한 객체의 경우.

   이 단계를 반복하여 동일한 이메일을 업데이트, 작업 및 문제로 변환할 수 있습니다( 참조). [이메일 콘텐츠를 사용하여 [!DNL G Suite]에서 Adobe Workfront 문제 생성](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). 브라우저를 새로 고치거나 다른 시간에 이메일로 돌아가면 이메일에 대해 만든 모든 링크가 맨 아래에 나열됩니다. [!UICONTROL Workfront for G Suite] 패널.

1. (선택 사항) [!DNL Workfront] 다음 중 하나를 수행하여 추가 기능 패널:

   * 에 다른 업데이트를 추가하려면 **[!UICONTROL 업데이트]** 탭을 클릭하고 **[!UICONTROL 새 업데이트 시작]** 정보를 입력합니다.

   * 의 업데이트에 회신하려면 **[!UICONTROL 업데이트]** 탭을 클릭하고 **[!UICONTROL 답변]** 회신을 입력하세요.

     위의 두 옵션 모두에서 **[!UICONTROL 알림]** 을 눌러 5단계에서와 같이 회신에 대한 수신자를 지정합니다. 준비가 되면 다음을 클릭합니다. **[!UICONTROL Post]** 업데이트 또는 회신을 추가합니다.

   * 다음을 클릭합니다. **[!UICONTROL 세부 사항]** 탭으로 이동하여 새 프로젝트, 작업 또는 문제에 대한 세부 정보를 볼 수 있습니다.
