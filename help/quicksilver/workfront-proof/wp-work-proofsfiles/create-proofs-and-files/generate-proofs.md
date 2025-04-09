---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: ' [!DNL Workfront Proof]에서 증명 생성'
description: Workfront Proof을 사용하면 문서 또는 웹 사이트에서 증명을 만들고 다른 사용자와 공유할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 1%

---

# [!DNL Workfront Proof]에서 증명 생성

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Workfront Proof]을(를) 사용하면 문서나 웹 사이트에서 증명을 만들고 다른 사용자와 공유할 수 있습니다. 다음 단계에서는 사용할 수 있는 다양한 구성 옵션에 대해 설명합니다.

## 문서에서 증명 생성

1. **[!UICONTROL 새 증명]** 페이지를 열려면 다음 중 하나를 수행하십시오.

   * 페이지의 왼쪽 상단에 있는 **[!UICONTROL 새 증명]** 단추를 클릭합니다.
   * Dropzone(엔터프라이즈 기능)을 통해 제출합니다.

1. 하나 이상의 문서를 증명하려면 다음 방법 중 하나로 증명을 추가할 문서를 추가합니다(이 프로세스를 반복하여 여러 문서를 추가).

   * 파일 시스템의 문서를 **[!UICONTROL 파일 추가]** 영역의 드래그 앤 드롭 영역으로 드래그합니다.
   * **[!UICONTROL 파일 추가]** 영역에서 **찾아보기** 링크를 클릭하여 워크스테이션의 파일 시스템에서 업로드할 문서를 찾아 선택합니다.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. 웹 사이트를 증명하려면 **[!UICONTROL 파일 추가]** 영역에 웹 사이트의 URL을 입력한 다음 **[!UICONTROL Enter]**&#x200B;를 누르십시오. 증명에 여러 웹 사이트를 추가하려면 이 단계를 반복합니다.

   증명 웹 사이트에 대한 자세한 내용은 [URL에 대한 증명 생성](#generate-a-proof-for-a-url)을 참조하세요.

   ![증명 웹 사이트](assets/proof-website-350x65.png)

1. (선택 사항) 업로드된 파일의 파일 이름을 수정합니다.

   1. 문서 목록에서 수정할 문서 이름을 마우스로 가리킨 다음 **[!UICONTROL 편집]** 아이콘을 클릭합니다.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. **[!UICONTROL 증명 이름]** 필드에서 새 이름을 지정한 다음 **[!UICONTROL 완료]**&#x200B;를 클릭합니다.

   1. (선택 사항) 업로드되는 파일을 삭제하려면 문서 목록에서 삭제할 문서를 마우스로 가리킨 다음 **[!UICONTROL 삭제]** 아이콘을 클릭합니다.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (선택 사항) **[!UICONTROL 모든 호환 파일을 하나의 증명으로 결합]** 옵션을 활성화합니다.

      **이 옵션이 활성화된 경우:** 모든 정적 파일과 웹 사이트를 하나의 증명으로 사용할 수 있으며 지정된 시간에 최대 50개의 파일을 업로드할 수 있습니다.

      >[!NOTE]
      >
      >비디오 및 대화형 웹 사이트를 포함한 대화형 파일은 하나의 증명으로 결합할 수 없습니다.

      **이 옵션을 사용하지 않도록 설정한 경우:** 모든 문서와 웹 사이트가 개별 증명으로 생성되며 한 번에 최대 20개의 파일을 업로드할 수 있습니다.

      업로드된 모든 파일과 웹 사이트를 하나의 증명으로 결합하려면 다음을 수행하십시오.

      1. **[!UICONTROL 호환 가능한 모든 파일을 하나의 증명으로 결합]** 옵션을 활성화합니다.
      1. **[!UICONTROL 증명 이름]** 필드에 결합된 증명의 새 이름을 입력합니다.
      1. **[!UICONTROL 파일 추가]** 영역에서 파일을 원하는 순서로 끌어 포함된 파일의 순서를 변경합니다. 파일 순서는 결합된 증명의 페이지 순서입니다. 결합된 증명 만들기에 대한 자세한 내용은 [다중 페이지 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)를 참조하십시오.

1. (선택 사항) 여러 단계를 포함하는 자동화된 워크플로를 사용하려면 **[!UICONTROL 워크플로]** 섹션에서 다음 옵션 중 선택하십시오.

   * **기본:** 증명을 만든 후 즉시 액세스할 사용자를 지정하려면 이 옵션을 선택하십시오. 여러 사용자와 증명을 공유할 수 있습니다.

     증명 공유에 대한 자세한 내용은 [다음 범위 내에서 증명 공유 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)를 참조하세요.

   * **자동:** 검토 프로세스가 복잡하거나 검토용 콘텐츠를 동일한 사용자 그룹에 정기적으로 보내는 경우 콘텐츠 검토 및 승인을 관리하려면 이 옵션을 선택하십시오. 자동화된 워크플로를 사용하면 증명이 최종 승인될 때까지 단계에서 스테이지로 이동합니다. 관련 사용자는 승인을 해야 한다는 알림을 언제든지 받습니다.

     자동화된 워크플로 만들기에 대한 자세한 내용은 [자동화된 워크플로를 사용하여 증명 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2)을 참조하십시오.

1. 이전 단계에서 선택한 사용자에게 이메일 알림 및 사용자 지정 메시지를 전송할지 여부를 선택합니다.

   * **이 증명에 대해 수신자에게 알림:** 사용자에게 전자 메일 알림을 보내려면 이 옵션을 선택하십시오. **[!UICONTROL 워크플로]** 섹션에서 **[!UICONTROL 기본 공유]**&#x200B;를 선택하면 증명을 만들 때 이메일 알림이 전송됩니다. **[!UICONTROL 워크플로]** 섹션에서 **[!UICONTROL 자동화된 워크플로]**&#x200B;를 선택하면 증명이 사용자와 연결된 자동화된 워크플로의 단계에 들어오면 전자 메일 알림이 전송됩니다.

   * **사용자 지정 메시지 추가:** 알림에 사용자 지정 메시지를 포함하려면 이 옵션을 선택하십시오. 제목과 메시지 본문을 지정할 수 있습니다. 메시지 본문에는 굵게, 글머리 기호 및 하이퍼링크와 같은 서식 있는 텍스트 서식이 포함될 수 있습니다.

1. 다음 증명 설정 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">로그인 필요. 이 증명은 다른 사용자와 공유할 수 없습니다.</td> 
      <td> <p>이 옵션을 선택한 경우:</p> 
       <ul> 
        <li>사용자가 증명에 추가되지 않은 경우 해당 증명에 로그인하여 볼 수 없습니다.</li> 
        <li>구독을 활성화할 수 없습니다.</li> 
       </ul> 
       <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요</td> 
      <td><p>이 옵션을 선택한 경우 사용자는 증명을 결정할 때 사용자 이름과 암호를 지정해야 합니다.</p>
      <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 모든 결정을 내릴 때 증명 잠금</td> 
      <td> <p>이 설정을 사용하면 모든 결정이 내려진 후 증명 상태가 잠깁니다. 최종 승인자가 결정을 내리면 상태는 자동으로 잠금 해제에서 잠금으로 변경됩니다.</p> 
      <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">원본 파일 다운로드 허용</td> 
      <td> <p><strong></strong> 이 옵션을 선택하면 검토자는 증명을 만든 원본 파일을 다운로드할 수 있습니다.</p> <p>이 옵션을 선택 취소하면 다운로드 아이콘이 더 이상 표시되지 않습니다.</p>
      <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통한 증명 공유 허용</td> 
      <td><p>이 옵션을 선택하면 공용 URL 또는 포함 코드를 통해 증명을 공유할 수 있습니다.</p>
       <p>이 옵션은 기본적으로 활성화되어 있습니다.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통한 증명 구독 허용</td> 
      <td> <p>이 옵션을 선택하면 증명에 추가되지 않은 사람도 증명에 가입할 수 있습니다. 증명을 구독하는 사용자에게는 다음 설정에서 정의한 역할 및 이메일이 부여됩니다.</p> 
       <ul> 
        <li><strong>구독자 역할</strong>: 증명을 구독하는 모든 검토자에게 할당된 기본 증명 역할입니다.</li> 
        <li><strong>구독자에 대한 전자 메일 경고 설정</strong>: 증명을 구독하는 모든 검토자에게 할당되는 기본 전자 메일 경고입니다.</li> 
        <li> <p><strong>전자 메일 링크를 통한 증명 액세스 필요</strong>: 구독자가 증명에 대한 링크가 포함된 전자 메일을 받는지 여부를 구성합니다. <strong>전자 메일 없음</strong>(증명에 액세스하는 데 전자 메일 링크가 필요하지 않음), <strong>증명 알림 전자 메일 전용</strong>(구독자가 확인 없이 전자 메일을 통해 증명에 대한 링크를 받음) 또는 <strong>확인 및 증명 알림 전자 메일</strong>(구독자가 전자 메일을 통해 증명에 대한 링크를 받고 증명에 액세스하려면 링크를 클릭해야 함)을 선택할 수 있습니다. 이 옵션의 목적은 개인이 액세스 권한이 있는 올바른 이메일 주소를 입력했는지 확인하는 것입니다.</p> <p>참고: 증명에 자동화된 워크플로가 첨부된 경우 모든 구독에서 증명 소유자에게 확인 이메일을 생성하므로 대상자를 추가해야 하는 단계를 결정할 수 있습니다.</p> </li> 
       </ul> 
        <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 증명 만들기]**&#x200B;를 클릭합니다. Workfront은 선택한 문서 또는 웹 사이트에 대한 증명을 생성합니다.

   문서 업로드의 지연 시간은 파일 크기와 유형에 따라 다릅니다. 파일이 클수록 생성하는 데 시간이 오래 걸립니다. Workfront에서 파일을 계속 생성하면 페이지에서 이동할 수 있습니다. 최대 파일 업로드 크기는 4GB입니다.

## URL로 정적 증명 생성 {#generate-a-proof-for-a-url}

웹 사이트 URL을 사용하여 정적 증명을 생성할 수 있습니다.

>[!NOTE]
>
>[!DNL Workfront] 환경이 [!DNL Workfront Proof] Premium 계정과 통합된 경우에만 URL에 대한 대화형 증명을 생성할 수 있습니다. 이 섹션에서 설명한 대로 증명을 사용할 수 없는 경우 Workfront 관리자에게 문의하십시오.

1. **[!UICONTROL 새 증명]** 페이지를 열려면 다음 중 하나를 수행하십시오.

   * 페이지의 왼쪽 상단에 있는 **[!UICONTROL 새 증명]** 단추를 클릭합니다.
   * Dropzone(엔터프라이즈 기능)을 통해 제출합니다.

1. **새 증명** 페이지에서 **[!UICONTROL 파일 추가]** 영역에 증명을 만들 웹 사이트의 URL을 입력한 다음 키보드에서 **[!UICONTROL Enter]** 또는 **[!UICONTROL Return]**&#x200B;을 누릅니다.

1. (선택 사항) 이 프로세스를 반복하여 증명에 여러 웹 사이트를 추가합니다.

   ![proof_website.png](assets/proof-website-350x65.png)

1. **[!UICONTROL 파일 추가]** 영역에서 URL 오른쪽에 있는 **편집** 아이콘을 클릭하여 웹 사이트 증명 세부 정보를 엽니다.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. **[!UICONTROL 증명 이름]**&#x200B;을 입력하십시오. 기본적으로 증명 이름은 사이트 URL과 동일합니다.

1. 다음 **[!UICONTROL 사이트 콘텐츠 처리]** 옵션 중 하나를 선택하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">스크린샷 캡처</td> 
      <td>URL 앞 페이지의 정적 이미지에 대한 증명을 만듭니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">인터랙티브</td> 
      <td> <p>검토자가 사이트를 탐색하고 HTML5 이미지, Flash 요소 등을 볼 수 있도록 하는 증명을 만듭니다.</p> <p>대화형 증명을 만들려면 보안 프로토콜(https)을 사용하여 웹 사이트를 호스팅해야 합니다. 또한 iframe에 포함할 수 없는 웹 사이트는 대화형 증명으로 생성할 수 없습니다(iframe 포함 제한 사항은 포함하려는 웹 사이트에 의해 제어됨).</p> <p>초기 증명을 만든 후에는 후속 버전을 만들 때 이 설정을 변경할 수 없습니다.</p> <p>대화형 증명에 대한 자세한 내용은 <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">대화형 콘텐츠에 대한 증명 생성</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">스크린샷 해상도</td> 
      <td> <p>(이 옵션은 대화형 증명에 사용할 수 없습니다.) 콘텐츠가 표시되는 해상도를 조정하거나 여러 해상도를 선택할 수 있습니다.</p> <p>이를 통해 사용자는 증명을 검토하여 다양한 크기의 휴대폰, 태블릿 및 모니터와 같은 다양한 디바이스에 콘텐츠가 표시되는 방식을 확인할 수 있습니다.</p> <p>여러 개의 해상도를 선택하면 선택한 각 해상도에 대해 별도의 증명이 만들어집니다.</p> <p>사용자가 증명에 댓글을 달면 댓글에 현재 화면 해상도가 자동으로 표시되어 댓글이 어떤 해상도와 연관되어 있는지 다른 사용자가 알 수 있도록 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 페이지 찾기</td> 
      <td>(이 옵션은 대화형 증명에 사용할 수 없습니다.) 웹 사이트의 페이지를 탐색하려면 이 옵션을 선택합니다. 웹 사이트를 기본 페이지에서 최대 2단계까지 확장할 수 있습니다. 페이지 위로 마우스를 가져가면 페이지의 URL을 볼 수 있으며 증명하려는 페이지만 선택합니다. 선택하는 각 페이지는 기본적으로 개별 증명으로 만들어집니다. 또는 <strong>모든 호환 파일을 하나의 증명으로 결합</strong> 옵션을 활성화할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 증명 공유, 자동화된 워크플로 추가 또는 액세스 및 구독 설정 설정과 같은 고급 증명 옵션을 구성합니다. 이러한 옵션에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [ [!DNL Adobe Workfront] 내에서 증명 공유](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [ [!DNL Workfront Proof]에서 자동화된 워크플로를 사용하여 증명 설정](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [증명에 대한 액세스 및 구독 설정 구성](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. **[!UICONTROL 완료]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 증명 만들기]**&#x200B;를 클릭합니다.

## 대화형 콘텐츠에 대한 증명 생성 {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

대화형 콘텐츠에 대한 자세한 내용은 [대화형 콘텐츠 증명 개요](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)를 참조하십시오.

* [대화형 컨텐츠를 URL로 추가](#add-interactive-content-as-a-url)
* [대화형 컨텐츠를 ZIP 파일로 추가](#add-interactive-content-as-a-zip-file)

### 대화형 컨텐츠를 URL로 추가 {#add-interactive-content-as-a-url}

대화형 URL 증명을 추가하는 방법에 대한 자세한 내용은 [URL에 대한 증명 생성](#generate-a-proof-for-a-url)을 참조하십시오.

### 대화형 컨텐츠를 ZIP 파일로 추가 {#add-interactive-content-as-a-zip-file}

1. .zip 번들 파일을 만들어 콘텐츠를 준비합니다.

   .zip 번들 파일 사양에 대한 자세한 내용은 [대화형 콘텐츠 증명 개요](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)를 참조하십시오.

1. **[!UICONTROL 새 증명]** 페이지를 열려면 다음 중 하나를 수행하십시오.

   * 페이지의 왼쪽 상단에 있는 **[!UICONTROL 새 증명]** 단추를 클릭합니다.
   * Dropzone(엔터프라이즈 기능)을 통해 제출합니다.

1. **[!UICONTROL 새 증명]** 페이지에서 대화형 .zip 번들을 **[!UICONTROL 파일 추가]** 영역으로 끌어다 놓습니다.

1. (선택 사항) 증명 공유, 자동화된 워크플로 추가 또는 액세스 및 구독 설정 설정과 같은 고급 증명 옵션을 구성합니다. 이러한 옵션에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [ [!DNL Adobe Workfront] 내에서 증명 공유](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [증명에 대한 액세스 및 구독 설정 구성](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. **[!UICONTROL 증명 만들기]**&#x200B;를 클릭합니다. Workfront은 zip 파일의 증명을 생성합니다.

   문서 업로드의 지연 시간은 zip 파일 크기에 따라 다릅니다. Workfront에서 파일을 계속 생성하면 페이지에서 이동할 수 있습니다. 최대 파일 업로드 크기는 4GB입니다.
