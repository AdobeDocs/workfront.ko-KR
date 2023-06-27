---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: SDL 관리 번역 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서 SDL Managed Translation 계정을 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오, 다음을 연결할 수 있습니다 [!DNL SDL Managed Translation] 여러 타사 애플리케이션 및 서비스에 대한 계정.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
  <td> <p>[!UICONTROL Pro] 이상</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] 모듈

>[!NOTE]
>
>호출 작업 시간 제한 [!DNL SDL Managed Translation] 은(는) **120초**.

### 파일

#### [!UICONTROL 번역된 파일 다운로드]

이 모듈은 지정된 프로젝트 내에 포함된 번역된 단일 파일의 콘텐츠를 검색합니다. 요청된 파일이 아직 다운로드 상태가 아닌 경우 파일의 콘텐츠가 아직 완전히 번역되지 않았을 수 있습니다. 파일이 다운로드 상태이고 성공적으로 검색한 경우 다음을 사용하여 파일을 완료로 표시해야 합니다 `Cancel or Complete File` 메서드를 사용합니다.

#### [!UICONTROL 파일 업로드]

이 모듈에서는 번역용 또는 번역 프로젝트에 참조 자료로 포함할 파일을 업로드할 수 있습니다. 업로드는 다중 파트/양식 데이터를 사용하여 제출해야 하며 둘 이상의 파일을 포함할 수 있습니다. 다음을 지정합니다. `ProjectOptionId` 업로드한 파일을 평가하는 데 사용해야 합니다. 이렇게 하면 업로드하는 각 파일이 번역을 위해 가능한 후보인지 또는 참조 자료로 처리해야 하는지 여부를 결정합니다. 아카이브의 경우 (`zip `, `rar`, `7z`, `tar` 파일) 앱은 아카이브 내용을 검사하고 아카이브를 전체적으로 번역할 수 있는지 여부 또는 번역 가능한 파일과 번역할 수 없는 파일이 혼합되어 있는지 여부를 나타냅니다.

>[!NOTE]
>
>한 번에 두 개 이상의 파일을 업로드하면 실패의 영향을 높일 수 있으므로 권장되지 않습니다.

#### [!UICONTROL 참조 파일 추가]

이 모듈은 참조 파일을 추가합니다.

### 프로젝트

#### [!UICONTROL 프로젝트 만들기]

이 모듈은 지정된 프로젝트를 만듭니다.

#### 프로젝트 취소 또는 완료

이 모듈은 지정된 프로젝트를 취소하거나 완료합니다. 프로젝트가 다운로드 대기 중인 경우 워크플로의 마지막 단계를 통해 프로젝트가 전환되고 결국 완료로 이동합니다. 프로젝트가 승인 대기 중이거나 공급업체 선택이 취소된 경우. 프로젝트가 다른 상태에 있으면 요청이 실패합니다.

#### [!UICONTROL 프로젝트 Zip 다운로드]

이 모듈은 `zip` 지정된 프로젝트에 대해 번역된 파일의 파일입니다.

#### [!UICONTROL 프로젝트 읽기]

이 모듈은 지정된 프로젝트를 가져옵니다.

#### [!UICONTROL 상태에서 프로젝트 가져오기]

이 모듈은 지정된 상태에서 사용 가능한 모든 프로젝트를 가져옵니다. 이 방법을 사용하면 다음을 지정하여 결과를 페이징할 수 있습니다. `$top`, `$skip`, 및 `$orderby` 쿼리 매개 변수.

#### [!UICONTROL 프로젝트 목록 가져오기]

각 프로젝트에 대한 일반 정보를 제공하여 모든 프로젝트의 간단한 목록을 가져옵니다. 이 방법을 사용하면 다음을 지정하여 결과를 페이지로 만들 수 있습니다. `$top`, `$skip`, 및 `$orderby` 쿼리 매개 변수.

#### [!UICONTROL 프로젝트 만들기 옵션 검색]

이 모듈에서는 프로젝트 만들기 옵션을 가져옵니다.

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈은 임의의 승인된 API 호출을 수행합니다.
