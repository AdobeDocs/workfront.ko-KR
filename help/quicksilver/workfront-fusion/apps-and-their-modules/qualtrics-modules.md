---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Qualtrics 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 Qualtrics를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Qualtrics 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Qualtrics]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## 전제 조건

를 사용하려면 [!DNL Qualtrics] 모듈이면 반드시 [!UICONTROL Qualtrics] 계정이 필요합니다.

## 연결 중 [!DNL Qualtrics] to [!DNL Workfront Fusion]

에 대한 연결을 만들 수 있습니다 [!DNL Qualtrics] 내에서 직접 계정 [!UICONTROL Qualtrics] 모듈.

1. 어떤 경우에서도 [!UICONTROL Qualtrics] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 다음 정보를 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 연결 이름]</p> </td> 
      <td> <p>새 연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 데이터 센터 ID] </td> 
      <td>형식 사용 <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API 키]</td> 
      <td>API 키를 찾으려면 를 참조하십시오. <a href="https://api.qualtrics.com/instructions/docs/Instructions/api-key-authentication.md">API 토큰 인증</a> 에서 [!DNL Qualtrics] 설명서.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Qualtrics] 모듈 및 해당 필드

다음 모듈은 [!DNL Qualtrics] 커넥터:

* [!UICONTROL 새 설문 조사 응답 보기]
* [!UICONTROL 디렉터리 연락처 만들기]
* [!UICONTROL 디렉터리 연락처 삭제]
* [!UICONTROL 디렉터리 연락처 가져오기]
* [!UICONTROL 디렉터리 연락처 업데이트]
* [!UICONTROL SMS를 통해 새 설문 조사 배포 만들기]
* [!UICONTROL 이메일을 통해 설문 조사 배포]
* [!UICONTROL API 호출 만들기]
* [!UICONTROL 디렉터리 연락처 나열]
