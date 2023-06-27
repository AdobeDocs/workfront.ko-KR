---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]
description: 이 문서에서는 다음 기간 동안 발생하는 이벤트에 대해 설명합니다. [!DNL Adobe Workfront Fusion] 초기화, 작업, 커밋 및 롤백과 같은 시나리오가 실행 중입니다.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# 의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] 는 관계형 데이터베이스와 유사한 트랜잭션 시스템입니다. 각 시나리오 실행은 초기화 단계로 시작하고, 작업 및 커밋/롤백 단계로 구성된 하나 이상의 주기를 계속하며, 종료 단계로 끝납니다.

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
>완료

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
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
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

## 초기화

초기화 단계에서 필요한 모든 연결(데이터베이스 연결, 이메일 서비스 등)이 생성됩니다. 또한 각 모듈이 의도한 작업을 수행할 수 있는지도 확인합니다.

## 주기

각 주기는 일련의 작업으로 구성된 나눌 수 없는 작업 단위를 나타냅니다. 의 최대 주기 수를 설정할 수 있습니다. [!UICONTROL 시나리오 설정] 패널. 기본 숫자는 1입니다.

자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 작업

작업 단계 동안 읽기 및/또는 쓰기 작업이 수행됩니다.

* 판독 동작은 미리 정의된 시나리오에 따라 다른 모듈에 의해 처리되는 서비스로부터 데이터를 획득하는 것으로 구성된다. 예를 들어 [!UICONTROL Dropbox] >[!UICONTROL 파일 보기] 모듈은 마지막 시나리오 실행 이후 생성된 새 번들(파일)을 반환합니다.
* 쓰기 작업은 추가 처리를 위해 주어진 서비스에 데이터를 전송하는 것으로 이루어진다. 예를 들어 [!DNL Dropbox] >[!UICONTROL 파일 업로드] 모듈이 파일을 [!DNL Dropbox] 폴더를 삭제합니다.

## 커밋

모든 모듈에 대해 작업 단계가 성공하면 모듈에서 수행한 모든 작업이 커밋되는 커밋 단계가 시작됩니다. 이는 다음을 의미합니다. [!DNL Workfront Fusion] 성공 여부에 대한 정보를 작업 단계와 관련된 모든 서비스에 보냅니다.

## 롤백

모듈에서 작업 또는 커밋 단계 중에 오류가 발생하면 단계가 중단되고 롤백 단계가 시작되므로 주어진 주기 동안 모든 작업이 무효화됩니다. 일부 모듈은 롤백을 지원하지 않으며 이러한 모듈에서 수행한 작업은 되돌릴 수 없습니다. 자세한 내용은 [ACID 모듈](#acid-modules) 섹션.

## 완료

완료 단계에서 열린 연결(예: FTP 연결, 데이터베이스 연결 등)이 닫히고 시나리오가 완료됩니다.

## ACID 모듈

모두 [!DNL Workfront Fusion] 롤백을 지원하는 모듈(트랜잭션이라고도 함)은 ACID 태그로 표시됩니다.

![](assets/acid-modules-350x189.png)

이 태그로 표시되지 않은 모듈은 다른 모듈에서 오류가 발생할 때 초기 상태로 되돌릴 수 없습니다. 비 ACID 모듈의 대표적인 예는 다음과 같습니다. [!UICONTROL 이메일] >[!UICONTROL 이메일 보내기] 작업. 이메일을 보낸 후에는 전송을 실행 취소할 수 없습니다.
