---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion의 누적 모듈
description: 누적 모듈은 여러 데이터 번들을 단일 번들로 병합하도록 설계된 모듈 유형입니다.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL 누적] 모듈 [!DNL Adobe Workfront Fusion]

누적 모듈은 여러 데이터 번들을 단일 번들로 병합하도록 설계된 모듈 유형입니다.

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

## [!UICONTROL 누적] 모듈

다음 경우에 [!UICONTROL 누적] 모듈이 실행되면, 다음을 수행합니다.

* 단일 소스 모듈의 작업 중에 수신되는 모든 번들을 누적합니다.
* 누적된 각 번들에 대해 하나의 항목이 포함된 배열로 단일 번들을 출력합니다. 배열 항목의 내용은 특정 항목에 따라 다릅니다 [!UICONTROL 누적] 모듈 및 해당 설정.

다음 이미지는 [!UICONTROL 누적] 모듈 :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 소스 모듈]</p> </td> 
   <td> <p>번들 집계가 시작될 모듈입니다. 소스 모듈은 대개 일련의 번들을 출력하는 반복기 또는 검색 모듈입니다. 누적 소스 모듈을 설정(및 누적 모듈의 설정을 닫기)할 때 소스 모듈과 누적 모듈 사이의 경로는 회색 영역으로 래핑되어 합계 시작 및 종료를 명확하게 볼 수 있습니다. 
   </p> <p>반복기에 대한 자세한 내용은 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">의 [!UICONTROL Iterator] 모듈 [!DNL Adobe Workfront Fusion]</a></p> <p>검색 모듈에 대한 자세한 내용은 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">모듈 유형</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target 구조 유형]</p> </td> 
   <td> <p>([!UICONTROL Array Aggregator] 모듈에만 적용할 수 있습니다.) 데이터를 집계할 대상 구조입니다. 기본 옵션인 [!UICONTROL Custom]을 사용하면 A[!UICONTROL raggregator]의 출력 번들의 출력 번들에 집계해야 하는 항목을 선택할 수 있습니다 <code>Array </code>항목:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>[!UICONTROL Array Aggregator] 모듈 다음에 모듈을 더 연결하고 모듈의 설정으로 돌아오면 [!UICONTROL Target] 구조 유형 드롭다운에는 다음 모듈 및 해당 필드가 모두 포함되며, 이 필드는 [!UICONTROL Attachments] 필드에 나와 있습니다 [!DNL Slack] &gt;[!UICONTROL 메시지 만들기] 모듈:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 집계된 필드]</td> 
   <td>누적 모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>[!UICONTROL Group by] 필드의 도움을 받아 누적 출력을 여러 그룹으로 분할할 수 있습니다. [!UICONTROL Group by] 필드에는 각 누적 입력 번들에 대해 평가되는 수식이 포함될 수 있습니다. 그런 다음 집계자는 개별 수식의 값당 하나의 번들을 출력합니다. 각 번들에는 두 개의 항목이 포함되어 있습니다.</p> 
    <ul> 
     <li><code>Key </code>에는 고유한 값이 포함되어 있습니다.</li> 
     <li><code>Array </code>는 수식이 <code>Key </code>값.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>빈 집계 후 처리 중지</p> </td> 
   <td> <p>기본적으로 [!UICONTROL Aggregator] 모듈은 번들이 [!UICONTROL Aggregator] 모듈에 도달하지 않은 경우에도 집계 결과를 출력합니다(예를 들어, 진행 중에 모두 필터링되었으므로). 빈 집계] 옵션이 활성화된 경우 [!UICONTROL Aggregator] 모듈에서 출력 번들을 생성하지 않고, 흐름이 중지됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>소스 모듈과 [!UICONTROL 누적] 모듈이 [!UICONTROL 누적] 모듈로 연결되므로 흐름 내의 모듈에서 다음 작업을 액세스할 수 없습니다 [!UICONTROL 누적]. 소스 모듈과 [!UICONTROL 누적] 모듈, [!UICONTROL 누적] 모듈 설정(과 같이) [!UICONTROL 집계된 필드] 의 설정 필드 [!UICONTROL 어레이 누적] 모듈).


>[!INFO]
>
>**예:** 사용 사례: 모든 이메일 첨부 파일을 지핑하고 ZIP을 업로드 합니다. [!DNL Dropbox]
>
>아래 시나리오에서는 다음 방법을 보여줍니다.
>
>* 수신 전자 메일의 사서함 보기: [!UICONTROL 이메일] >[!UICONTROL 이메일 보기] 트리거가 항목이 있는 번들을 출력합니다. `Attachments[]`: 모든 전자 메일의 첨부 파일을 포함하는 배열입니다.
>
>* 전자 메일의 첨부 파일을 반복합니다. [!UICONTROL 이메일] >[!UICONTROL 첨부 파일 반복] 반복기는 `Attachments[]` 하나씩 배열하고 별도의 번들로 추가로 전송합니다.
>
>* 에서 출력한 번들을 집계합니다. [!UICONTROL 이메일] >[!UICONTROL 첨부 파일 반복] 모듈: [!UICONTROL 아카이브] >[!UICONTROL 아카이브 누적 만들기] 이 번들이 수신한 모든 번들을 축적하고 ZIP 파일을 포함하는 단일 번들을 출력합니다.
>
>* 결과 ZIP 파일을에 업로드합니다. [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL 파일 업로드] 에서 ZIP 파일을 가져옵니다 [!UICONTROL 아카이브] > [!UICONTROL 아카이브 만들기] 모듈로 업로드하여 [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>다음은 의 샘플 설정입니다 [!UICONTROL 아카이브] > [!UICONTROL 아카이브 만들기] 누적:
>
>![](assets/archive-create-an-archive-350x484.png)
