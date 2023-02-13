---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]
description: 이 문서에서는 [!DNL Adobe Workfront Fusion] 시나리오.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 50b43cd4bafdfc3379eb1d73c12e15c791e28dbe
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]

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

## 오류 처리를 위한 지시어

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>롤백</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>시나리오 실행이 즉시 중지되고 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">롤백</a> 단계가 모든 모듈에서 초기 상태로 되돌리기 위해 시작됩니다. 후속 모듈이 처리되지 않습니다.</p> <p>몇 가지 오류 유형을 사용하지 않는 경우 시나리오 설정에 지정된 연속 오류 수가 지나면 시나리오가 비활성화됩니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">연속 오류 수</a>.</p> <p>시나리오 실행 상태는 "error"로 표시됩니다.</p> <p>참고: 모듈 및 모듈에 연결된 오류 처리기 경로가 없는 경우 이 동작이 기본 동작입니다 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL 완료되지 않은 실행 저장 허용]</a> [!UICONTROL 시나리오 설정] 아래의 설정이 선택되어 있지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>커밋</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>시나리오 실행이 즉시 중지되고 모든 모듈에서 커밋 단계가 시작됩니다. 후속 모듈이 처리되지 않습니다.</p> <p>처리되지 않은 모든 번들은 무시됩니다.</p> <p>시나리오 실행 상태는 "성공"으로 표시됩니다. 커밋 단계에 대한 자세한 내용은 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">커밋</a> 기사 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion의 시나리오 실행, 주기 및 단계</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>다시 시작</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>대체 출력이 지정되고 오류가 발생하는 모듈에 제공됩니다.</p> <p>후속 모듈이 처리됩니다.</p> <p>시나리오 실행 상태는 "성공"으로 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>무시</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>오류가 무시되고 후속 모듈이 처리되지 않습니다.</p> <p>처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속 실행됩니다.</p> <p>시나리오 실행 상태는 "성공"으로 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>브레이크</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>시나리오 실행 상태는 오류를 수동으로 해결할 수 있는 불완전한 실행 큐에 저장됩니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결</a>. </p> <p>그러나, 몇 가지 예외가 있습니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">불완전한 실행 저장 허용</a> 기사 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion의 시나리오 설정 패널</a>.</p> <p>후속 모듈이 처리되지 않습니다.</p> <p>처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속 실행됩니다.</p> <p>[!UICONTROL 자동 실행] 옵션이 비활성화되어 있으면 시나리오 실행 상태가 "경고"로 표시됩니다.</p> <p>자세한 내용은 <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> 자세한 내용은 아래 섹션을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>다시 시도</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>경우에 따라 실패 이유가 시간이 지남에 따라 지나갈 수 있는 가능성이 있는 경우 몇 번 실패한 모듈을 다시 실행하는 것이 유용할 수 있습니다.</p> <p>Workfront Fusion은 현재 Retry 지시문을 제공하지 않지만, 몇 가지 해결 방법을 사용하여 해당 기능을 모방할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Adobe Workfront Fusion에서 오류 처리 다시 시도</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>현재 오류 처리 지시문은 오류 처리 경로 및 [!DNL Workfront Fusion] 현재 은(는) 해결 방법을 사용하여 해당 기능을 모방할 수 있지만 조건부로 오류(throw)를 쉽게 생성할 수 있도록 해주는 Throw 모듈을 제공하지 않습니다. 자세한 내용은 [오류 처리기 경로](../../workfront-fusion/errors/error-handling.md#error) 기사 [Adobe Workfront Fusion의 오류 처리](../../workfront-fusion/errors/error-handling.md). 참조: [Throw에 대한 해결 방법](../../workfront-fusion/errors/throw.md#workarou) 기사 [Adobe Workfront Fusion에서 오류 처리 실행](../../workfront-fusion/errors/throw.md).

## 브레이크 {#break}

에서 오류를 처리하는 경우 [!DNL Break] 지시문, 레코드는 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) 이전 모듈의 데이터와 함께 시나리오 실행 상태를 저장하는 폴더입니다. 오류를 일으키는 각 데이터 번들에 대해 별도의 레코드가 생성됩니다.

레코드는 오류가 발생한 모듈을 참조하며 모듈에서 받은 데이터에 대한 정보를 입력으로 포함합니다. 자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

여기에서 시나리오를 업데이트하고(필요한 경우) 한 번 실행하여 오류를 수동으로 해결할 수 있습니다.

반면 를 활성화하면 [!UICONTROL 자동 실행 완료] Break 지시어 설정 아래의 옵션은 지정된 시간(분) 후에 시나리오를 다시 실행하여 불완전한 실행을 자동으로 처리하도록 구성할 수 있습니다.

이 옵션을 활성화하면 오류가 발생하면 ( [!UICONTROL 시도 간격] 필드)가 실행되어 원래 입력 데이터로 실행됩니다. 이 작업은 오류 없이 또는 지정된 시도 횟수에 도달할 때까지 모듈 실행이 완료될 때까지 반복됩니다.

>[!NOTE]
>
>초기 다시 시도 시도가 실패하면 다시 시도 사이의 간격이 다른 시도마다 기하급수적으로 증가합니다.

&quot;자동 완료 실행&quot;이 켜지면 브레이크 오류 처리기의 자동 재시도는 자동으로 문제를 처리하므로 시나리오 실행이 &quot;성공&quot;으로 표시됩니다. 이 경우 사용자는 실패한 실행에 대한 이메일을 받지 않습니다.

&quot;Automatically complete execution&quot;이 해제되면 실행이 &quot;Warning&quot;으로 표시됩니다.

![](assets/break-directive-350x241.png)

그러나 실행 작업이 불완전한 실행 아래에 저장되고 일부 오류 유형이 있는 경우 시나리오 실행의 자동 재시도를 수행할 수 없습니다. 자세한 내용은 [불완전한 실행 저장 허용](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 기사 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md).

자세한 내용은 [Adobe Workfront Fusion의 고급 오류 처리](../../workfront-fusion/errors/advanced-error-handling.md).
