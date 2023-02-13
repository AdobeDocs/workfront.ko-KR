---
title: 암호화
description: Adobe Workfront Fusion Encryptor 모듈을 사용하여 텍스트 데이터를 암호화할 수 있습니다. 현재 AES256 및 PGP(OpenPGP)를 통해 메시지 암호화를 지원합니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 암호화

[!DNL Adobe Workfront Fusion] [!UICONTROL 암호화] 모듈을 사용하면 텍스트 데이터를 암호화할 수 있습니다. 현재 AES256 및 PGP( )를 통해 메시지 암호화를 지원합니다[!UICONTROL OpenPGP]).

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## PGP를 사용한 메시지 암호화 및 암호 해독

PGP를 통해 암호화 및 암호 해독할 때는 키체인을 사용하고 개인 또는 공개 키(또는 둘 다)를 만들어야 합니다.

공개 및 개인 키에 대한 자세한 내용은 [기본 용어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). 키체인에 대한 자세한 내용은 [키 입력 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL 암호화] 모듈 및 해당 필드

구성 시 [!UICONTROL 암호화] 모듈, 다음 필드가 표시됩니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

### PGP 메시지 암호화

이 모듈을 사용하면 공개 키와 개인 키를 사용하여 메시지를 암호화할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 개인 키]</td>
        <td>보낸 사람의 개인 키를 입력합니다. 발신자의 ID를 인증할 수 있습니다.</td>
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

이 모듈을 사용하면 공개 키와 개인 키를 사용하여 메시지 암호를 해독할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 개인 키]</td>
        <td>수신자의 개인 키를 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 공개 키]</td>
        <td>수신자의 공개 키를 입력합니다. 발신자의 ID를 인증할 수 있습니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>해독할 메시지를 매핑합니다.</td>
    </tr>
</table>
