---
title: 암호화기
description: Adobe Workfront Fusion Encryptor 모듈을 사용하면 모든 텍스트 데이터를 암호화할 수 있습니다. 현재 AES256 및 PGP(OpenPGP)를 통해 메시지 암호화를 지원합니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 암호화기

[!DNL Adobe Workfront Fusion] [!UICONTROL 암호화기] 모듈을 사용하면 모든 텍스트 데이터를 암호화할 수 있습니다. 현재 AES256 및 PGP([!UICONTROL OpenPGP]).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
  <td> <p>[!UICONTROL Pro] 이상</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
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

## PGP를 이용한 메시지 암호화 및 복호화

PGP를 통해 암호화 및 복호화할 때 키체인을 사용하고 개인 또는 공개 키(또는 둘 다)를 생성해야 한다.

공개 및 개인 키에 대한 자세한 내용은 [의 기본 용어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). 키체인에 대한 자세한 내용은 [의 키 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL 암호화기] 모듈 및 해당 필드

를 구성하는 경우 [!UICONTROL 암호화기] 모듈, 다음 필드가 표시됩니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

### PGP 메시지 암호화

이 모듈에서는 공개 및 개인 키를 사용하여 메시지를 암호화할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 개인 키]</td>
        <td>보낸 사람의 개인 키를 입력합니다. 발신자의 신원을 인증할 수 있습니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 공개 키]</td>
        <td>수신자의 공개 키를 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>암호화할 메시지를 입력합니다.</td>
    </tr>

### PGP 메시지 암호 해독

이 모듈에서는 공개 및 개인 키를 사용하여 메시지의 암호를 해독할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 개인 키]</td>
        <td>수신자의 개인 키를 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 공개 키]</td>
        <td>수신자의 공개 키를 입력합니다. 발신자의 신원을 인증할 수 있습니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>해독할 메시지를 매핑합니다.</td>
    </tr>
</table>
