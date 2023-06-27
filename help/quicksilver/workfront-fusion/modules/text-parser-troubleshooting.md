---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 의 텍스트 파서 문제 해결 [!DNL Adobe Workfront Fusion]
description: 텍스트 구문 분석기를 사용하여 출력을 생성할 수 없는 경우 이 정보를 사용합니다.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 의 텍스트 파서 문제 해결 [!DNL Adobe Workfront Fusion]

텍스트 구문 분석기를 사용하여 출력을 생성할 수 없는 경우 이 정보를 사용합니다.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
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

## 문제 해결

사례 시나리오의 경우 파일 문서 &quot;filename.docx&quot;의 파일 유형을 구문 분석하려고 하며 파일 이름의 확장자는 항상 DOCX에서 PDF으로 CSV로 다릅니다.

이 경우 사용할 수 있는 표현식은 다음과 같습니다. [!DNL \..+]

regex101.com에서 regex 표현식에서 이 함수를 사용하고자 하는 경우 전체 일치 항목을 얻을 수 있습니다.

![](assets/regex-expression-350x130.png)

위의 이미지에서 파일 확장명이 올바르게 일치했습니다. 이 옵션을 선택하고 텍스트 파서에서 구현해 보면 다음과 같습니다.

![](assets/text-parser-350x602.png)

일치 항목을 가져올 수 없습니다.

![](assets/text-parser-you-dont-get-a-match-350x365.png)

그 이유는 &quot;i&quot;가 일치 항목 당 일치 항목 수만 표시하므로 이 경우 2개의 일치 항목이 있으므로 &quot;i&quot; 다음에 숫자 값 1과 2가 있습니다. 이 사용 사례에서는 두 번째 일치하는 값만 필터를 통해 데이터를 일치시키거나 전달해야 하는 경우 숫자 값으로 표현되는 값을 지정할 수 있습니다.

![](assets/text-parser-matches-350x355.png)

구문 분석할 부분에 대괄호를 추가하는 데 필요한 일치 값을 가져올 수 있으려면(예: &quot;filename.docx&quot; - &quot;docx&quot;에서만 추출) 이 경우 시나리오에서 사용 중인 정규 표현식에 따라 대괄호를 \에 적용해야 합니다.(.+)

이렇게 하면 DOCX를 캡처하고 그룹에 지정한 다음 &quot;.&quot; 빠지라고

![](assets/text-parser-get-matches-350x592.png)

아래 그림에 표시된 출력에서 캡처 그룹은 모든 문자와 일치합니다(줄 종결자 제외).

![](assets/text-parser-output-350x389.png)

정규 표현식도 통합하는 또 다른 해결 방법은 바꾸기 기능을 사용하는 것입니다

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

다음 바꾸기 `abcdefghijklmno pqr stuvw xyz.docx` 와 함께 사용하십시오.
