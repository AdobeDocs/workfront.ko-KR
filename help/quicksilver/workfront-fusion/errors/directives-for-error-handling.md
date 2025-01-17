---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion]의 오류 처리에 대한 지시문'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 12%

---

# [!DNL Adobe Workfront Fusion]에서 오류 처리를 위한 지시문

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [오류 처리에 대한 지시문](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/directives-for-error-handling.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

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

## 오류 처리를 위한 지시문

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Rollback</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>시나리오 실행이 즉시 중지되고 모든 모듈을 초기 상태로 되돌리기 위해 모든 모듈에서 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">롤백</a> 단계가 시작됩니다. 후속 모듈이 처리되지 않습니다.</p> <p>몇 가지 오류 유형이 없으면 시나리오 설정에 지정된 연속 오류 수가 지나면 시나리오가 비활성화됩니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">연속 오류 수</a>를 참조하십시오.</p> <p>시나리오 실행 상태는 “오류”로 표시됩니다.</p> <p>참고: 모듈에 연결된 오류 처리기 경로가 없고 [!UICONTROL 시나리오 설정] 아래의 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL 미완료 실행 저장 허용]</a> 설정이 선택되어 있지 않은 경우 기본 동작입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>커밋</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>시나리오 실행이 즉시 중지되고 모든 모듈에서 커밋 단계가 시작됩니다. 후속 모듈이 처리되지 않습니다.</p> <p>처리되지 않은 모든 번들은 무시됩니다.</p> <p>시나리오 실행 상태가 "성공"으로 표시됩니다. 커밋 단계에 대한 자세한 내용은 문서 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion의 시나리오 실행, 주기 및 단계</a>에서 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">커밋</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Resume</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>대체 출력이 지정되어 오류가 발생한 모듈에 제공됩니다.</p> <p>후속 모듈이 처리됩니다.</p> <p>시나리오 실행 상태는 “성공”으로 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>무시</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>오류가 무시되고 후속 모듈이 처리되지 않습니다.</p> <p>처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속됩니다.</p> <p>시나리오 실행 상태는 “성공”으로 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Break</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>시나리오 실행 상태가 오류를 수동으로 해결할 수 있는 불완전한 실행 대기열에 저장됩니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Adobe Workfront Fusion에서 불완전한 실행 확인 및 해결</a>을 참조하십시오. </p> <p>그러나 몇 가지 예외가 있습니다. 자세한 내용은 문서 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion의 시나리오 설정 패널</a>에서 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">불완전한 실행 저장 허용</a>을 참조하십시오.</p> <p>후속 모듈이 처리되지 않습니다.</p> <p>처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속됩니다.</p> <p>[!UICONTROL 자동으로 실행 완료] 옵션을 비활성화하면 시나리오 실행 상태가 "경고"로 표시됩니다.</p> <p>자세한 내용은 아래의 <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> 섹션을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>다시 시도</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>경우에 따라 시간이 지남에 따라 실패 사유가 사라질 가능성이 있을 때 두 번 동안 실패 모듈을 다시 실행하는 것이 유용할 수 있습니다.</p> <p>Workfront Fusion은 현재 Retry 지시문을 제공하지 않지만 몇 가지 해결 방법을 사용하여 해당 기능을 모방할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Adobe Workfront Fusion에서 오류 처리 다시 시도</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 현재 오류 처리 지침은 오류 처리 경로 외부에서 사용할 수 없습니다.
>
>   자세한 내용은 문서 [Adobe Workfront Fusion의 오류 처리](../../workfront-fusion/errors/error-handling.md)에서 [오류 처리기 경로](../../workfront-fusion/errors/error-handling.md#error)를 참조하십시오.
>* [!DNL Workfront Fusion]은(는) 기능을 모방하도록 해결 방법을 사용할 수 있지만, 조건부로 오류를 쉽게 생성(throw)할 수 있는 Throw 모듈을 제공하지 않습니다.
>
>   자세한 내용은 문서 [Adobe Workfront Fusion에서 오류 처리 실행](../../workfront-fusion/errors/throw.md)에서 [Throw에 대한 해결 방법](../../workfront-fusion/errors/throw.md#workaround-for-throw)을 참조하십시오.

## Break {#break}

[!DNL Break] 지시문에서 오류를 처리하면 미완료 실행 폴더에 레코드가 만들어집니다. 이 레코드에는 이전 모듈의 데이터와 함께 시나리오 실행 상태가 저장됩니다. 레코드는 오류가 발생한 모듈을 참조하고 모듈에 의해 입력으로 수신된 데이터에 관한 정보를 포함합니다. 오류를 일으키는 각 데이터 번들에 대해 별도의 레코드가 만들어집니다.

자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 확인 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.

### Break 지시문으로 인한 오류 해결

필요한 경우 시나리오를 업데이트하고 한 번 실행하여 오류를 수동으로 해결할 수 있습니다.

시나리오를 다시 실행하여 불완전한 실행을 자동으로 처리하도록 시나리오를 구성할 수도 있습니다. 미완료 실행을 처리하도록 모듈을 구성하려면 다음을 수행합니다.

1. 브레이크 모듈 내에서 [!UICONTROL **자동으로 실행 완료**] 옵션을 사용하도록 설정합니다.
1. **시도 횟수** 필드에 모듈에서 실행을 다시 시도할 최대 시도 횟수를 입력하거나 매핑합니다

   이 숫자는 1에서 100 사이여야 합니다.
1. **시도 간격** 필드에 각 재시도 간격(분)을 입력하거나 매핑합니다.

이 옵션을 활성화하면 오류가 발생하면 불완전한 실행이 검색되고([!UICONTROL 시도 간격] 필드에 지정된 시간 이후) 원래 입력 데이터로 실행됩니다. 이 작업은 모듈 실행이 오류 없이 완료되거나 지정된 시도 횟수에 도달할 때까지 반복됩니다.

>[!NOTE]
>
>초기 재시도 시도가 실패하면 재시도 간격은 다른 시도마다 기하급수적으로 증가합니다.


&quot;자동 실행 완료&quot;가 켜지면 브레이크 오류 처리기의 자동 다시 시도가 문제를 자동으로 처리하고 있으므로 시나리오 실행이 &quot;성공&quot;으로 표시됩니다. 이 경우 실패한 실행에 대한 이메일이 사용자에게 전송되지 않습니다.

자동 실행 완료가 꺼져 있으면 실행이 &quot;경고&quot;로 표시됩니다.

미완료 실행에 저장되는 실행은 예외적이며, 일부 오류 유형에서는 시나리오 실행의 자동 재시도가 불가능합니다.

자세한 내용은 문서 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md)에서 [불완전한 실행 저장 허용](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)을 참조하십시오.

자세한 내용은 [Adobe Workfront Fusion의 고급 오류 처리](../../workfront-fusion/errors/advanced-error-handling.md)를 참조하십시오.
