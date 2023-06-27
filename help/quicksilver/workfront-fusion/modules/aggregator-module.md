---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion의 집계 모듈
description: 집계 모듈은 여러 데이터 번들을 단일 번들로 병합하도록 설계된 모듈 유형입니다.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL 집계] 의 모듈 [!DNL Adobe Workfront Fusion]

집계 모듈은 여러 데이터 번들을 단일 번들로 병합하도록 설계된 모듈 유형입니다.

모듈 유형에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md).

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

## [!UICONTROL 집계] 모듈

다음의 경우 [!UICONTROL 집계] 모듈이 실행되면 다음 작업을 수행합니다.

* 단일 소스 모듈의 작업 중에 수신하는 모든 번들을 누적합니다.
* 누적된 각 번들에 대해 하나의 항목을 포함하는 배열이 있는 단일 번들을 출력합니다. 배열 항목의 내용은 특정 항목에 따라 다릅니다 [!UICONTROL 집계] 모듈 및 해당 설정.

다음 이미지는 의 일반적인 설정을 보여 줍니다 [!UICONTROL 집계] 모듈 :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 소스 모듈]</p> </td> 
   <td> <p>번들 집계가 시작될 모듈입니다. 소스 모듈은 일반적으로 반복자 또는 일련의 번들을 출력하는 검색 모듈이다. 애그리게이터의 소스 모듈을 설정하고 애그리게이터 설정을 닫으면 소스 모듈과 애그리게이터 모듈 사이의 경로가 회색 영역으로 줄바꿈되어 애그리게이션의 시작과 끝을 명확하게 볼 수 있습니다. 
   </p> <p>반복자에 대한 자세한 내용은 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">의 [!UICONTROL Iterator] 모듈 [!DNL Adobe Workfront Fusion]</a></p> <p>검색 모듈에 대한 자세한 내용은 의 검색 모듈을 참조하십시오. <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">모듈 유형</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target 구조 유형]</p> </td> 
   <td> <p>([!UICONTROL Array Aggregator] 모듈에만 적용됩니다.) 데이터를 집계할 대상 구조입니다. 기본 옵션인 [!UICONTROL Custom]을(를) 사용하면 A[!UICONTROL Array Aggregator]의 출력 번들로 집계해야 하는 항목을 선택할 수 있습니다 <code>Array </code>항목:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>[!UICONTROL Array Aggregator] 모듈 다음에 모듈을 더 연결하고 모듈의 설정으로 돌아가면 [!UICONTROL Target] 구조 유형 드롭다운에 의 [!UICONTROL Attachments] 필드에 표시된 대로 컬렉션 배열 유형의 다음 모든 모듈과 해당 필드가 포함됩니다. [!DNL Slack] &gt;[!UICONTROL 메시지 작성] 모듈:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 집계된 필드]</td> 
   <td>집계 모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>집계자의 출력은 [!UICONTROL Group by] 필드를 사용하여 여러 그룹으로 분할할 수 있습니다. [!UICONTROL Group by] 필드에는 각 집계기의 입력 번들에 대해 평가되는 수식이 포함될 수 있습니다. 그런 다음 집계기는 각 개별 공식의 값마다 하나의 번들을 출력합니다. 각 번들에는 두 개의 항목이 포함되어 있습니다.</p> 
    <ul> 
     <li><code>Key </code>는 고유 값을 포함합니다.</li> 
     <li><code>Array </code>에는 공식이 로 평가된 번들의 집계된 데이터가 포함됩니다. <code>Key </code>값.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>빈 집계 후 처리 중지</p> </td> 
   <td> <p>기본적으로 [!UICONTROL 집계] 모듈은 [!UICONTROL 집계] 모듈에 도달한 번들이 없는 경우에도 집계 결과를 출력합니다(예: 도중에 모두 필터링되었기 때문). 빈 집계 후 [!UICONTROL 처리 중지] 옵션을 활성화하면 [!UICONTROL Aggregator] 모듈에서 출력 번들을 생성하지 않고 흐름이 중지됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>소스 모듈과 [!UICONTROL 집계] 모듈이 [!UICONTROL 집계] 모듈을 사용하므로 다음 흐름의 모듈에서 액세스할 수 없습니다. [!UICONTROL 집계]. 소스 모듈과 [!UICONTROL 집계] 모듈에서 주어진 항목을 [!UICONTROL 집계] 모듈 설정(예: [!UICONTROL 집계된 필드] 의 설정 필드 [!UICONTROL 배열 집계] 모듈)을 참조하십시오.


>[!INFO]
>
>**예:** 사용 사례: 모든 이메일 첨부 파일 압축 및 ZIP 업로드 [!DNL Dropbox]
>
>아래 시나리오는 다음 방법을 보여 줍니다.
>
>* 사서함에서 수신 전자 메일 확인: [!UICONTROL 이메일] >[!UICONTROL 이메일 보기] 트리거는 항목이 있는 번들을 출력합니다. `Attachments[]`: 모든 이메일의 첨부 파일이 포함된 배열입니다.
>
>* 이메일의 첨부 파일 반복: [!UICONTROL 이메일] >[!UICONTROL 첨부 파일 반복] 반복기는 다음에서 항목을 가져옵니다. `Attachments[]` 하나씩 정렬하여 별도의 번들로 추가로 전송합니다.
>
>* 에서 출력하는 번들을 집계합니다. [!UICONTROL 이메일] >[!UICONTROL 첨부 파일 반복] 모듈: [!UICONTROL 보관] >[!UICONTROL 아카이브 집계 만들기] 는 수신하는 모든 번들을 누적하고 ZIP 파일이 포함된 단일 번들을 출력합니다.
>
>* 결과 ZIP 파일을에 업로드 [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL 파일 업로드] 에서 ZIP 파일 가져오기 [!UICONTROL 보관] > [!UICONTROL 아카이브 만들기] 모듈 및에 업로드합니다. [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>다음은 의 샘플 설정입니다. [!UICONTROL 보관] > [!UICONTROL 아카이브 만들기] 집계:
>
>![](assets/archive-create-an-archive-350x484.png)
