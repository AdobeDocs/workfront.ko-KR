---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: SOAP 모듈
description: SOAP 모듈을 사용하여 Adobe Workfront Fusion의 SOAP API에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL SOAP] 모듈

를 사용할 수 있습니다 [!UICONTROL SOAP] 연결할 모듈 [!UICONTROL SOAP] 의 API [!UICONTROL Adobe Workfront Fusion].

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

## 사용 [!UICONTROL SOAP] 모듈

다음 [!UICONTROL SOAP] 모듈이 현재 베타 버전이며 지원되지 않습니다.

* 요소 재정의
* 분수 자릿수 제한
* 총 자릿수 제한
* 화이트 스페이스 제한
* 입력 및 출력 메시지의 여러 부분. 단일 부품 메시지만 지원됩니다
* 다음을 사용하여 정의된 사용자 정의 XML 스키마 요소 [[!UICONTROL SOAP] 인코딩](http://schemas.xmlsoap.org) 스키마 및 요소.

>[!INFO]
>
>**예:**
>  
>다음은에서 올바르게 인식하지 못합니다. [!UICONTROL Workfront Fusion]:
>
>
```
><complexType name="ArrayOfFloat">
>
>   
  <complexContent>
>
>      
     <restriction base="soapenc:Array">
>
>         
        <attribute ref="soapenc:arrayType"
>
>            
           wsdl:arrayType="xsd:integer[]"/>
>
>      
     </restriction>
>
>   
  </complexContent>
>
>
</complexType>
>```

여기에는 다음이 포함됩니다 `soapenc:Array`, `soapenc:arrayType` 및 `wsdl:arrayType` 참조 - 아직 에서 지원되지 않음 [!UICONTROL Workfront Fusion].

## 해결 방법

만약 [!UICONTROL SOAP] 모듈이 WSDL 파일 처리를 거부하거나 모듈의 구성에 여러 오류가 발생하면 범용 **[!UICONTROL HTTP] > [!UICONTROL 요청 수행]** 대신,

1. in [!DNL Workfront Fusion], 새 시나리오를 만듭니다 .
1. 를 삽입합니다. **[!UICONTROL HTTP] > [!UICONTROL 요청 수행]** 모듈에 대해 고려합니다.
1. 모듈의 구성을 열고 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 메서드]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 컨텐츠 유형]</td> 
      <td> <p>[!UICONTROL XML(application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 구문 분석 응답]</td> 
      <td>[!UICONTROL Enabled]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. 새 웹 브라우저 창이나 탭을 엽니다.
1. WSDL URL을 웹 브라우저의 주소 표시줄에 붙여 넣고 XML 파일을 가져옵니다.

   WSDL URL은 일반적으로 `?wsdl`예를 들어 반드시 필요한 것은 아닙니다 `http://voip.ms/api/v1/server.wsdl`.

1. WSDL 파일이 웹 브라우저에 직접 표시되지 않으면 다운로드한 파일을 텍스트 편집기에서 엽니다.
1. 을 검색합니다. `<service>` 또는 `<wsdl:service>` 태그:

   ![](assets/service-350x65.png)

1. 위치를 찾으면 URL을 `location` 속성을 사용합니다.
1. in [!DNL Workfront Fusion]를 HTTP 모듈의 URL 필드에 붙여넣습니다.
1. 를 엽니다. [온라인 [!UICONTROL SOAP] 클라이언트](https://wsdlbrowser.com/) 새 웹 브라우저 창/탭에서 을 클릭합니다.
1. WSDL URL을 WSDL URL 필드에 붙여 넣습니다.
1. 클릭 **[!UICONTROL 찾아보기]**.
1. 함수 목록에서 왼쪽에 있는 을 선택합니다. `getLanguages`.
1. 의 컨텐츠 복사 [!UICONTROL XML 요청] 텍스트 영역.
1. in [!UICONTROL Workfront Fusion]복사한 콘텐츠를 모듈의 URL 필드에 붙여넣습니다.
1. 물음표를 실제 값으로 대체하여 선택한 매개 변수의 값을 제공합니다.

   ![](assets/request-xml-350x172.png)

1. 을(를) 클릭하여 모듈의 구성을 닫습니다. **[!UICONTROL 확인]**.
1. 시나리오 또는 모듈을 실행합니다.
