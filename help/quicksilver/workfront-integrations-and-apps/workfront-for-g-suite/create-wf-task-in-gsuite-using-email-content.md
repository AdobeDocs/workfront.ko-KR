---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: 이메일 콘텐츠를 사용하여 Google Workspace에서  [!DNL Adobe Workfront] 작업 만들기
description: 외부 전자 메일(Adobe  [!DNL Workfront]에서 생성되지 않음)을 Workfront 작업으로 변환할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# 전자 메일 콘텐츠를 사용하여 [!DNL Google Workspace]에서 [!DNL Adobe Workfront] 작업 만들기

>[!NOTE]
>
>Google용 Adobe Workfront 플러그인의 최신 버전은 2023년 6월 26일에 릴리스되었습니다.

외부 전자 메일([!DNL Adobe Workfront]에서 생성되지 않음)을 [!DNL Workfront] 작업으로 변환할 수 있습니다.

외부 이메일을 기존 작업에 대한 업데이트로 변환할 수도 있습니다. 자세한 내용은 [항목 업데이트 [!DNL Adobe Workfront] 출처 [!DNL Google Workspace] 이메일 콘텐츠 사용](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)을 참조하세요.

[!DNL Workfront]이(가) 보낸 알림 전자 메일로 작업하기 위해 [!DNL Google Workspace]을(를) 사용하는 방법에 대한 자세한 내용은 [관리 [!DNL Adobe Workfront] 알림 세부 정보 [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md)를 참조하세요.

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

[!DNL Google Workspace]에서 [!DNL Workfront] 작업을 만들려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront for Google Workspace] 설치\
   지침은 [설치 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)를 참조하십시오.

## 전자 메일 콘텐츠를 사용하여 [!DNL Google Workspace]에서 [!DNL Adobe Workfront] 작업 만들기

1. [!UICONTROL Workfront for Google Workspace] 패널이 표시되지 않으면 페이지의 오른쪽 끝에 있는 [!DNL Google Workspace] 추가 기능 사이드바에서 [!DNL Workfront] 아이콘 ![](assets/wf-lion-icon.png)을(를) 클릭하십시오.
1. [!DNL Google Workspace]에 전자 메일 메시지를 연 상태에서 [!DNL Workfront for Google Workspace]의 옵션을 클릭하여 전자 메일을 새 [!DNL Workfront] 작업으로 전환합니다.

1. **[!UICONTROL 새로 만들기]** 옵션을 선택하여 작업이 프로젝트의 일부가 될지 아니면 프로젝트와 독립적인 개인 작업이 될지 여부를 나타냅니다.
1. 작업을 상위 프로젝트에 연결하려면 **[!UICONTROL 프로젝트 이름]**&#x200B;을 클릭하고 작업을 원하는 프로젝트 이름을 입력한 다음 아래 목록에 표시될 때 프로젝트 이름을 클릭하십시오.
1. 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 작업 이름]</td> 
      <td>이메일의 제목란에서 가져온 이 텍스트의 모든 부분을 편집합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>이메일 본문에서 가져온 이 텍스트의 일부를 편집합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 할당 대상]</td> 
      <td><strong>[!UICONTROL 할당 대상]</strong>을 클릭하고 표시되는 <strong>[!UICONTROL 할당 대상]</strong> 옵션을 클릭한 다음, 사용자 이름을 입력하고 아래 목록에 나타나면 클릭합니다. 추가하려는 각 사용자에 대해 이 작업을 반복한 다음 <strong>[!UICONTROL 저장]</strong>을(를) 클릭합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 계획된 기간]</td> 
      <td> <p><strong>[!UICONTROL 계획된 기간]</strong>을(를) 클릭한 다음 작업을 수행할 일 수를 입력합니다. </p> <p>참고: 이 옵션은 다른 방법으로 조직에 대해 구성할 수 있습니다. 예를 들어 조직의 경우 일 대신 시간 수를 입력해야 할 수 있습니다. 자세한 내용은 [!DNL Workfront] 관리자에게 문의하십시오. 구성된 기본값 이외의 기간을 지정하려면 분, 시간, 일, 주 또는 개월을 나타내는 숫자 뒤에 <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> 또는 <strong>mo</strong>를 입력하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 우선 순위]</td> 
      <td>드롭다운 화살표를 클릭한 다음 작업에 대해 원하는 우선 순위를 클릭합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 이메일 첨부 파일 포함]</td> 
      <td> <p>이메일에 첨부 파일이 하나 이상 포함된 경우에만 사용할 수 있습니다. 이메일의 첨부 파일을 작업의 [!UICONTROL 문서] 영역에 저장하려면 이 옵션을 클릭합니다. </p> <p>첨부 파일을 저장하지 않으려면 이름 오른쪽에 있는 X를 클릭합니다. </p> <p>전자 메일에 [!DNL Google Drive]의 문서에 대한 링크가 포함되어 있으면 만들고 있는 작업의 [!UICONTROL 개요] 탭에 저장됩니다. </p> <p>중요: 이 기능이 작동하려면 [!DNL Workfront] 관리자가 문서 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">문서 통합 구성</a>의 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">문서를 관리하기 위한 통합 구성</a> 섹션에 설명된 대로 [!DNL Google Drive]에서 [!DNL Workfront]의 문서로 작업할 수 있도록 권한을 부여해야 합니다.</p> <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 변환하는 다른 이메일에 대해 활성화된 상태로 유지됩니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 이메일 파일 포함]</td> 
      <td> <p>원본 전자 메일을 EML(전자 메일) 파일 <span>로 작업의 [!UICONTROL 문서] 영역</span>에 저장하려면 이 옵션을 클릭합니다. 여기에서 파일을 두 번 클릭하여 이메일 애플리케이션에서 이메일을 열 수 있습니다.</p> <p>이 옵션을 활성화하면 작업, 문제 및 업데이트로 변환하는 다른 이메일에 대해 활성화된 상태로 유지됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 작업 만들기]**&#x200B;를 클릭합니다.

   새 작업에 대한 **[!UICONTROL 세부 정보]** 탭이 [!DNL Workfront for Google Workspace] 패널에 표시됩니다. **[!UICONTROL 업데이트]**&#x200B;를 클릭하고 받은 편지함을 떠나지 않고 바로 공동 작업자와 대화를 시작할 수 있습니다.

   **[!UICONTROL 세부 정보]** 탭 하단에서 **[!UICONTROL 다음 항목 보기[!DNL Workfront]]**&#x200B;를 클릭하여 Workfront의 새 작업으로 이동할 수도 있습니다.

   브라우저를 새로 고치면 [!DNL Workfront for Google Workspace] 패널 아래쪽에 링크가 있는 메시지가 표시되어 사용자가 전자 메일을 작업으로 전환했음을 확인합니다.

   링크를 클릭하여 [!DNL Workfront for Google Workspace] 패널 내의 만든 작업에 대한 세부 정보 보기로 이동할 수 있습니다.

   이 단계를 반복하여 동일한 이메일을 여러 작업으로 변환할 수 있습니다. 브라우저를 새로 고치거나 다른 시간에 전자 메일로 돌아가면 전자 메일에 대해 만든 모든 링크가 [!UICONTROL Google Workspace용 Workfront] 패널 하단에 나열됩니다.

1. (선택 사항) 다음 중 하나를 수행하여 [!DNL Workfront for Google Workspace] 패널에서 작업을 계속 수행합니다.

   * **[!UICONTROL 업데이트]** 탭에서 업데이트를 추가하려면 **[!UICONTROL 새 업데이트 시작]**&#x200B;을 클릭하고 업데이트를 입력하십시오.

   * **[!UICONTROL 업데이트]** 탭에서 업데이트에 회신하려면 **[!UICONTROL 회신]**&#x200B;을 클릭하고 회신을 입력하세요.

     위의 두 작업 모두에 대해 특정 사용자에게 댓글에 대해 알릴 수 있습니다. **[!UICONTROL 알림]**&#x200B;을 클릭하고 사용자 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다. 알림을 보낼 다른 사용자에 대해 이 프로세스를 반복한 다음 **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

   * 작업과 함께 저장된 문서를 보려면 **[!UICONTROL 문서]** 탭을 클릭하십시오.

이 단계를 반복하여 동일한 이메일을 여러 작업으로 변환할 수 있습니다. 브라우저를 새로 고치거나 다른 시간에 전자 메일로 돌아가면 전자 메일에 대해 만든 모든 링크가 [!DNL Workfront for Google Workspace] 패널 하단에 나열됩니다.
