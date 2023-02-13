---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: ID 공급자에서 SAML 2.0 메타데이터 업데이트
description: ID 공급자에서 SAML 2.0 메타데이터를 업데이트할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# ID 공급자에서 SAML 2.0 메타데이터 업데이트

{{important-admin-console-onboard}}

다음 섹션에서는 ADFS(Active Directory Federation Services)를 ID 공급자로 사용할 때 SAML(Security Assertion Markup Language) 2.0 메타데이터를 업데이트하는 방법에 대해 설명합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ADFS를 ID 공급자로 사용

Adobe Workfront에서 SAML 2.0 인증서를 업데이트하기 전이나 후에 ADFS 메타데이터를 업데이트할 수 있습니다. Workfront에서 SAML 2.0 인증서를 업데이트하기 전에 ADFS 메타데이터를 업데이트하도록 선택하는 경우 추가 단계가 필요합니다.

* [ADFS 메타데이터 업데이트](#update-your-adfs-metadata)
* [ADFS 메타데이터를 강제로 업데이트함](#force-your-adfs-metadata-to-update)

### ADFS 메타데이터 업데이트 {#update-your-adfs-metadata}

자동으로 업데이트되도록 ADFS 메타데이터를 설정하려면 이 섹션의 단계를 완료하십시오.

기본적으로 ADFS는 모든 신뢰 당사자 트러스트 메타데이터에 대한 업데이트를 자동으로 확인하도록 구성되어 있습니다. 하지만, 기본값은 24시간마다 폴링되도록 설정되어 있습니다. powershell 명령을 사용하여 이 값을 변경할 수 있습니다.

1. ADFS 서버에 로그인하고 ADFS 관리 콘솔을 엽니다.
1. 왼쪽 패널에서 를 확장합니다. **ADFS 2.0,** 그런 다음 **신뢰 관계.**

1. 을(를) 클릭합니다. **신뢰 당사자 트러스트** 폴더를 입력합니다.
1. Workfront에서 이전에 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 를 클릭합니다&#x200B;**페더레이션 메타데이터에서 업데이트**.
1. (조건부) 이 옵션이 흐리게 표시되면(메타 데이터 파일을 사용하여 신뢰 당사자 트러스트를 이전에 구성했음을 의미함) 다음을 완료하십시오.

   1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

   1. 클릭 **시스템** > **단일 사인온(SSO)**.

   1. 클릭 **설정 편집.**
   1. 클릭 **구성 편집**&#x200B;를 선택하고 을 선택합니다. **SAML 2.0** 에서 **유형** 드롭다운 목록.

   1. 를 복사합니다. **메타데이터 URL**: 와(과) 유사해야 합니다.

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. ADFS 서버에서 이전에 구성한 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭한 다음 **속성.**
   1. 을(를) 클릭합니다. **모니터링** 탭에서 Workfront에서 복사한 URL을 **신뢰 당사자의 페더레이션 메타데이터 URL** 필드.

   1. 옵션을 선택하여 **신뢰 당사자 모니터링** 및 **신뢰 당사자 자동 업데이트**.

   1. 클릭 **네.**
   1. Workfront에 사용하도록 이전에 구성한 신뢰 당사자 트러스트를 선택합니다. 그런 다음 오른쪽 패널에서 **페더레이션 메타데이터에서 업데이트합니다.**

1. 클릭 **확인** ADFS 2.0에서 지원하지 않는 페더레이션 메타데이터의 일부 컨텐츠에 대한 메시지를 무시합니다.
1. 열기 **Windows Powershell 모듈입니다.**
1. 모든 모듈이 로드되면 powershell에서 다음 명령을 실행하십시오.

   `Get-ADFSProperties`

1. 옆에 있는 값을 찾습니다 **모니터링 간격.**

   폴링 사이의 분 수를 나타내는 숫자가 됩니다. 기본값은 1440(1440분 = 24시간)이어야 합니다.

1. powershell에서 다음 명령을 실행하여 새 값을 설정합니다.

   `Set-ADFSProperties -MonitoringInterval 1`

   이에 따라 모니터링 간격이 24시간마다 변경됩니다. 더 자주 폴링하려면 1을 더 큰 값으로 변경할 수 있습니다.

1. 이 작업이 제대로 작동하는지 확인하려면 **이벤트 뷰어** ADFS2.0 로그에서 다음 정보를 찾으려면

   **이벤트 ID 156 및 157**

### ADFS 메타데이터를 강제로 업데이트함 {#force-your-adfs-metadata-to-update}

ADFS 메타데이터를 업데이트하려면 다음 섹션의 단계를 완료하십시오.

ADFS(Active Directory Federation Services)를 사용할 때 Workfront과 SAML 2.0 공급자 간에 메타데이터를 강제로 교환하려면,

>[!NOTE]
>
>이러한 변경 사항 중 일부는 IT 부서에서 수행해야 할 수 있습니다.

1. ADFS 서버에 로그인하고 **ADFS 관리 콘솔**.
1. 왼쪽 패널에서 를 확장합니다. **ADFS 2.0**&#x200B;를 확장한 다음 **신뢰 관계**.

1. 을(를) 클릭합니다. **신뢰 당사자 트러스트** 폴더를 입력합니다.
1. Workfront에서 이전에 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 를 클릭합니다 **페더레이션 메타데이터에서 업데이트**.

   이 옵션이 흐리게 표시되어 선택할 수 없는 경우 다음을 완료하십시오.

   메타데이터 파일을 사용하여 신뢰 당사자 트러스트를 이전에 구성한 경우에만 옵션이 흐리게 표시됩니다.

   1. Workfront의 설정 영역에서 **메타데이터 URL** Workfront 단일 사인온 설정 화면에서 선택합니다.

      에 대한 정보에 액세스하려면 **메타데이터 URL**:

      1. 클릭 **설정** 전역 탐색 막대의 Adobe Workfront 오른쪽 위 모서리 근처에 있습니다.
      1. > 를 클릭합니다. **시스템** > **단일 사인온(SSO)**.
      1. 클릭 **설정 편집.**
      1. 클릭 **구성 편집**&#x200B;를 선택하고 을 선택합니다. **SAML 2.0** 에서 **유형** 드롭다운 목록.
      1. 를 복사합니다. **메타데이터 URL**: 와(과) 유사해야 합니다.

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. ADFS 서버에서 이전에 구성한 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭한 다음 **속성.**
   1. 을(를) 클릭합니다. **모니터링** 탭에서 Workfront에서 복사한 URL을 **신뢰 당사자의 페더레이션 메타데이터 URL** 필드.
   1. 옵션을 선택하여 **신뢰 당사자 모니터링** 및 **신뢰 당사자 자동 업데이트**.
   1. 클릭 **확인**.
   1. Workfront에서 이전에 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 를 클릭합니다 **페더레이션 메타데이터에서 업데이트합니다.**


1. 클릭 **확인** ADFS 2.0에서 지원하지 않는 페더레이션 메타데이터의 일부 컨텐츠에 대한 메시지를 무시합니다.
1. 클릭 **업데이트** 페더레이션 메타데이터 업데이트를 완료하려면

Workfront 로그인 자격 증명을 사용하여 기본 로그인 화면을 통해 Workfront에 액세스할 수 있는 사용자(다음을 통해)를 **액세스** 섹션)에서 다음 URL로 이동하여 Workfront 사용자 이름과 암호를 사용하여 로그인할 수 있습니다. `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## 다른 ID 공급자 사용

ADFS 이외의 ID 공급자(Ping, Okta 또는 Centrify)를 사용하는 경우 Workfront 메타데이터를 다시 ID 공급자에게 업로드해야 합니다.

새 Workfront 메타데이터 URL을 가져오는 방법에 대한 자세한 내용은 [ADFS 메타데이터 업데이트](#update-your-adfs-metadata).

Workfront에서 SAML 2.0과 함께 ADFS(Active Directory Federation Services)를 사용하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [ADFS를 사용하여 SAML 2.0으로 Adobe Workfront 구성](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
