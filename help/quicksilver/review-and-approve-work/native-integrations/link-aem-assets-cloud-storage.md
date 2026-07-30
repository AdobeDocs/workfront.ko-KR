---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Experience Manager Assets의 컨텐츠 및 폴더를 Adobe 클라우드 스토리지와 연결
description: 조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Experience Manager Assets의 컨텐츠 및 폴더를 문서를 지원하는 모든 Adobe Workfront 개체에 연결할 수 있습니다.
author: Courtney
source-git-commit: 805cc8dfaa17438eb1d454d00d5f7986540379b3
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 2%

---

# Experience Manager Assets의 컨텐츠 및 폴더를 Adobe 클라우드 스토리지와 연결

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Experience Manager Assets에서 Workfront으로 컨텐츠 및 폴더를 연결할 수 있습니다. 연결되면 Workfront에서 컨텐츠를 보고 관리할 수 있으며, Experience Manager Assets의 컨텐츠에 대한 모든 변경 사항이 Workfront에 반영됩니다.

>[!IMPORTANT]
>
>조직에서 GenAI 라이더 계약에 서명하는 것을 거부하는 경우 Content Advisor를 사용하여 Experience Manager Assets에서 에셋 및 폴더를 선택할 수는 있지만 AI 검색, 스마트 제안 또는 캠페인 개요 분석과 같은 AI 기반 기능에 액세스할 수는 없습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 제품</td> 
   <td>Experience Manager as a Cloud Service이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 권한</td> 
    <td>폴더에 대한 쓰기 액세스 권한이 있어야 합니다.</td> 
   </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에:

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Frame.io 통합에 Adobe Experience Manager 사용](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)을 참조하십시오.

* 스마트 제안 또는 Campaign Brief 기능을 사용하려면 GenAI 라이더에 서명해야 합니다. 자세한 내용은 [콘텐츠 관리자를 사용하여 Adobe 응용 프로그램의 AEM 콘텐츠에 액세스](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)를 참조하십시오.

## Experience Manager Assets에서 컨텐츠 연결

컨텐츠를 연결하려면 다음 작업을 수행하십시오.

1. 콘텐츠를 연결하려는 Workfront 개체로 이동합니다.
1. 왼쪽 패널에서 **문서** 섹션을 클릭합니다.
1. 페이지 오른쪽에서 **새로 만들기**&#x200B;를 클릭한 다음 **AEM 파일**&#x200B;을 클릭하여 개별 자산을 연결합니다.
   ![문서 영역에 AEM 파일 추가](assets/aem-files.png)

1. Content Advisor를 사용하여 다음과 같은 작업을 수행할 수 있습니다.

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>AI 검색을 사용하여 자산을 검색합니다.</strong> 쿼리의 의미와 의도를 이해하고 여러 언어, 오타 및 동의어를 지원하는 AI 기반 검색을 사용합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">스마트 자산 검색용 AI 검색</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>컨텍스트 및 의도를 기반으로 스마트 제안을 봅니다.</strong> 호스트 Adobe 애플리케이션의 컨텍스트 인식 권장 사항을 사용하여 콘텐츠 요구 사항에 맞는 에셋을 검색합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">컨텍스트 및 의도에 따른 스마트 제안</a>을 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>관련 에셋을 검색하려면 캠페인 개요를 업로드하십시오.</strong> PDF, DOCX 또는 TXT 캠페인 개요 문서를 업로드하여 Content Advisor가 이를 분석하고 관련 에셋을 추천할 수 있도록 합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">관련 자산을 검색하는 캠페인 개요</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>Dynamic Media 에셋 렌디션을 보고 선택합니다.</strong> 이미지 사전 설정, 스마트 자르기 및 형식 유형을 포함하여 채널에 최적화된 렌디션을 찾아보고 Dynamic Media 수정자를 적용하여 조정을 실시간으로 미리 볼 수 있습니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">사용할 수 있는 Dynamic Media 에셋 렌디션</a>을 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>변환에 Dynamic Media 수정자를 적용합니다.</strong> 수정자를 추가하여 자산 렌디션을 실시간으로 변형하고 호스트 애플리케이션의 렌디션을 선택하기 전에 결과를 미리 봅니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">사용할 수 있는 Dynamic Media 에셋 렌디션</a>을 참조하십시오.</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>자산 메타데이터에 액세스합니다.</strong> Assets 보기와 일치하는 제목, 설명, 형식, 크기 및 기타 메타데이터 탭(제품, 캠페인, 태그)과 같은 자산 속성을 검토합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Assets 보기와 일치하는 자산 메타데이터에 액세스</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>미리 정의된 필터를 사용하여 자산을 필터링합니다.</strong> 파일 유형, 파일 형식, 에셋 상태, 파일 크기, 이미지 너비, 이미지 높이, 수정한 날짜 및 만든 날짜와 같은 필터를 사용하여 에셋 결과를 구체화합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Assets 보기와 일치하는 필터에 액세스</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>검색을 저장하고 다시 사용합니다.</strong> 검색어와 필터 옵션을 지정하여 저장된 검색을 작성한 다음 Experience Manager Assets 및 기타 Adobe 애플리케이션에서 재사용합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">최근 검색 및 저장된 검색 다시 사용</a>을 참조하세요.</td>
      </tr>
      <tr>
         <td><strong>컬렉션 간 및 컬렉션 내 자산을 검색합니다.</strong> 모든 컬렉션에서 에셋 또는 컬렉션을 검색하거나 특정 컬렉션으로 검색을 제한합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">컬렉션 간 및 컬렉션 내 자산 검색</a>을 참조하십시오.</td>
      </tr>
   </tbody>
   </table>

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## 고려 사항

* 연결된 AEM 자산에 대해서는 검토 및 승인 워크플로가 지원되지 않습니다.
* 메타데이터 필드는 자산을 Workfront에서 Experience Manager Assets으로 보낼 때 먼저 매핑됩니다. Workfront 관리자가 오브젝트 메타데이터 동기화를 활성화한 경우 두 애플리케이션에서 변경된 필드가 최신 상태로 유지됩니다.
