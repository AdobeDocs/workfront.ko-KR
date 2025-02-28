---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Illustrator 및 InDesign용 Workfront 확장 사용
description: Workfront 확장 프로그램을 사용하여 Adobe Illustrator 및 Adobe InDesign에서 저장하고 만든 디지털 콘텐츠를 Workfront으로 내보낼 수 있습니다. 이를 통해 문서 검토 및 승인 프로세스를 가속화할 수 있습니다.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '3107'
ht-degree: 0%

---

# Illustrator 및 InDesign용 Workfront 확장 사용

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Illustrator 및 InDesign용 Workfront 확장을 [업데이트된 Creative Cloud 플러그인](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md)(으)로 바꾸는 중입니다. 2022년 말부터 이 확장 프로그램은 더 이상 지원되지 않으며 그대로 사용할 수 있습니다.

Workfront 확장 프로그램을 사용하여 Adobe Illustrator 및 Adobe InDesign에서 저장하고 만든 디지털 콘텐츠를 Workfront으로 내보낼 수 있습니다. 이를 통해 문서 검토 및 승인 프로세스를 가속화할 수 있습니다.

Workfront 확장은 다음 애플리케이션에서 Adobe Creative Cloud 2017 이상에 대해 지원됩니다.

* InDesign
* Illustrator
* Photoshop

  >[!NOTE]
  >
  >새로운 [Photoshop용 Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) 플러그인을 사용하는 것이 좋습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재: Pro 이상</p>
   또는
   <p>신규: 모든 플랜</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재: 작업 시간 이상</p>
   또는
   <p>새로운 기능: 표준</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Workfront 라이선스 외에 Adobe Creative Cloud 라이선스가 있어야 합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>상호 작용할 개체에 대한 액세스 권한을 편집합니다.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Illustrator 또는 InDesign에서 Workfront 확장 프로그램에 로그인합니다 {#log-in-to-workfront-extension-from-illustrator-or-indesign}

지원되는 Adobe 애플리케이션 중 하나에서 Workfront에 로그인하면 지원되는 모든 Adobe 애플리케이션에 로그인됩니다.

1. Workfront 확장을 사용할 Adobe 애플리케이션으로 이동합니다.

   지원되는 각 응용 프로그램에 대해 지원되는 형식 목록을 보려면 이 문서에서 [지원되는 내보낸 파일 형식](#supported-exported-file-formats)을 참조하십시오.

1. **창** > **확장** > Workfront을 클릭합니다.

1. (선택 사항) Workfront 패널을 Adobe 애플리케이션에서 표시할 위치로 드래그합니다.
1. 화면의 지침에 따라 Workfront에 로그인합니다.

   >[!NOTE]
   >
   >* Workfront은 사용자의 인증 및 권한 부여를 위해 대부분의 웹 기반 통합에서 사용하는 보안 표준인 OAuth 2.0을 사용하여 Adobe Creative Cloud에 연결합니다.
   >* Workfront 계정의 [도메인 또는 호스트]를 입력하라는 메시지가 표시되면 다음 형식을 사용하여 입력하십시오.`yourCompany'sDomain.my.workfront.com`. 회사의 도메인은 일반적으로 회사의 이름입니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

## Workfront 프로젝트, 작업 또는 문제에 파일 업로드 {#upload-a-file-to-a-workfront-project-task-or-issue}

컴퓨터 파일 시스템에서 파일을 업로드하거나 Adobe Creative Cloud 애플리케이션에서 현재 열려 있는 파일을 Workfront 프로젝트, 작업 또는 문제로 내보낼 수 있습니다. 

Adobe Creative Cloud에서 파일을 업로드하거나 내보낼 때 다음 사항을 고려하십시오.

* 액세스 수준에서는 Workfront에 문서를 업로드할 수 있어야 합니다. 자세한 내용은 [문서에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)를 참조하십시오.
* 문서를 원하는 항목에 업로드할 수 있는 권한이 있어야 합니다. 자세한 내용은 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.
* 선택한 Workfront 객체의 문서 영역에 파일이 업로드됩니다.
* Adobe Creative Cloud 응용 프로그램에서 문서를 기본 메뉴 ![기본 메뉴 아이콘](assets/main-menu-icon.png)의 문서 영역으로 내보낼 수 없습니다.

다음 섹션은 다음 사항을 설명합니다.

* [파일 업로드](#upload-a-file)
* [현재 Illustrator 또는 InDesign에서 열려 있는 파일을 내보냅니다](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Illustrator 또는 InDesign에서 파일의 새 버전 업로드](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### 파일 업로드 {#upload-a-file}

Adobe Creative Cloud 애플리케이션을 종료하지 않고 프로젝트, 작업 또는 문제에 파일을 업로드할 수 있습니다.

1. Adobe Creative Cloud 애플리케이션을 열 때 Workfront 확장이 표시되지 않으면 **Window** > **확장** > **Workfront**&#x200B;을(를) 클릭합니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

1. 파일을 업로드할 프로젝트, 작업 또는 문제의 이름을 클릭합니다.

   **검색** 상자에 이름을 입력하고 **검색** 상자 오른쪽의 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**&#x200B;를 선택하여 검색할 수 있습니다. 작업 항목의 이름이 목록에 없으면 **Enter**&#x200B;를 눌러 보기 액세스 권한이 있는 모든 Workfront 항목을 검색합니다.

1. Workfront 확장의 오른쪽 아래 모서리에서 **선택**&#x200B;을 클릭합니다.
1. **형식을 선택하려면 클릭** 드롭다운 메뉴에서 Workfront에서 파일을 저장할 형식을 클릭합니다.

   지원되는 각 응용 프로그램에 대해 지원되는 형식 목록을 보려면 이 문서에서 [지원되는 내보낸 파일 형식](#supported-exported-file-formats)을 참조하십시오.

1. (조건부) 파일을 업로드할 작업 항목에 문서 폴더가 있는 경우 **문서 폴더를 선택하려면 클릭** 필드에서 문서 폴더를 선택한 다음 **선택**&#x200B;을 클릭합니다.

1. **로컬 파일 업로드**&#x200B;를 클릭합니다.
1. **파일 열기** 상자에서 파일 시스템에서 파일을 찾은 다음 **열기**&#x200B;를 클릭합니다.

1. (선택 사항) 파일의 새 이름을 입력합니다.

   ![파일 이름 바꾸기](assets/rename-file-uploading.png)

1. **업로드**&#x200B;를 클릭합니다.

   이제 Workfront에서 선택한 프로젝트, 작업 또는 문제에 대한 문서 영역에 문서가 나열됩니다.

1. (선택 사항) 문서 이름을 클릭하여 Workfront에서 문서 세부 정보 페이지를 엽니다.

   Workfront이 새 브라우저 탭에서 열립니다.

### 현재 Illustrator 또는 InDesign에서 열려 있는 파일 내보내기 {#export-a-file-currently-open-in-illustrator-or-indesign}

1. 지원되는 Adobe Creative Cloud 애플리케이션에서 Workfront으로 내보낼 파일을 엽니다.
1. Workfront 확장이 표시되지 않으면 **창** > **확장** > **Workfront**&#x200B;을 클릭합니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

1. 파일을 내보낼 프로젝트, 작업 또는 문제의 이름을 클릭합니다.

   **검색** 상자에 이름을 입력하고 **검색** 상자 오른쪽의 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**&#x200B;를 선택하여 검색할 수 있습니다. 작업 항목의 이름이 목록에 없으면 **Enter**&#x200B;를 눌러 보기 액세스 권한이 있는 모든 Workfront 항목을 검색합니다.

1. **형식을 선택하려면 클릭** 드롭다운 메뉴에서 Workfront에서 파일을 저장할 형식을 클릭합니다.

   지원되는 각 응용 프로그램에 대해 지원되는 형식 목록을 보려면 이 문서에서 [지원되는 내보낸 파일 형식](#supported-exported-file-formats)을 참조하십시오.

1. (조건부) 파일을 업로드할 작업 항목에 문서 폴더가 있는 경우 **문서 폴더를 선택하려면 클릭** 필드에서 문서 폴더를 선택한 다음 **선택**&#x200B;을 클릭합니다.
1. (선택 사항) 문서의 이름을 바꾸려면 문서 이름을 클릭하고 새 이름을 입력합니다.

   ![내보낼 때 문서 이름 바꾸기](assets/rename-doc-exporting.png)

1. **내보내기**&#x200B;를 클릭합니다.

   문서를 Workfront으로 성공적으로 내보냈음을 확인하는 메시지가 표시됩니다.

   Workfront에서 문서는 Workfront에서 지정한 객체의 문서 영역에 나열됩니다.

1. (선택 사항) Workfront에서 액세스하려면 문서의 이름을 클릭합니다.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront이 새 브라우저 탭에서 열립니다.

### Illustrator 또는 InDesign에서 파일의 새 버전 업로드 {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. 지원되는 Adobe 애플리케이션에서 작업 중인 파일을 Workfront의 새 파일 버전으로 내보내려면 Adobe 애플리케이션에서 파일을 엽니다.
1. Workfront 확장이 표시되지 않으면 **창** > **확장** > **Workfront**&#x200B;을 클릭합니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

1. 기존 문서가 나열된 프로젝트, 작업 또는 문제의 이름을 클릭합니다.

   **검색** 상자에 이름을 입력하고 **검색** 상자 오른쪽의 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**&#x200B;를 선택하여 검색할 수 있습니다. 작업 항목의 이름이 목록에 없으면 **Enter**&#x200B;를 눌러 보기 액세스 권한이 있는 모든 Workfront 항목을 검색합니다.

   Adobe 애플리케이션에서 업로드했는지 여부에 관계없이 프로젝트, 작업 또는 문제에 업로드된 모든 문서가 목록에 표시됩니다.

1. **형식을 선택하려면 클릭** 드롭다운 메뉴에서 Workfront에서 파일을 저장할 형식을 클릭합니다.

   Adobe 애플리케이션에서 연 파일을 내보내는 경우 필요합니다. 지원되는 각 응용 프로그램에 대해 지원되는 형식 목록을 보려면 이 문서에서 [지원되는 내보낸 파일 형식](#supported-exported-file-formats)을 참조하십시오.

1. Adobe 응용 프로그램에서 연 파일을 선택한 Workfront 문서의 새 버전으로 내보내는 경우 **내보내기**&#x200B;를 클릭합니다.

   또는

   컴퓨터 파일 시스템에서 파일을 선택한 Workfront 문서의 새 버전으로 업로드하려면 **로컬 파일 업로드**&#x200B;를 클릭하고 나타나는 상자에서 파일을 찾은 다음 **열기**&#x200B;를 클릭하고 **업로드**&#x200B;를 클릭합니다.

1. (선택 사항) Workfront에서 새 버전을 보려면 문서 이름을 클릭합니다.

   >[!NOTE]
   >
   >Workfront의 문서 이름은 기본적으로 채워지며 편집할 수 없습니다. 업로드하거나 새 버전으로 내보내는 파일의 이름도 변경되지 않습니다.
   >
   >
   >![문서 이름을 변경할 수 없습니다](assets/doc-name-cant-be-changed.png)

## Illustrator 또는 InDesign의 Workfront 문서에 대한 댓글 {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Adobe 애플리케이션 내에서 Workfront 문서에 직접 주석을 추가할 수 있습니다. Workfront에서 문서의 업데이트 영역과 문서가 저장된 Workfront 항목에 대한 업데이트 영역에 주석이 표시됩니다.

1. 지원되는 Adobe 애플리케이션 중 하나를 엽니다.
1. Workfront 확장이 표시되지 않으면 **창** > **확장** > **Workfront**&#x200B;을 클릭합니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

1. 기존 문서가 나열된 프로젝트, 작업 또는 문제를 클릭합니다.

   **검색** 상자에 이름을 입력하고 **검색** 상자 오른쪽의 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**&#x200B;를 선택하여 검색할 수 있습니다. 작업 항목의 이름이 목록에 없으면 **Enter**&#x200B;를 눌러 보기 액세스 권한이 있는 모든 Workfront 항목을 검색합니다.

1. 기존 문서의 이름을 클릭한 다음 Workfront 확장의 오른쪽 아래 모서리에 있는 **선택**&#x200B;을 클릭합니다.
1. **댓글** 탭을 클릭한 다음 상자에 업데이트를 입력하십시오.

1. (선택 사항) 댓글에 다른 Workfront 사용자 또는 팀을 포함하려면 **사람 또는 팀에 알림** 상자에 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.
1. (선택 사항) 문서에 대한 승인을 요청하려면 **승인 요청 만들기**&#x200B;를 선택합니다.
1. **업데이트**&#x200B;를 클릭합니다.

   문서의 업데이트 탭에 업데이트가 게시됩니다. 댓글에 포함하는 Workfront 사용자는 인앱 알림을 받으며, Workfront이 구성되는 방식에 따라 이메일 알림을 받을 수도 있습니다.

   Workfront 내의 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)를 참조하십시오.

   전자 메일 알림 수신에 대한 자세한 내용은 [Adobe Workfront 알림](../../workfront-basics/using-notifications/wf-notifications.md)을 참조하세요.

## Illustrator 또는 InDesign에서 문서 승인 요청

Adobe 애플리케이션에서 직접 Workfront 문서 승인을 요청할 수 있습니다.

다음 엔티티에서 문서 승인을 요청할 수 있습니다.

* Workfront 사용자
* Workfront 계정이 없는 외부 사용자

다음과 같은 방법으로 Adobe 애플리케이션에서 문서에 대한 승인을 요청할 수 있습니다.

* 승인자를 문서에 첨부합니다.
* 문서에 댓글을 달거나 댓글을 달면 해당 사용자에게 알리고 해당 문서에 승인자로 첨부합니다.

  문서에 댓글을 달 때 승인을 요청하는 방법에 대한 자세한 내용은 이 문서의 [Illustrator 또는 InDesign의 Workfront 문서에 대한 댓글](#comment-on-a-workfront-document-from-illustrator-or-indesign) 섹션을 참조하십시오.

Adobe 애플리케이션에서 문서에 대한 승인을 요청하려면

1. 지원되는 Adobe 애플리케이션 중 하나를 엽니다.
1. Workfront 확장이 표시되지 않으면 **창** > **확장** > **Workfront**&#x200B;을 클릭합니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

1. 기존 문서가 나열된 프로젝트, 작업 또는 문제를 클릭한 다음 기존 문서의 이름을 클릭합니다.

   **검색** 상자에 이름을 입력하고 **검색** 상자 오른쪽의 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**&#x200B;를 선택하여 검색할 수 있습니다. 작업 항목의 이름이 목록에 없으면 **Enter**&#x200B;를 눌러 보기 액세스 권한이 있는 모든 Workfront 항목을 검색합니다.

1. 기존 문서의 이름을 클릭한 다음 Workfront 확장의 오른쪽 아래 모서리에 있는 **선택**&#x200B;을 클릭합니다.
1. **승인** 탭을 클릭합니다.
1. 승인자를 추가하려면 **이름 상자 입력**&#x200B;에서 다음 중 하나를 실행하십시오.

   * 승인자의 이름을 입력한 다음 목록에 표시될 때 선택합니다.

     ![문서 승인자 추가](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * 외부 사용자의 이메일 주소를 입력합니다.

1. **승인 요청**&#x200B;을 클릭합니다.

   댓글에 포함하거나 승인자로 추가하는 Workfront 사용자는 인앱 알림을 받으며, Workfront의 구성 방법에 따라 이메일 알림을 받을 수도 있습니다.\
   외부 사용자는 승인을 결정할 수 있는 위치에서 이메일 알림을 받습니다.

   Workfront의 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)를 참조하십시오. 이메일 알림 수신에 대한 자세한 내용은 [Adobe Workfront 알림](../../workfront-basics/using-notifications/wf-notifications.md)을 참조하세요.

## Illustrator 또는 InDesign에서 증명 생성 {#generate-a-proof-from-illustrator-or-indesign}

조직에서 자동화된 워크플로 템플릿을 사용하는 경우 애플리케이션을 종료하지 않고 Adobe 애플리케이션에서 만든 문서에 대한 증명을 생성할 수 있습니다. 증명 만들기에 대한 자세한 내용은 [증명 만들기](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md)를 참조하십시오. 자동화된 워크플로 템플릿에 대한 자세한 내용은 [자동화된 워크플로 개요](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)에서 [자동화된 워크플로 템플릿](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate)을 참조하십시오.

1. 지원되는 Adobe 애플리케이션 중 하나를 엽니다.
1. Workfront 확장이 표시되지 않으면 **창** > **확장** > Workfront을 클릭합니다.

   프로젝트가 현재 상태인 경우 사용자에게 할당된 작업 항목 목록이 표시됩니다. 목록이 표시되지 않으면 Workfront에 로그인합니다.

   개인 작업은 **프로젝트 없음** 아래에 나열됩니다.

1. 문서가 이미 Workfront에 업로드되어 있는 경우, 문서가 나열된 Workfront 확장 기능에서 프로젝트, 작업 또는 문제를 선택한 다음 문서 이름을 클릭합니다.

   또는

   이 문서의 [Workfront 프로젝트, 작업 또는 문제에 파일 업로드](#upload-a-file-to-a-workfront-project-task-or-issue) 섹션에 설명된 대로 Adobe 문서를 Workfront 개체에 업로드한 다음 문서 이름을 클릭합니다.

1. **형식을 선택하려면 클릭** 드롭다운 메뉴에서 Workfront에서 파일을 저장할 형식을 클릭합니다.

   이 형식의 다음 단계에서 증명 기능을 활성화한 후에는 일부 형식을 사용할 수 없습니다. 자세한 내용은 이 문서에서 [지원되는 내보낸 파일 형식](#supported-exported-file-formats)을 참조하십시오.

1. 활성화하려면 **새 증명으로 업로드**&#x200B;를 클릭하세요.
1. 직원들이 문서를 검토할 때 사용할 **워크플로 템플릿**&#x200B;을(를) 선택하십시오.

   [자동화된 워크플로 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)에 설명된 대로 Workfront 관리자가 자동화된 워크플로 템플릿을 설정합니다. 질문이 있는 경우 관리자에게 문의하십시오.

   1. 워크플로 템플릿의 모든 단계에 최소 한 명 이상의 **새 수신자**&#x200B;를 추가하십시오.

      표시되는 드롭다운 목록에 이름이 표시되면 이름을 입력하고 선택할 수 있습니다.

   1. 추가하는 각 받는 사람에 대해 **증명 역할** 및 **전자 메일 경고**&#x200B;의 빈도를 지정하십시오.

   1. (선택 사항) **전자 메일 알림** 섹션에서 추가한 모든 증명 수신자에게 증명에 대한 선택적 사용자 지정 메시지가 포함된 전자 메일 알림을 전송할지 여부를 선택합니다.

1. **증명 만들기**&#x200B;를 클릭합니다.

   증명 작성 프로세스의 진행 상황을 확인할 수 있습니다. 생성이 완료되면 경고가 나타납니다. 증명을 만든 작업을 열 수 있으며 해당 작업이 여기에 나열됩니다.

## Illustrator 또는 InDesign을 종료하지 않고 새 증명 버전 업로드

1. 증명이 있는 기존 문서를 클릭한 다음 오른쪽 하단의 **선택**&#x200B;을 클릭합니다.
1. **새 증명 버전으로 업로드**&#x200B;를 클릭하여 사용하도록 설정합니다.
1. (선택 사항) 직원들이 새 버전을 검토할 때 사용할 **워크플로 템플릿**&#x200B;을(를) 선택합니다.

   다른 템플릿을 선택하지 않으면 이전 버전에 대해 선택한 템플릿이 계속 적용됩니다. 또한 이전 버전의 템플릿을 수정한 경우에는 새 버전에 변경 사항이 적용됩니다.

   [자동화된 워크플로 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)에 설명된 대로 Workfront 관리자가 자동화된 워크플로 템플릿을 설정합니다. 질문이 있는 경우 관리자에게 문의하십시오.

   1. 워크플로 템플릿의 모든 단계에 최소 한 명 이상의 **새 수신자**&#x200B;를 추가하십시오.

      표시되는 드롭다운 목록에 이름이 표시되면 이름을 입력하고 선택할 수 있습니다.

   1. 추가하는 각 받는 사람에 대해 **증명 역할** 및 **전자 메일 경고**&#x200B;의 빈도를 지정하십시오.
   1. (선택 사항) **전자 메일 알림** 섹션에서 추가한 모든 증명 수신자에게 증명에 대한 선택적 사용자 지정 메시지가 포함된 전자 메일 알림을 전송할지 여부를 선택합니다.

1. **새 증명 버전 만들기**&#x200B;를 클릭합니다.

   증명 작성 프로세스의 진행 상황을 확인할 수 있습니다. 생성이 완료되면 경고가 나타납니다. 증명을 만든 작업을 열 수 있으며 해당 작업이 여기에 나열됩니다.

## Workfront 확장에서 로그아웃

1. Adobe 응용 프로그램에서 **창** > **확장** > **Workfront**&#x200B;을 클릭합니다.

1. 패널의 오른쪽 상단에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.

1. (선택 사항) 간단한 설문 조사를 열고 Workfront for Adobe Creative Cloud에 대한 피드백을 Workfront에 보내려면 **피드백**&#x200B;을 클릭하십시오.
1. **로그아웃**&#x200B;을 클릭합니다.\
   로그인 화면이 표시됩니다. 로그인에 대한 자세한 내용은 이 문서에서 [Illustrator 또는 InDesign에서 Workfront 확장 로그인](#log-in-to-workfront-extension-from-illustrator-or-indesign)을 참조하십시오.

## 지원되는 내보낸 파일 형식 {#supported-exported-file-formats}

* [Adobe InDesign에서 지원되는 내보낸 파일 형식](#supported-exported-file-formats-for-adobe-indesign)
* [Adobe Illustrator에서 지원되는 내보낸 파일 형식](#supported-exported-file-formats-for-adobe-illustrator)

### Adobe InDesign에서 지원되는 내보낸 파일 형식  {#supported-exported-file-formats-for-adobe-indesign}

Workfront은 InDesign에서 Workfront으로 파일을 내보내기 위해 다음과 같은 파일 형식을 지원합니다.

* EPS - 캡슐화된 PostScript
* EPUB - 고정된 레이아웃 전자 발행
* EPUB - 리플로우 가능한 전자 발행물 &#42;
* HTML - 하이퍼텍스트 마크업 언어
* IDML - InDesign 마크업 언어 &#42;
* JPG, JPEG - Joint Photography Experts Group
* PDF - Adobe 휴대용 문서 파일
* PNG - 이동식 네트워크 그래픽
* SWF - Flash Player &#42;
* XML - Extensible Markup Language &#42;

&#42; **새 증명 업로드**&#x200B;를 사용하는 경우에는 이 파일 형식을 사용할 수 없습니다(이 옵션에 대한 자세한 내용은 이 문서의 [Illustrator 또는 InDesign에서 증명 생성](#generate-a-proof-from-illustrator-or-indesign)을 참조하십시오). **새 증명 업로드**&#x200B;를 사용하기 전에 이 파일 형식을 이미 선택한 경우, 시스템이 파일 형식을 PDF으로 변경합니다. 목록에서 다른 형식을 선택할 수 있습니다.

### Adobe Illustrator에서 지원되는 내보낸 파일 형식  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront은 Illustrator에서 Workfront으로 파일을 내보내기 위해 다음과 같은 파일 형식을 지원합니다.

* DWG - AutoCAD 드로잉, AutoCAD 교환 파일 &#42;
* JPG, JPEG - Joint Photography Experts Group
* PNG - 이동식 네트워크 그래픽
* PSD - Photoshop 문서
* SWF - Flash Player &#42;
* TIFF - 태그가 지정된 이미지 파일 형식

&#42; **새 증명 업로드**&#x200B;를 사용하는 경우에는 이 파일 형식을 사용할 수 없습니다(이 옵션에 대한 자세한 내용은 이 문서의 [Illustrator 또는 InDesign에서 증명 생성](#generate-a-proof-from-illustrator-or-indesign)을 참조하십시오). **새 증명 업로드**&#x200B;를 사용하기 전에 이 파일 형식을 이미 선택한 경우, 시스템이 파일 형식을 PNG로 변경합니다. 목록에서 다른 형식을 선택할 수 있습니다.
