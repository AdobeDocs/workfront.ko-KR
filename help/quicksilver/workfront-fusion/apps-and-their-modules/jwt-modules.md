---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JWT 모듈
description: 다음 [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app은 제공된 알고리즘을 기반으로 JWT 토큰을 생성하는 모듈을 제공합니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 121aef2ee55597fee2e2adc8250dd0651ea86f17
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] 모듈

다음 [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app은 제공된 알고리즘을 기반으로 JWT 토큰을 생성하는 모듈을 제공합니다.

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

## JWT 모듈 및 해당 필드

### JWT 생성

이 모듈은 선택한 알고리즘을 기반으로 JWT를 생성합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 알고리즘]</td> 
   <td> <p>JWT를 생성할 알고리즘을 선택합니다.</p> <ul>
   <li><b>HS256</b>: SHA-256 해시 알고리즘을 사용하는 HMAC</li>
   <li><b>HS384</b>: SHA-384 해시 알고리즘을 사용하는 HMAC</li>
   <li><b>HS512</b>: SHA-512 해시 알고리즘을 사용하는 HMAC</li>
   <li><b>RS256</b>: SHA-256 해시 알고리즘을 사용하는 RSASSA-PKCS1-v1_5</li>
   <li><b>RS384</b>: SHA-384 해시 알고리즘을 사용하는 RSASSA-PKCS1-v1_5</li>
   <li><b>RS512</b>: SHA-512 해시 알고리즘을 사용하는 RSASSA-PKCS1-v1_5</li>
   <li><b>PS256</b>: SHA-256 해시 알고리즘을 사용하는 RSASSA-PSS(노드 ^6.12.0 또는 &gt;=8.0.0만)</li>
   <li><b>PS384</b>: SHA-384 해시 알고리즘을 사용하는 RSASSA-PSS(노드 ^6.12.0 또는 &gt;=8.0.0만)</li>
   <li><b>PS512</b>: SHA-512 해시 알고리즘을 사용하는 RSASSA-PSS(노드 ^6.12.0 또는 &gt;=8.0.0만)</li>
   <li><b>ES256</b>: P-256 곡선 및 SHA-256 해시 알고리즘을 사용한 ECDSA</li>
   <li><b>ES384</b>: P-384 곡선 및 SHA-384 해시 알고리즘을 사용한 ECDSA</li>
   <li><b>ES512</b>: P-521 곡선 및 SHA-512 해시 알고리즘을 사용한 ECDSA</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload] </td> 
   <td> <p>추가할 각 페이로드 항목에 대해 <b>항목 추가</b> 항목의 키와 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options] </td> 
   <td> <p>추가할 각 옵션 항목에 대해 <b>항목 추가</b> 항목의 키와 값을 입력합니다.</p> <p>다음 키를 사용할 수 있습니다.
   <ul>
   <li><b>알고리즘</b>: (기본값: RS256)</li>
   <li><b>expiresIn</b>: 초 단위 또는 시간 범위를 설명하는 문자열(예: 2일, 10h, 7d)로 표시됩니다. 숫자 값은 초 수로 해석됩니다. 문자열을 사용하는 경우 시간 단위(일, 시간 등)를 제공해야 합니다. 그렇지 않으면 밀리초 단위가 기본적으로 사용됩니다(120은 120밀리초와 같음).</li>
   <li><b>notBefore</b>: 초 단위 또는 시간 범위를 설명하는 문자열(예: 2일, 10h, 7d)로 표시됩니다. 숫자 값은 초 수로 해석됩니다. 문자열을 사용하는 경우 시간 단위(일, 시간 등)를 제공해야 합니다. 그렇지 않으면 밀리초 단위가 기본적으로 사용됩니다(120은 120밀리초와 같음).
</li>
   <li><b>대상자</b></li>
   <li><b>발급자</b></li>
   <li><b>jwtid</b></li>
   <li><b>제목</b></li>
   <li><b>no타임스탬프</b></li>
   <li><b>머리글</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: 경우 <code>true</code>, sign 함수는 페이로드 개체를 직접 수정합니다. 이 기능은 호출이 적용된 후 토큰으로 인코딩되기 전에 페이로드에 대한 원시 참조가 필요한 경우 유용합니다.</li>
   <li><b>allowInsecureKeySizes</b>: 경우 <code>true</code>를 통해 2048년 미만의 모듈러스를 갖는 개인 키를 RSA에 사용할 수 있습니다.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: 경우 <code>true</code>을 사용하면 지정된 알고리즘과 일치하지 않는 비대칭 키를 사용할 수 있습니다. 이 옵션은 이전 버전과의 호환성을 위한 것이므로 피해야 합니다.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>


