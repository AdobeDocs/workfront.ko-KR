---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]
description: 이 문서에서는 [!DNL Adobe Workfront Fusion] 초기화, 작업, 커밋 및 롤백과 같은 시나리오가 실행 중입니다.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] 는 관계형 데이터베이스와 유사한 트랜잭션 시스템입니다. 각 시나리오 실행은 초기화 단계로 시작하고 작업 및 커밋/롤백 단계로 구성된 하나 이상의 사이클을 사용하여 계속되며 종료 단계로 끝납니다.

>[!INFO]
>
>**예**
>
>초기화
>
>주기 #1
>
>작업(읽기 또는 쓰기)
>
>커밋 또는 롤백
>
>주기 #2
>
>작업(읽기 또는 쓰기)
>
>커밋 또는 롤백
>
>...
>
>주기 #N
>
>작업(읽기 또는 쓰기)
>
>커밋 또는 롤백
>
>확정

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 초기화

초기화 단계 동안 필요한 모든 연결(데이터베이스에 연결, 이메일 서비스 등)이 생성됩니다. 또한 각 모듈에서 의도한 작업을 수행할 수 있는지 확인합니다.

## 주기

각 사이클은 일련의 작업으로 구성된 분할이 불가능한 작업의 단위를 나타냅니다. 에서 최대 주기 수를 설정할 수 있습니다 [!UICONTROL 시나리오 설정] 패널. 기본 번호는 1입니다.

자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 작업

작업 단계 읽기 및/또는 쓰기 작업이 수행되는 동안:

* 읽기 작업은 미리 정의된 시나리오에 따라 다른 모듈에서 처리되는 서비스에서 데이터를 얻는 것으로 구성됩니다. 예: [!UICONTROL Dropbox] >[!UICONTROL 감시 파일] 모듈은 마지막 시나리오 실행 이후 생성된 새 번들(파일)을 반환합니다.
* 쓰기 작업은 추가 처리를 위해 데이터를 지정된 서비스에 보내는 것으로 구성됩니다. 예: [!DNL Dropbox] >[!UICONTROL 파일 업로드] 모듈에 파일을 [!DNL Dropbox] 폴더를 입력합니다.

## 커밋

모든 모듈에 대해 작업 단계가 성공하면 커밋 단계가 모듈에 의해 수행되는 모든 작업을 커밋하는 동안 시작됩니다. 이것은 [!DNL Workfront Fusion] 성공 시 작업 단계에 포함된 모든 서비스에 정보를 보냅니다.

## 롤백

모듈에서 작업 또는 커밋 단계 중에 오류가 발생하면 단계가 중단되고 롤백 단계가 시작되어 지정된 주기 동안 모든 작업이 무효화됩니다. 일부 모듈은 이러한 모듈에 의해 수행되는 롤백 및 작업을 지원하지 않습니다. 자세한 내용은 [산모듈](#acid-modules) 섹션을 참조하십시오.

## 확정

종료 단계 동안 열린 연결(예: FTP 연결, 데이터베이스 연결 등)이 닫히고 시나리오가 완료됩니다.

## 산모듈

모두 [!DNL Workfront Fusion] 롤백(트랜잭션이라고도 함)을 지원하는 모듈은 ACID 태그로 표시됩니다.

![](assets/acid-modules-350x189.png)

이 태그로 표시되지 않은 모듈은 다른 모듈에서 오류가 발생하면 초기 상태로 되돌릴 수 없습니다. 비산 모듈의 일반적인 예는 다음과 같습니다 [!UICONTROL 이메일] >[!UICONTROL 이메일 보내기] 작업. 전자 메일이 전송되면 전송을 취소할 수 없습니다.
