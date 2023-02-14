---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,슬라이드
navigation-topic: workfront-for-g-suite
title: 만들기 [!DNL Adobe Workfront] 이메일 콘텐츠를 사용한 G Suite의 문제
description: 외부 이메일을 변환할 수 있습니다(에서 생성하지 않음) [!DNL Adobe Workfront)] 변환 후 [!DNL Workfront] 문제.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# 만들기 [!DNL Adobe Workfront] 문제 [!DNL G Suite] 이메일 콘텐츠 사용

>[!NOTE]
>
>다음 항목이 있습니다 [알려진 문제](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 현재 버전의 [!DNL Workfront for G Suite] 예상대로 작동하지 않습니다. Adobe는 새 버전에서 작업하고 있으며 Launch가 [!DNL Google Marketplace] 가까운 미래에.

외부 이메일을 변환할 수 있습니다(에서 생성하지 않음) [!DNL Adobe Workfront]) [!DNL Workfront] 문제.

외부 이메일을 기존 문제에 대한 업데이트로 변환할 수도 있습니다. 자세한 내용은 [업데이트 [!DNL Adobe Workfront] 전자 메일 콘텐츠를 사용하여 [!DNL G Suite]의 항목](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

사용에 대한 자세한 정보 [!DNL G Suite] 보낸 알림 이메일을 사용하여 작업 [!DNL Workfront]를 참조하십시오. [관리 [!DNL Adobe Workfront] [!DNL G Suite]의 알림 세부 정보](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

다음에서 문제를 만들려면 먼저 [!DNL G Suite]:

* 설치 [!DNL Workfront for G suite]\
   자세한 내용은 [설치 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 만들기 [!DNL Adobe Workfront] 문제 [!DNL G Suite] 이메일 콘텐츠 사용

1. 만약 [!UICONTROL G Suite용 Workfront] 패널이 표시되지 않으면 [!DNL Workfront] 아이콘 ![](assets/wf-lion-icon.png) 에서 [!DNL G Suite] 페이지 맨 오른쪽에 있는 추가 기능 사이드바.
1. 전자 메일 메시지를 연 상태에서 [!DNL G Suite]에서 옵션을 클릭합니다. [!DNL Workfront for G Suite] 이메일을 새 주소로 변환하려면 [!DNL Workfront] 문제.

   ![](assets/convert-email-task-issue-update.png)

1. 문제를 상위 프로젝트에 첨부하려면 **[!UICONTROL 프로젝트 이름]**&#x200B;에서 문제를 해결할 프로젝트의 이름을 입력하고 아래 목록에 프로젝트 이름이 표시되면 프로젝트 이름을 클릭합니다.
1. 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 문제 이름]</td> 
      <td>이메일 제목 줄에서 가져온 이 텍스트의 일부를 편집합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>이메일 본문에서 가져온 이 텍스트의 일부를 편집합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 할당 대상]</td> 
      <td>클릭 <strong>[!UICONTROL 할당 대상]</strong>를 클릭하고 <strong>[!UICONTROL 다음 항목에 할당]</strong> 옵션이 표시되면 이름을 입력하고 아래 목록에 이 이름이 나타나면 클릭합니다. 추가할 각 사용자에 대해 이 단계를 반복한 다음 를 클릭합니다 <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>드롭다운 화살표를 클릭한 다음 문제에 대해 원하는 우선 순위를 클릭합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 전자 메일 첨부 파일 포함]</td> 
      <td> <p>이메일에 하나 이상의 첨부 파일이 포함된 경우에만 사용할 수 있습니다. 전자 메일의 첨부 파일을 문제의 [!UICONTROL 문서] 영역에 저장하려면 이 옵션을 클릭합니다. </p> <p>첨부 파일을 저장하지 않으려면 해당 이름의 오른쪽에 있는 X 를 클릭합니다. </p> <p>전자 메일에 의 문서에 대한 링크가 포함되어 있는 경우 [!DNL Google Drive]를 입력하면 생성 중인 문제의 [!UICONTROL 개요] 탭에 저장됩니다. </p> <p>중요 사항: 이렇게 하려면 [!DNL Workfront] 관리자 권한 [!DNL Google Drive] 에서 문서를 사용하여 작업 [!DNL Workfront]섹션에 설명된 대로 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">문서 관리를 위한 통합 구성</a> 기사 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">문서 통합 구성</a>.</p> <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 전환하는 다른 이메일에 대해 활성화됩니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">전자 메일 파일 포함</td> 
      <td> <p>원본 이메일을 이메일(EML)(이메일) 파일로 저장하려면 이 옵션을 클릭합니다 <span>[!UICONTROL Documents] 영역으로 이동합니다.</span> 문제. 여기에서 파일을 두 번 클릭하여 이메일 애플리케이션에서 이메일을 열 수 있습니다.</p> <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 전환하는 다른 이메일에 대해 활성화됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 문제 만들기]**.

   다음 **[!UICONTROL 세부 사항]** 새 문제에 대한 탭에 [!DNL Workfront for G Suite] 패널. 을(를) 클릭합니다 **[!UICONTROL 업데이트]** 그리고 을(를) 즉시 상태로 두지 않고 공동 작업자와 커뮤니케이션을 시작합니다.

   아래쪽에서 **[!UICONTROL 세부 사항]** 탭에서 **[!UICONTROL Workfront에서 보기]** Workfront의 새 문제로 이동합니다.

   브라우저를 새로 고치면, [!UICONTROL G Suite용 Workfront] 패널에서 이메일이 문제로 변환되었는지 확인합니다.

   ![](assets/email-was-converted.png)

   링크를 클릭하여 [!DNL Workfront for G Suite] 패널에 표시되어야 합니다.

   이 단계를 반복하여 동일한 이메일을 여러 문제로 변환할 수 있습니다. 브라우저를 새로 고치거나 다른 시간에 이메일로 돌아가면 전자 메일에 대해 만든 모든 링크가 의 맨 아래에 나열됩니다 [!UICONTROL G Suite용 Workfront] 패널.

1. (선택 사항)에서 문제를 계속 처리합니다 [!DNL Workfront for G Suite] 다음 중 하나를 수행하여 패널을 엽니다.

   * 에 업데이트를 추가하려면 **[!UICONTROL 업데이트]** 탭, **[!UICONTROL 새 업데이트 시작]** 업데이트를 입력합니다.

   * 에 대한 업데이트에 응답하려면 **[!UICONTROL 업데이트]** 탭, **[!UICONTROL 회신]** 답변을 입력합니다.

      위의 두 작업 모두에 대해 특정 사용자에게 주석에 대해 알릴 수 있습니다. 클릭 **[!UICONTROL 알림]**&#x200B;을 입력하여 사용자 이름을 입력한 다음 드롭다운 목록에 표시될 이름을 클릭합니다. 알릴 다른 사용자에 대해 이 프로세스를 반복한 다음 **[!UICONTROL Post]**.

   * 을(를) 클릭합니다. **[!UICONTROL 문서]** 탭하여 문제와 함께 저장된 문서를 볼 수 있습니다.
