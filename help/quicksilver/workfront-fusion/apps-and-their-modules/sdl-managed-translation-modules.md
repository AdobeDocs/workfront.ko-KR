---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: SDL 관리 번역 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 SDL Managed Translation 계정을 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL SDL Managed Translation] 여러 타사 애플리케이션 및 서비스에 계정을 설정합니다.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] 모듈

>[!NOTE]
>
>호출에 대한 작업 시간 제한 [!DNL SDL Managed Translation] is **120초**.

### 파일

#### [!UICONTROL 번역된 파일 다운로드]

이 모듈은 지정된 프로젝트 내에 포함된 번역된 단일 파일의 컨텐츠를 검색합니다. 요청된 파일이 아직 Downland 상태가 아닌 경우, 파일의 내용이 아직 완전히 번역되지 않을 수 있습니다. 파일이 다운로드 상태이고 이 파일을 성공적으로 검색한 경우 를 사용하여 파일을 완료로 표시해야 합니다. `Cancel or Complete File` 메서드를 사용합니다.

#### [!UICONTROL 파일 업로드]

이 모듈을 사용하면 번역 또는 번역 프로젝트에 참조 자료로 포함할 파일을 업로드할 수 있습니다. 멀티파트/양식 데이터를 사용하여 업로드를 제출해야 하며 둘 이상의 파일을 포함할 수 있습니다. 을(를) 지정합니다. `ProjectOptionId` 업로드된 파일을 평가하는 데 사용해야 합니다. 이는 업로드하는 각 파일이 번역을 수행할 수 있는 후보인지 아니면 참조 자료로 처리되어야 하는지를 결정합니다. 아카이브의 경우 (`zip `, `rar`, `7z`, `tar` 파일) 이 앱은 보관 파일의 내용을 검사하고 보관 파일이 전체적으로 번역될 수 있는지 여부 또는 번역 가능한 파일과 그렇지 않은 파일이 포함되어 있는지 여부를 나타냅니다.

>[!NOTE]
>
>한 번에 두 개 이상의 파일을 업로드하는 것은 실패의 영향을 증가시킬 수 있으므로 권장되지 않습니다.

#### [!UICONTROL 참조 파일 추가]

이 모듈은 참조 파일을 추가합니다.

### 프로젝트

#### [!UICONTROL 프로젝트 만들기]

이 모듈은 지정된 프로젝트를 만듭니다.

#### 프로젝트 취소 또는 완료

이 모듈은 지정된 프로젝트를 취소하거나 완료합니다. 프로젝트가 다운로드를 기다리는 경우 프로젝트는 워크플로우의 최종 단계를 통해 전환되고 결국 완료됩니다. 프로젝트가 승인을 기다리고 있거나 공급업체 선택이 취소되는 경우. 프로젝트가 다른 상태에 있으면 요청이 실패합니다.

#### [!UICONTROL 프로젝트 Zip 다운로드]

이 모듈은 `zip` 지정된 프로젝트의 번역된 파일 파일입니다.

#### [!UICONTROL 프로젝트 읽기]

이 모듈은 지정된 프로젝트를 가져옵니다.

#### [!UICONTROL 상태에서 프로젝트 가져오기]

이 모듈은 지정된 상태의 사용 가능한 모든 프로젝트를 가져옵니다. 이 방법을 사용하면 `$top`, `$skip`, 및 `$orderby` 쿼리 매개 변수.

#### [!UICONTROL 프로젝트 목록 가져오기]

각 프로젝트에 대한 일반 정보를 제공하는 간단한 모든 프로젝트 목록을 가져옵니다. 이 방법을 사용하면 `$top`, `$skip`, 및 `$orderby` 쿼리 매개 변수.

#### [!UICONTROL 프로젝트 만들기 옵션 검색]

이 모듈은 프로젝트 만들기 옵션을 가져옵니다.

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈은 임의 인증 API 호출을 수행합니다.
