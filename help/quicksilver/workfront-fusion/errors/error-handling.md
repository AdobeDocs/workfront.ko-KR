---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 오류 처리 중 [!DNL Adobe Workfront Fusion]
description: 시나리오 실행 중에 오류가 발생하면 일반적으로 오류로 인해 서비스를 사용할 수 없거나, 서비스가 예기치 않은 데이터로 응답하거나, 입력 데이터의 유효성 검사가 실패하기 때문입니다.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 에서 오류 처리 중 [!DNL Adobe Workfront Fusion]

시나리오 실행 중에 오류가 발생하면 일반적으로 오류로 인해 서비스를 사용할 수 없거나, 서비스가 예기치 않은 데이터로 응답하거나, 입력 데이터의 유효성 검사가 실패하기 때문입니다.

>[!NOTE]
>
>시나리오 실행 중에 모듈에 오류가 발생하고 모듈에 연결된 오류 처리 경로가 없는 경우 의 설명에 따라 기본 오류 처리 논리가 실행됩니다. [에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

모듈에 오류 처리기 경로를 추가하면 기본 오류 처리 논리를 직접 바꿀 수 있습니다. [!DNL Adobe Workfront Fusion] 은 5개의 다른 지시어를 제공하며, 이 지시어는 오류 처리기 경로의 끝에 삽입할 수 있습니다. 자세한 내용은 [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 오류 처리기 경로

모듈에 오류 처리기 경로를 추가하려면(모듈 X라고 함) 모듈을 마우스 오른쪽 버튼으로 클릭하고 를 선택합니다 **[!UICONTROL 오류 처리기 추가]**:

![](assets/error-handler-route.png)

이 모듈은 시나리오에 사용되는 앱과 지시어 목록을 보여줍니다. 모듈 X가 경로에 있는 마지막 모듈인 경우 지시어 중 하나를 선택해야 합니다. 또는 경로에 하나 이상의 모듈을 추가할 수 있습니다. 이 경우 [!UICONTROL 무시] 지시어는 기본적으로 모듈 X에 적용되며, 오류가 발생하면 해당 경로의 후속 모듈이 처리됩니다.

![](assets/directives-350x426.png)

아래에서 볼 수 있듯이 를 실행하는 동안 오류가 발생하는 경우 [!UICONTROL 폴더 만들기] 모듈, [!UICONTROL 무시] 지시어가 자동으로 적용되며 &quot;Data Error Take Place&quot; 필터가 하나 이상의 번들을 반환하는 경우 시나리오가 오류 처리기 경로의 다음 모듈로 이동합니다.

그러나 오류가 없으면 시나리오가 [!UICONTROL 폴더 모듈에 있는 모든 파일 나열] 정차.

![](assets/if-there-is-no-error-350x234.png)

또한, 오류 처리기 경로를 일반 경로와 구분하기 위해, 상기와 같이 투명 원으로 구성되어 있다.

## 지시 처리 오류

지침은 아래에 간략하게 설명되어 있습니다. 자세한 내용은 [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

시나리오 실행을 계속할지 여부를 기준으로 다음 범주로 그룹화할 수 있는 총 5개의 지시어가 있습니다.

다음 지시문은 시나리오 실행이 계속되도록 합니다.

* **[!UICONTROL 다시 시작]** 을 사용하면 오류가 있는 모듈의 대체 출력을 지정할 수 있으며 시나리오 실행 상태가 성공으로 표시됩니다
* **[!UICONTROL 무시]** 오류를 무시하면 시나리오 실행 상태가 성공으로 표시됩니다
* **[!UICONTROL 브레이크]** 불완전한 실행 대기열에 입력을 저장하고 시나리오 실행 상태가 경고로 표시됩니다. 자세한 내용은 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

반면 시나리오 실행을 중지해야 하는 경우 다음 지시문 중 하나를 사용해야 합니다.

* **[!UICONTROL 롤백]** 시나리오 실행을 즉시 중지하고 상태를 오류로 표시
* **[!UICONTROL 커밋]** 시나리오 실행을 즉시 중단하고 상태를 성공으로 표시합니다

## 추가 리소스

* [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [의 고급 오류 처리 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (위에 참조된 Dropbox 시나리오 세트 포함)
