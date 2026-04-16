---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets에서 제공하는 Content Advisor를 사용하여 컨텐츠 및 폴더 연결
description: 컨텐츠 권고자를 사용하여 Experience Manager Assets의 컨텐츠나 폴더를 문서를 지원하는 모든 Adobe Workfront 개체에 연결할 수 있습니다. Content Advisor는 상황에 맞는 지능적인 검색 기능을 Workfront에 바로 제공하여 관련성이 높은 승인된 컨텐츠를 신속하게 찾을 수 있도록 지원합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 2%

---

# Experience Manager Assets의 Content Advisor를 사용하여 콘텐츠 및 폴더 연결

Content Advisor는 상황에 맞는 지능적인 검색 기능을 Workfront에 바로 제공하여 상황에 따라 관련성이 있고 승인된 콘텐츠를 신속하게 찾을 수 있도록 지원합니다. 스마트 제안, Dynamic Media 렌디션 및 세부 에셋 메타데이터와 같은 기능을 통해 Workfront을 종료하지 않고도 콘텐츠를 효율적으로 평가하고 재사용할 수 있으며, 브랜드 일관성을 유지하면서 콘텐츠 생성 시간을 단축할 수 있습니다.

컨텐츠 권고자를 사용하여 Experience Manager Assets의 컨텐츠와 폴더를 Workfront에 연결할 수 있습니다. 연결되면 Workfront에서 컨텐츠를 보고 관리할 수 있으며, Experience Manager Assets의 컨텐츠에 대한 모든 변경 사항이 Workfront에 반영됩니다.

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
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</td> 
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

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)을 참조하십시오.

* 스마트 제안 또는 Campaign Brief 기능을 사용하려면 GenAI 라이더에 서명해야 합니다. 자세한 내용은 [콘텐츠 관리자를 사용하여 Adobe 응용 프로그램의 AEM 콘텐츠에 액세스](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)를 참조하십시오.



## 콘텐츠 관리자를 사용하여 Experience Manager Assets의 콘텐츠 연결

이제 콘텐츠 관리자를 사용하여 Workfront 내에서 직접 Experience Manager Assets의 콘텐츠를 연결할 수 있습니다. Assets Essentials에는 콘텐츠 관리자를 사용할 수 없습니다.

컨텐츠를 연결하려면 다음 작업을 수행하십시오.

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. **새로 추가**&#x200B;를 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택하십시오.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Experience Manager Assets에 대해서는 구체적으로 언급하지 않을 수 있습니다.

1. Content Advisor를 사용하여 다음과 같은 작업을 수행할 수 있습니다.


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>AI 검색을 사용하여 자산을 검색합니다.</strong> 쿼리 뒤에 있는 의미와 의도를 이해하고 여러 언어, 오타 및 동의어를 지원하는 AI 기반 검색을 사용합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">스마트 자산 검색용 AI 검색</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>컨텍스트 및 의도를 기반으로 스마트 제안을 봅니다.</strong> 호스트 Adobe 애플리케이션의 컨텍스트 인식 권장 사항을 사용하여 콘텐츠 요구 사항에 맞는 에셋을 검색합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">컨텍스트 및 의도에 따른 스마트 제안</a>을 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>관련 에셋을 검색하려면 캠페인 개요를 업로드하십시오.</strong> Content Advisor에서 PDF, DOCX 또는 TXT 캠페인 개요 문서를 업로드하여 이를 분석하고 관련 에셋을 추천할 수 있습니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">관련 자산을 검색하는 캠페인 개요</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>Dynamic Media 에셋 렌디션을 보고 선택합니다.</strong> 이미지 사전 설정, 스마트 자르기 및 형식 유형을 포함하여 채널에 최적화된 렌디션을 찾아보고 Dynamic Media 수정자를 적용하여 실시간으로 조정을 미리 봅니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">사용할 수 있는 Dynamic Media 에셋 렌디션</a>을 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>변환에 Dynamic Media 수정자를 적용합니다.</strong> 수정자를 추가하여 자산 렌디션을 실시간으로 변환하고 호스트 응용 프로그램의 렌디션을 선택하기 전에 결과를 미리 봅니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">사용할 수 있는 Dynamic Media 에셋 렌디션</a>을 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>콘텐츠 조각을 검색하고 찾아봅니다.</strong> 콘텐츠 조각을 검색하고, 실시간 썸네일 미리 보기를 보고, 상태(초안, 수정됨 또는 게시됨)를 확인하고, 세부 속성, 참조 및 변형을 검사합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">콘텐츠 조각 검색</a>을 참조하세요.</td>
      </tr>
      <tr>
         <td><strong>자산 메타데이터에 액세스합니다.</strong> 제목, 설명, 형식, 크기 및 Assets 보기와 일치하는 기타 메타데이터 탭(제품, 캠페인, 태그)과 같은 자산 속성을 검토합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Assets 보기와 일치하는 자산 메타데이터에 액세스</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>미리 정의된 필터를 사용하여 자산을 필터링합니다.</strong> 파일 형식, 파일 형식, 에셋 상태, 파일 크기, 이미지 너비, 이미지 높이, 수정한 날짜 및 만든 날짜와 같은 필터를 사용하여 에셋 결과를 구체화합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Assets 보기와 일치하는 필터에 액세스</a>를 참조하십시오.</td>
      </tr>
      <tr>
         <td><strong>검색을 저장하고 다시 사용합니다.</strong> 검색어와 필터 옵션을 지정하여 저장된 검색을 만든 다음 Experience Manager Assets 및 기타 Adobe 응용 프로그램에서 다시 사용합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">최근 검색 및 저장된 검색 다시 사용</a>을 참조하세요.</td>
      </tr>
      <tr>
         <td><strong>컬렉션에서 에셋을 검색합니다.</strong> 모든 컬렉션에서 에셋 또는 컬렉션을 검색하거나 특정 컬렉션으로 검색을 제한합니다.</td>
         <td>자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">컬렉션 간 및 컬렉션 내 자산 검색</a>을 참조하십시오.</td>
      </tr>
   </tbody>
   </table>


### Experience Manager Assets에서 콘텐츠 관리자를 사용하여 새 버전 연결

Experience Manager Assets 또는 Assets Essentials에서 새 콘텐츠를 가져와서 기존 에셋에 새 버전으로 추가할 수 있습니다. 문서가 이미 연결되어 있고 Experience Manager Assets 또는 Assets Essentials에 새 버전이 추가된 경우 새 버전이 Workfront에 자동으로 표시됩니다.

새 버전을 연결하려면 다음을 수행하십시오.

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. 새 버전으로 바꿀 자산을 선택합니다. 연결된 폴더에 자산의 새 버전을 만들 수 없습니다.
1. **새로 추가** > **버전**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Experience Manager Assets에 대해 특별히 언급하지 않을 수 있습니다.

1. 연결할 콘텐츠를 선택합니다.

   * Experience Manager Assets 또는 Assets Essentials에서 에셋, 폴더 또는 컬렉션을 찾아보려면 Assets 탭을 선택합니다.

     ![콘텐츠 관리자](assets/content-advisor-full.png)

   * 컨텐츠 조각은 버전을 지원하지 않습니다. 컨텐츠 조각을 선택하면 새 버전이 만들어지는 대신 새 버전이 기존 컨텐츠 조각을 대체합니다.

1. **선택**&#x200B;을 클릭합니다.

## Experience Manager Assets의 폴더를 컨텐츠 권고자와 연결

폴더 내의 개별 에셋을 볼 수 있는 권한은 Experience Manager Assets 권한에 따라 다릅니다.

폴더를 연결하려면 다음 작업을 수행하십시오.

1. 폴더를 원하는 Workfront의 **문서** 영역으로 이동합니다.
1. **새로 추가**&#x200B;를 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택하십시오.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Experience Manager Assets에 대해 특별히 언급하지 않을 수 있습니다.

1. **Assets** > **파일 및 폴더**&#x200B;를 클릭합니다.

1. **필터** 아이콘을 클릭한 다음 **자산 유형** 섹션에서 **폴더**&#x200B;를 선택합니다.

1. 연결할 폴더를 선택합니다.

1. **선택**&#x200B;을 클릭합니다.

## 고려 사항

* Adobe 엔터프라이즈 스토리지를 사용하는 객체에는 컨텐츠 권고자 기능을 사용할 수 없습니다. 조직에서 Adobe Enterprise Storage를 사용하는 경우 Experience Manager Assets 또는 Assets Essentials의 에셋 및 폴더를 계속 연결할 수 있지만 AI 검색, 스마트 제안 또는 Dynamic Media 렌디션과 같은 Content Advisor 기능에 액세스할 수는 없습니다. 자세한 내용은 [Frame.io 통합에 Adobe Experience Manager 사용](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)을 참조하십시오.

* Assets Essentials에는 콘텐츠 관리자 기능을 사용할 수 없습니다. Assets Essentials에서 에셋 및 폴더를 연결하려면 [Experience Manager Assets Essentials에서 에셋 및 폴더 연결](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md)을 참조하십시오.

* 메타데이터 필드는 자산을 Workfront에서 Experience Manager Assets으로 보낼 때 먼저 매핑됩니다. Workfront 관리자가 오브젝트 메타데이터 동기화를 활성화한 경우 두 애플리케이션에서 변경된 필드가 최신 상태로 유지됩니다.
