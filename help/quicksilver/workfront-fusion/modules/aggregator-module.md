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
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 [!UICONTROL 집계] 모듈

집계 모듈은 여러 데이터 번들을 단일 번들로 병합하도록 설계된 모듈 유형입니다.

모듈 유형에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

+++

## [!UICONTROL 집계] 모듈 개요

[!UICONTROL 집계] 모듈이 실행되면 다음을 수행합니다.

* 단일 소스 모듈의 작업 중에 수신하는 모든 번들을 누적합니다.
* 누적된 각 번들에 대해 하나의 항목을 포함하는 배열이 있는 단일 번들을 출력합니다. 배열 항목의 내용은 특정 [!UICONTROL 집계] 모듈과 그 설정에 따라 다릅니다.

다음 이미지는 [!UICONTROL 집계] 모듈의 일반적인 설정을 보여 줍니다.

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>번들 집계가 시작되는 모듈입니다. 소스 모듈은 일반적으로 반복자 또는 일련의 번들을 출력하는 검색 모듈이다.</p><p>애그리게이터의 소스 모듈을 설정하고 애그리게이터 설정을 닫으면 소스 모듈과 애그리게이터 모듈 사이의 경로가 회색 영역으로 줄바꿈되어 애그리게이션의 시작과 끝을 명확하게 볼 수 있습니다. 
   </p> <p>반복기에 대한 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL 반복기] 모듈을 참조하십시오.</p> <p>검색 모듈에 대한 자세한 내용은 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">모듈 유형</a>의 검색 모듈을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target 구조 유형]</p> </td> 
   <td> <p>([!UICONTROL Array Aggregator] 모듈에만 적용됩니다.) 데이터가 집계되는 대상 구조입니다. 기본 옵션인 [!UICONTROL Custom]을(를) 사용하면 [!UICONTROL Array Aggregator]의 출력 번들의 <code>Array </code>개 항목으로 집계할 항목을 선택할 수 있습니다.</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>[!UICONTROL Array Aggregator] 모듈 다음에 모듈을 더 연결하고 모듈의 설정으로 돌아가면 [!UICONTROL Target] 구조 유형 드롭다운 메뉴에 [!DNL Slack] &gt;[!UICONTROL Create a Message] 모듈의 [!UICONTROL Attachments] 필드에 표시된 대로 '컬렉션 배열' 유형인 다음 모든 모듈과 해당 필드가 포함됩니다.</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 집계된 필드]</td> 
   <td>집계 모듈 출력에 포함할 필드입니다.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>집계자의 출력은 [!UICONTROL Group by] 필드를 사용하여 여러 그룹으로 분할할 수 있습니다. [!UICONTROL Group by] 필드에는 각 집계기의 입력 번들에 대해 평가되는 수식이 포함될 수 있습니다. 그런 다음 집계기는 각 개별 공식의 값마다 하나의 번들을 출력합니다. 각 번들에는 두 개의 항목이 포함되어 있습니다.</p> 
    <ul> 
     <li><code>Key </code>는 고유 값을 포함합니다.</li> 
     <li><code>Array </code><code>Key </code> 값으로 계산되는 수식이 포함된 번들의 집계 데이터를 포함합니다.</li> 
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
>원본 모듈과 [!UICONTROL 집계] 모듈 사이의 모듈에서 생성된 번들은 [!UICONTROL 집계] 모듈에서 출력되지 않으므로 [!UICONTROL 집계] 이후의 흐름에서 모듈에서 해당 번들에 액세스할 수 없습니다. 소스 모듈과 [!UICONTROL 집계] 모듈 사이의 모듈에서 출력된 번들의 데이터가 필요한 경우 [!UICONTROL 집계] 모듈의 설정에 지정된 항목을 포함하십시오([!UICONTROL 배열 집계] 모듈의 설정에 있는 [!UICONTROL 집계된 필드] 필드에서와 같이).


## 집계자의 작동 방식에 대한 예제 시나리오

이 예제 시나리오는 모든 이메일 첨부 파일을 압축하고 ZIP을 [!DNL Dropbox]에 업로드하는 방법을 보여 줍니다.

![](assets/dropbox-archive-350x87.png)

아래 시나리오는 다음 방법을 보여 줍니다.

* 첫 번째 모듈은 수신 전자 메일에 대한 사서함을 감시합니다. [!UICONTROL 전자 메일] >[!UICONTROL 전자 메일 감시] 트리거는 모든 전자 메일의 첨부 파일이 포함된 배열인 `Attachments[]` 항목이 있는 번들을 출력합니다.

* 두 번째 모델은 전자 메일의 첨부 파일을 반복합니다. [!UICONTROL 전자 메일] >[!UICONTROL 첨부 파일 반복] 반복기는 `Attachments[]` 배열의 항목을 하나씩 가져와서 별도의 번들로 더 보냅니다.

* 세 번째 모듈은 [!UICONTROL 이메일] >[!UICONTROL 첨부 파일 반복] 모듈에서 출력된 번들을 집계합니다. [!UICONTROL 보관] >[!UICONTROL 보관 집계 만들기]는 수신한 모든 번들을 누적하고 ZIP 파일이 포함된 단일 번들을 출력합니다.

* 마지막 모듈이 결과 ZIP 파일을 [!DNL Dropbox]에 업로드합니다. [!DNL Dropbox] > [!UICONTROL 파일 업로드] [!UICONTROL 보관] > [!UICONTROL 보관 만들기] 모듈에서 ZIP 파일을 가져와서 [!DNL Dropbox]에 업로드합니다.



다음은 [!UICONTROL 보관] > [!UICONTROL 보관 만들기] 집계의 샘플 설정입니다.

![](assets/archive-create-an-archive-350x484.png)
