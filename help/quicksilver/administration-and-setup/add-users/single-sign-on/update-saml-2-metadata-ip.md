---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: ID 공급자에서 SAML 2.0 메타데이터 업데이트
description: ID 공급자에서 SAML 2.0 메타데이터를 업데이트할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 93f4c1691210d88531fcc269bd40ee7ed8633309
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# ID 공급자에서 SAML 2.0 메타데이터 업데이트

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Adobe Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다.
>
>Adobe Admin Console에 온보딩된 조직의 사용자 특성을 매핑하려면 사용자 특성 매핑 문서에서 [Adobe 통합 경험에서 사용자 특성 매핑](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience)을 참조하십시오.

다음 섹션에서는 ID 공급자로 ADFS(Active Directory Federation Services)를 사용할 때 SAML(Security Assertion Markup Language) 2.0 메타데이터를 업데이트하는 방법에 대해 설명합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## ADFS를 ID 공급자로 사용

Adobe Workfront이 SAML 2.0 인증서를 업데이트하기 전 또는 그 후에 ADFS 메타데이터를 업데이트할 수 있습니다. Workfront이 SAML 2.0 인증서를 업데이트하기 전에 ADFS 메타데이터를 업데이트하도록 선택하는 경우 추가 단계가 필요합니다.

* [ADFS 메타데이터 업데이트](#update-your-adfs-metadata)
* [ADFS 메타데이터 강제 업데이트](#force-your-adfs-metadata-to-update)

### ADFS 메타데이터 업데이트 {#update-your-adfs-metadata}

자동으로 업데이트되도록 ADFS 메타데이터를 설정하려면 이 섹션의 단계를 완료하십시오.

기본적으로 ADFS는 모든 신뢰 당사자 트러스트 메타데이터에 대한 업데이트를 자동으로 확인하도록 구성되지만 기본값은 24시간마다 폴링하도록 설정됩니다. powershell 명령을 사용하여 이 값을 변경할 수 있습니다.

1. ADFS 서버에 로그인하고 ADFS 관리 콘솔을 엽니다.
1. 왼쪽 패널에서 **ADFS 2.0,**&#x200B;을 확장한 다음 **트러스트 관계**&#x200B;를 확장합니다.

1. **신뢰 당사자 트러스트** 폴더를 클릭합니다.
1. 이전에 Workfront에서 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 **페더레이션 메타데이터에서 업데이트**&#x200B;를 클릭합니다.
1. (조건부) 이 옵션이 흐리게 표시되면(신뢰 당사자 트러스트가 이전에 메타데이터 파일을 사용하여 구성되었음을 의미함) 다음 단계를 완료합니다.

   1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **설정** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

   1. **시스템** > **SSO(Single Sign-On)**&#x200B;를 클릭합니다.

   1. **설정 편집**&#x200B;을 클릭합니다.
   1. **구성 편집**&#x200B;을 클릭한 다음 **유형** 드롭다운 목록에서 **SAML 2.0**&#x200B;을(를) 선택합니다.

   1. **메타데이터 URL**&#x200B;을(를) 복사합니다. 복사한 값은 다음과 유사해야 합니다.

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. ADFS 서버에서 이전에 구성한 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭한 다음 **속성**&#x200B;을 클릭합니다.
   1. **모니터링** 탭을 클릭한 다음 Workfront에서 복사한 URL을 **신뢰 당사자의 페더레이션 메타데이터 URL** 필드에 붙여 넣습니다.

   1. **신뢰 당사자 모니터링** 및 **신뢰 당사자 자동 업데이트**&#x200B;에 대한 옵션을 확인하십시오.

   1. **확인**&#x200B;을 클릭합니다.
   1. 이전에 Workfront에서 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 **페더레이션 메타데이터에서 업데이트**&#x200B;를 클릭합니다.

1. ADFS 2.0에서 지원하지 않는 페더레이션 메타데이터의 일부 콘텐츠에 대한 메시지를 무시하려면 **확인**&#x200B;을 클릭하십시오.
1. **Windows Powershell 모듈을 엽니다.**
1. 모든 모듈이 로드되면 powershell에서 다음 명령을 실행합니다.

   `Get-ADFSProperties`

1. **모니터링 간격 옆의 값을 찾습니다.**

   투표 사이의 분 수를 나타내는 숫자가 될 것이다. 기본값은 1440(1440분 = 24시간)이어야 합니다.

1. powershell에서 다음 명령을 실행하여 새 값을 설정합니다.

   `Set-ADFSProperties -MonitoringInterval 1`

   그러면 모니터링 간격이 24시간에서 1분마다 변경됩니다. 폴링 빈도를 줄이려면 1을 다른 큰 값으로 변경할 수 있습니다.

1. 이 기능이 올바르게 작동하는지 확인하려면 **이벤트 뷰어**&#x200B;를 사용하여 ADFS2.0 로그에서 다음 정보를 찾으십시오.

   **이벤트 ID 156 및 157**

### ADFS 메타데이터 강제 업데이트 {#force-your-adfs-metadata-to-update}

ADFS 메타데이터를 업데이트하려면 다음 섹션의 단계를 완료하십시오.

ADFS(Active Directory Federation Services)를 사용할 때 Workfront과 SAML 2.0 공급자 간에 메타데이터를 강제로 교환하려면 다음을 수행하십시오.

>[!NOTE]
>
>이러한 변경 사항 중 일부는 IT 부서에서 수행해야 할 수 있습니다.

1. ADFS 서버에 로그인하고 **ADFS 관리 콘솔**&#x200B;을 엽니다.
1. 왼쪽 패널에서 **ADFS 2.0**&#x200B;을 확장한 다음 **트러스트 관계**&#x200B;을 확장합니다.

1. **신뢰 당사자 트러스트** 폴더를 클릭합니다.
1. 이전에 Workfront에서 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 **페더레이션 메타데이터에서 업데이트**&#x200B;를 클릭합니다.

   이 옵션이 흐리게 표시되어 선택할 수 없는 경우 다음을 완료하십시오.

   (신뢰 당사자 트러스트가 이전에 메타데이터 파일을 사용하여 구성된 경우에만 옵션이 흐리게 표시됩니다.)

   1. Workfront의 설정 영역에서 Workfront Single Sign-On 설정 화면에서 **메타데이터 URL**&#x200B;을 복사합니다.

      **메타데이터 URL**&#x200B;에 대한 정보에 액세스하려면:

      1. 전역 탐색 모음에서 Adobe Workfront 오른쪽 상단 근처에 있는 **설정**&#x200B;을 클릭합니다.
      1. > **시스템** > **SSO(Single Sign-On)**&#x200B;를 클릭합니다.
      1. **설정 편집**&#x200B;을 클릭합니다.
      1. **구성 편집**&#x200B;을 클릭한 다음 **유형** 드롭다운 목록에서 **SAML 2.0**&#x200B;을(를) 선택합니다.
      1. **메타데이터 URL**&#x200B;을(를) 복사합니다. 복사한 값은 다음과 유사해야 합니다.

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. ADFS 서버에서 이전에 구성한 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭한 다음 **속성**&#x200B;을 클릭합니다.
   1. **모니터링** 탭을 클릭한 다음 Workfront에서 복사한 URL을 **신뢰 당사자의 페더레이션 메타데이터 URL** 필드에 붙여 넣습니다.
   1. **신뢰 당사자 모니터링** 및 **신뢰 당사자 자동 업데이트**&#x200B;에 대한 옵션을 확인하십시오.
   1. **확인**&#x200B;을 클릭합니다.
   1. 이전에 Workfront에서 사용하도록 구성한 신뢰 당사자 트러스트를 선택한 다음 오른쪽 패널에서 **페더레이션 메타데이터에서 업데이트**&#x200B;를 클릭합니다.

1. ADFS 2.0에서 지원하지 않는 페더레이션 메타데이터의 일부 콘텐츠에 대한 메시지를 무시하려면 **확인**&#x200B;을 클릭하십시오.
1. 페더레이션 메타데이터 업데이트를 완료하려면 **업데이트**&#x200B;를 클릭하십시오.

Workfront 로그인 자격 증명을 사용하여 기본 로그인 화면을 통해 Workfront에 액세스할 수 있는 사용자(**액세스** 섹션의 각 사용자 프로필 페이지에서 구성할 수 있음)는 다음 URL로 이동하여 Workfront 사용자 이름과 암호를 사용하여 로그인할 수 있습니다. `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## 다른 ID 공급자 사용

ADFS 이외의 ID 공급자(예: Ping, Okta 또는 Centrify)를 사용하는 경우 Workfront 메타데이터를 ID 공급자에게 다시 업로드해야 합니다.

새 Workfront 메타데이터 URL을 얻는 방법에 대한 자세한 내용은 [ADFS 메타데이터 업데이트](#update-your-adfs-metadata)를 참조하십시오.

Workfront에서 SAML 2.0과 함께 ADFS(Active Directory Federation Services)를 사용하는 방법에 대한 자세한 내용은 [ADFS를 사용하여 SAML 2.0과 함께 Adobe Workfront 구성](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)을 참조하십시오.
