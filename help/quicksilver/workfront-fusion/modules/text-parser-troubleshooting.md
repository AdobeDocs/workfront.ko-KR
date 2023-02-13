---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 의 텍스트 파서 문제 해결 [!DNL Adobe Workfront Fusion]
description: 텍스트 파서를 가져와서 출력을 생성할 수 없는 경우 이 정보를 사용하십시오.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 의 텍스트 파서 문제 해결 [!DNL Adobe Workfront Fusion]

텍스트 파서를 가져와서 출력을 생성할 수 없는 경우 이 정보를 사용하십시오.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 문제 해결

사례 시나리오 예를 들어 파일 문서 &quot;filename.docx&quot;의 파일 유형을 구문 분석하려고 하며 파일 이름의 확장명은 항상 DOCX에서 PDF에서 CSV로 변경됩니다.

이 경우에 사용할 수 있는 식은 다음과 같습니다 [!DNL \..+]

regex101.com의 regex 표현식에서 이 기능을 사용하려는 경우 전체 일치 항목이 제공됩니다.

![](assets/regex-expression-350x130.png)

위의 이미지에서 파일 확장자가 올바르게 일치했습니다. 이를 가져와 텍스트 파서에서 구현하려고 하면 다음과 같이 하십시오.

![](assets/text-parser-350x602.png)

일치하는 항목이 없습니다.

![](assets/text-parser-you-dont-get-a-match-350x365.png)

이유는 &quot;i&quot;가 일치당 일치 횟수만 표시하므로 이 경우 2개가 일치하므로 &quot;i&quot; 다음에 숫자 값 1과 2가 있기 때문입니다. 이 사용 사례에서는 두 번째 일치 값만 필터를 통해 데이터를 일치시키거나 전달해야 하며 숫자 값으로 표시되는 값을 지정할 수 있습니다.

![](assets/text-parser-matches-350x355.png)

구문 분석하려는 부분에 대괄호를 추가해야 하는 일치 값을 가져오려면(예: &quot;filename.docx&quot; - &quot;docx&quot;에서만 추출), 이 사례 시나리오에서 사용하는 regex 표현식에 따라 대괄호를 \에 적용해야 합니다.(이)를 참조하십시오.+)

이렇게 하면 DOCX를 캡처하고 그룹에 지정하고 &quot;.&quot;를 그대로 둡니다. 빠져나가

![](assets/text-parser-get-matches-350x592.png)

아래 그림에 표시된 출력에서 캡처 그룹은 모든 문자(라인 종료자 제외)와 일치합니다.

![](assets/text-parser-output-350x389.png)

regex를 통합하는 또 다른 해결 방법은 replace 함수를 사용하는 것입니다

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

그런 다음 를 바꿉니다 `abcdefghijklmno pqr stuvw xyz.docx` 실제 파일 이름 변수로 사용됩니다.
