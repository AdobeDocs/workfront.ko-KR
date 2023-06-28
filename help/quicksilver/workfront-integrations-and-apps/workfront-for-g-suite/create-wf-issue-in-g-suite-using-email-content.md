---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: 만들기 [!DNL Adobe Workfront] 이메일 콘텐츠를 사용한 G Suite의 문제
description: 외부 이메일(에 의해 생성되지 않음)을 변환할 수 있습니다. [!DNL Adobe Workfront)] (으)로 [!DNL Workfront] 문제.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 만들기 [!DNL Adobe Workfront] 의 문제 [!DNL G Suite] 이메일 콘텐츠 사용

>[!NOTE]
>
>Google용 Adobe Workfront 플러그인의 최신 버전은 2023년 6월 26일에 릴리스되었습니다.

외부 이메일(에 의해 생성되지 않음)을 변환할 수 있습니다. [!DNL Adobe Workfront]) (으)로 [!DNL Workfront] 문제.

외부 이메일을 기존 문제에 대한 업데이트로 변환할 수도 있습니다. 자세한 내용은 [업데이트 [!DNL Adobe Workfront] 이메일 콘텐츠를 사용하는 [!DNL G Suite]의 항목](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

사용에 대한 정보 [!DNL G Suite] (이)가 보낸 알림 이메일을 사용하여 작업 [!DNL Workfront], 참조 [관리 [!DNL Adobe Workfront] [!DNL G Suite]의 알림 세부 정보](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

에서 문제를 만들기 전에 [!DNL G Suite], 다음을 수행해야 합니다.

* 설치 [!DNL Workfront for G suite]\
   자세한 내용은 [설치 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 만들기 [!DNL Adobe Workfront] 의 문제 [!DNL G Suite] 이메일 콘텐츠 사용

1. 다음과 같은 경우 [!UICONTROL Workfront for G Suite] 패널이 표시되지 않으면 [!DNL Workfront] 아이콘 ![](assets/wf-lion-icon.png) 다음에서 [!DNL G Suite] 페이지 오른쪽 끝에 있는 추가 기능 사이드바.
1. 에서 이메일 메시지가 열려 있는 상태 [!DNL G Suite]에서 옵션을 클릭합니다. [!DNL Workfront for G Suite] 이메일을 새 이메일로 변환 [!DNL Workfront] 문제.

   ![](assets/convert-email-task-issue-update.png)

1. 문제를 상위 프로젝트에 첨부하려면 **[!UICONTROL 프로젝트 이름]**&#x200B;에서 문제가 발생할 프로젝트의 이름을 입력한 다음 아래 목록에 표시될 때 프로젝트 이름을 클릭합니다.
1. 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 문제 이름]</td> 
      <td>이메일의 제목란에서 가져온 이 텍스트의 모든 부분을 편집합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>이메일 본문에서 가져온 이 텍스트의 일부를 편집합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 할당 대상]</td> 
      <td>클릭 <strong>[!UICONTROL 할당 대상]</strong>를 클릭하고 <strong>[!UICONTROL 할당 대상]</strong> 표시되는 옵션을 선택한 다음 해당 사용자의 이름을 입력하고 아래 목록에 나타나면 해당 이름을 클릭합니다. 추가하려는 각 사용자에 대해 이 작업을 반복한 다음 <strong>[!UICONTROL 저장]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 우선 순위]</td> 
      <td>드롭다운 화살표를 클릭한 다음, 문제에 대해 원하는 우선 순위를 클릭합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 이메일 첨부 파일 포함]</td> 
      <td> <p>이메일에 첨부 파일이 하나 이상 포함된 경우에만 사용할 수 있습니다. 이메일의 첨부 파일을 문제의 [!UICONTROL 문서] 영역에 저장하려면 이 옵션을 클릭합니다. </p> <p>첨부 파일을 저장하지 않으려면 이름 오른쪽에 있는 X를 클릭합니다. </p> <p>이메일에 문서에 대한 링크가 포함된 경우 [!DNL Google Drive], 만들고 있는 문제의 [!UICONTROL 개요] 탭에 저장됩니다. </p> <p>중요: 이 작업을 수행하려면 다음을 수행하십시오. [!DNL Workfront] 관리자가 권한을 부여해야 함 [!DNL Google Drive] 에서 문서 작업하기 [!DNL Workfront]섹션에 설명된 대로 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">문서 관리를 위한 통합 구성</a> 이 문서에서 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">문서 통합 구성</a>.</p> <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 변환하는 다른 이메일에 대해 활성화된 상태로 유지됩니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이메일 파일 포함</td> 
      <td> <p>원본 이메일을 이메일(EML)(이메일) 파일로 저장하려면 이 옵션을 클릭합니다 <span>[!UICONTROL Documents] 영역으로</span> 을 참조하십시오. 여기에서 파일을 두 번 클릭하여 이메일 애플리케이션에서 이메일을 열 수 있습니다.</p> <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 변환하는 다른 이메일에 대해 활성화된 상태로 유지됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 문제 만들기]**.

   다음 **[!UICONTROL 세부 사항]** 새 문제에 대한 탭이 [!DNL Workfront for G Suite] 패널. 다음을 클릭할 수 있습니다. **[!UICONTROL 업데이트]** 대화 상자를 종료하지 않고 바로 공동 작업자와 통신할 수 있습니다.

   의 맨 아래에서 **[!UICONTROL 세부 사항]** 탭을 클릭하고 **[!UICONTROL Workfront에서 보기]** Workfront의 새 문제로 이동합니다.

   브라우저를 새로 고치면 맨 아래에 링크가 있는 메시지가 표시됩니다. [!UICONTROL Workfront for G Suite] 패널에서 이메일이 문제로 전환되었음을 확인합니다.

   링크를 클릭하여 내의 세부 사항 보기로 이동할 수 있습니다. [!DNL Workfront for G Suite] 패널: 생성한 문제에 대해.

   이 단계를 반복하여 동일한 이메일을 여러 문제로 변환할 수 있습니다. 브라우저를 새로 고치거나 다른 시간에 이메일로 돌아가면 이메일에 대해 만든 모든 링크가 맨 아래에 나열됩니다. [!UICONTROL Workfront for G Suite] 패널.

1. (선택 사항)에서 문제 해결 계속 [!DNL Workfront for G Suite] 다음 중 하나를 수행하여 패널을 만듭니다.

   * 에 업데이트를 추가하려면 **[!UICONTROL 업데이트]** 탭을 클릭하고 **[!UICONTROL 새 업데이트 시작]** 업데이트를 입력합니다.

   * 의 업데이트에 회신하려면 **[!UICONTROL 업데이트]** 탭을 클릭하고 **[!UICONTROL 답변]** 회신을 입력하세요.

     위의 두 작업 모두에 대해 특정 사용자에게 댓글에 대해 알릴 수 있습니다. 클릭 **[!UICONTROL 알림]**&#x200B;에서 사용자 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다. 알림을 보낼 다른 사용자에 대해 이 프로세스를 반복한 다음 **[!UICONTROL Post]**.

   * 다음을 클릭합니다. **[!UICONTROL 문서]** 탭으로 이동하여 문제와 함께 저장된 문서를 확인합니다.
