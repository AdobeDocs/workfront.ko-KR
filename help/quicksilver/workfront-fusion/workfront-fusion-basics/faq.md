---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion FAQ
description: 이 문서에서는 [!DNL Adobe Workfront Fusion]- Fusion 워크플로우에서 일반적으로 사용되는 객체에 대한 정보를 포함합니다
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Adobe Workfront Fusion FAQ

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 시나리오란 무엇입니까?

### 답변

시나리오는 실행할 단계의 순서를 정의합니다 [!DNL Adobe Workfront Fusion]. 각 시나리오에 대해 데이터 소스, 데이터 처리 방법, 사용할 데이터 및 무시할 데이터를 지정합니다. [!DNL Workfront Fusion] 필요한 만큼 복잡한 시나리오를 만들 수 있습니다. 가장 복잡한 시나리오도 가능하다.

자세한 내용은 [에서 연습 통합 시나리오를 만듭니다 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## 시나리오에서 두 개 이상의 모듈을 사용할 수 있습니까? 아니면 그냥 방아쇠와 행동인가?

### 답변

시나리오에 원하는 수만큼 모듈을 사용할 수 있습니다. 독립 경로를 만들고 경로를 통해 이동해야 하는 데이터를 지정할 수 있습니다. 개별 작업에서 반환된 결과를 사용한 다음 다음 작업에 전달할 수도 있습니다.

## Can [!DNL Workfront Fusion] 파일을 사용하여 작업

### 답변

예. 사용 [!DNL Workfront Fusion], 파일은 수신, 저장, 변환, 암호화 등의 작업을 수행할 수 있습니다. 게다가 [!DNL Workfront Fusion] 는 사용자가 파일에 포함된 데이터를 효율적이고 창의적으로 작업할 수 있도록 설계된 다양한 내장 기능을 제공합니다.

자세한 내용은 [의 파일 매핑 기본 정보 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## 만약 내가 [!DNL Workfront Fusion] 둘 이상의 첨부 파일이 포함된 이메일을 처리하시겠습니까?

### 답변

를 사용하는 경우 [!UICONTROL 이메일] 모듈 [!UICONTROL 첨부 파일 검색]각 첨부 파일은 시나리오의 나머지 모듈을 통해 개별적으로 전송됩니다. 여러 파일을 한 번에 받는 다른 앱에서도 유사한 모듈을 사용할 수 있습니다.

자세한 내용은 [[!UICONTROL 이메일] 모듈](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## 일부 트리거를 사용하면 시나리오가 즉시 실행될 수 있습니다. &#39;즉시&#39;이란 무슨 뜻이죠?

### 답변

일반적인 시나리오는 지정한 일정에 따라 간격마다(예: 매 시간, 5분마다, 한 달에 한 번 등) 실행됩니다. 특정 서비스에서 데이터를 받은 후 즉시 시나리오를 시작할 수 있는 인스턴트 트리거(webhooks)라는 특수 트리거가 있습니다. 즉각적인 트리거는 매우 유용할 수 있습니다. 가능하면 항상 사용하는 것이 좋습니다. 이러한 기능은 작업 수를 줄이는 데 도움이 됩니다. 수신된 데이터는 다음 예약된 실행을 기다리지 않고 즉시 처리됩니다. 예: [!DNL Google Sheets] 모듈 [!UICONTROL 변경 사항 보기] 셀이 업데이트된 후 즉시 시나리오를 시작합니다.

## 집계자란 무엇입니까?

### 답변

An [!UICONTROL 누적] 데이터를 하나의 컬렉션으로 병합합니다. 예를 들어, 파일은 zip 아카이브로 압축되고 이메일 첨부 파일로 전송됩니다.

자세한 내용은 [[!UICONTROL 누적] 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 수술이란 무엇입니까?

### 답변

작업은 모듈에서 수행하는 모든 작업입니다. 예를 들어, 트리거가 실행될 때마다 및 작업이 작업을 수행할 때마다 작업이 발생합니다.

## 데이터 전송이란 무엇입니까?

### 답변

데이터 전송은 시나리오를 통해 전송된 데이터의 양을 나타냅니다. 예를 들어 FTP에서 100KB 이미지를 검색하고 크기를 50KB로 줄이고 두 이미지를 모두 [!DNL Dropbox]. 이 시나리오에서 사용되는 데이터 양은 150KB입니다.

## 연결이란 무엇입니까?

### 답변

연결은 [!DNL Workfront Fusion] 계정 및 사용할 타사 서비스입니다. 시나리오를 편집할 때 연결을 쉽게 만들 수 있습니다. 연결을 추가하려면 **[!UICONTROL 추가]** 버튼을 클릭하고 단계별 지침을 따릅니다.

자세한 내용은 [연결 정보 [!DNL Adobe Workfront Fusion] 앱 또는 서비스에](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
