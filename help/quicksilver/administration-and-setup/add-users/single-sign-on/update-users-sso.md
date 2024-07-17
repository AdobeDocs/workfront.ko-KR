---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: SSO(Single Sign-On)를 위해 사용자 업데이트
description: Workfront에서 단일 사인온에 대해 사용자를 업데이트할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 1%

---

# SSO(Single Sign-On)를 위해 사용자 업데이트

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Adobe Workfront 인스턴스에서 SSO(Single Sign-On)를 활성화하면 사용자가 SSO 자격 증명으로 Workfront에 로그인할 수 있습니다.

SSO 자격 증명과 연결된 사용자로 이미 채워진 기존 시스템이 있는 경우 쉼표로 구분된 값(CSV) 파일을 Workfront으로 가져와서 사용자의 ID를 Workfront으로 가져올 수 있습니다.

Workfront과 SSO 시스템을 통합하는 방법에 대한 자세한 내용은 [Adobe Workfront의 Single Sign-On 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)를 참조하십시오.


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
   <td><p>새로운 기능: 표준</p><p>또는</p><p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## SSO 사용자 이름

사용하는 SSO 솔루션에 따라 SSO 환경의 사용자 이름을 다음 중 하나로 호출할 수 있습니다.

* SSO 사용자 이름
* Federation ID
* 페더레이션 사용자 이름

SSO 환경에서 호출되는 사용자 이름에 관계없이 필드의 값은 사용자 객체의 SSO 사용자 이름 필드에 저장됩니다.

사용자가 SSO 자격 증명을 사용하여 Workfront에 로그인할 수 있도록 하려면 Workfront 사용자 이름 외에 SSO 사용자 이름을 포함하도록 프로필을 업데이트해야 합니다.

Workfront 관리자는 사용자 이름 목록을 Workfront으로 가져와서 Workfront 사용자에 대한 SSO 사용자 이름 필드를 대량 업데이트할 수 있습니다. 이 목록은 다음과 같아야 합니다.

* Workfront 사용자 ID(GUID)와 각 사용자에 대한 해당 SSO 사용자 이름을 포함합니다
* CSV 또는 TSV 파일로 저장합니다.

이 프로세스는 Workfront의 기존 SSO 사용자 이름을 업데이트하거나 누락된 경우 새 SSO 사용자 이름을 추가합니다.

## 가져오기 파일 준비 {#prepare-the-import-file}

SSO 사용자 이름 필드를 업데이트해야 하는 Workfront의 모든 사용자에 대한 보고서를 작성하여 가져오기 파일의 준비를 시작할 수 있습니다.

1. Workfront에서 사용자 보고서를 작성합니다.

   Workfront에서 사용자 보고서를 작성하는 방법에 대한 지침은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

1. 보고서에서 다음 필드를 선택합니다.

   | 필드 | 설명 |
   |---|---|
   | 이름 | Workfront 사용자의 전체 이름. |
   | ID | ID는 Workfront 영숫자 GUID입니다. |
   | SSO 사용자 이름 | 가져오기로 덮어쓰는 사용자 이름이 없는지 확인하기 위해 SSO 사용자 이름 필드를 추가합니다. 사용자가 아직 SSO에 대해 업데이트되지 않은 경우 모든 사용자에 대해 이 필드를 비워 두어야 합니다. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. 보고서를 저장합니다.
1. 보고서 상단의 **내보내기**&#x200B;를 클릭하고 보고서를 Excel로 내보냅니다.
1. 내보낸 Excel 파일을 열고 SSO 사용자 이름 열의 보고서에 각 사용자에 대한 SSO 사용자 이름을 추가합니다.

   >[!IMPORTANT]
   >
   >SSO 사용자 이름은 대소문자를 구분합니다.

1. Excel 파일에서 **ID** 및 **SSO 사용자 이름** 열을 제외한 모든 열을 삭제합니다.

1. 열 헤더를 삭제하고 보고서 상단에 빈 행이 없는지 확인합니다.

   SSO 사용자 이름 **must**&#x200B;을(를) 사용하여 Workfront 사용자를 업데이트하는 데 사용 중인 파일에는 다음 순서로 단 2개의 열이 포함되어 있습니다.

   * 첫 번째 열에는 Workfront 사용자 ID(Workfront에 있는 사용자 GUID)가 표시되어야 합니다.
   * 두 번째 열에는 SSO 시스템에 표시되는 SSO 사용자 이름이 있어야 합니다.
   * 열에는 헤더가 없어야 하며 이름 목록의 맨 위에는 빈 행이 없어야 합니다.

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. 보고서를 컴퓨터에 CSV 또는 TSV 파일로 저장합니다.

## SSO를 위해 사용자 업데이트 {#update-your-users-for-sso}

SSO에 대해 사용자를 업데이트하는 프로세스에서는 SSO 사용자 이름 필드가 없는 경우 이 필드를 Workfront 사용자에게 추가하거나 사용자와 이미 연결된 값이 있는 경우 이 필드의 값을 업데이트합니다.

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. **시스템**&#x200B;을 클릭한 다음 **SSO에 대한 사용자 업데이트**&#x200B;를 선택하십시오.

1. **파일 선택**&#x200B;을 클릭하여 준비한 파일을 찾습니다.

   이 파일을 준비하는 방법에 대한 자세한 내용은 [가져오기 파일 준비](#prepare-the-import-file)를 참조하십시오.

1. 컴퓨터에서 파일을 선택한 다음 **열기**&#x200B;를 클릭합니다.

   이렇게 하면 Workfront에 SSO 자격 증명이 삽입되므로 모든 사용자가 SSO 자격 증명을 사용하여 Workfront에 로그인할 수 있습니다.

   CSV에 포함된 모든 사용자에 대해 **`<SSO Configuration>` 인증만 허용** 설정을 사용할 수 있습니다. 이렇게 하면 사용자가 SSO를 통해 로그인해야 합니다.

## 사용자의 Workfront 사용자 이름에 대해 SSO 확인

SSO 사용자 이름 정보가 포함된 사용자 보고서를 작성하는 방법에 대한 지침은 [가져오기 파일 준비](#prepare-the-import-file)를 참조하십시오.

1. SSO 사용자 이름 정보가 포함된 사용자 보고서를 실행합니다.

   각 사용자에 대해 SSO 사용자 이름 열이 채워져 있습니다.

1. SSO 사용자 이름 열의 값이 SSO 서버의 SSO 사용자 이름과 일치하는지 확인하십시오.
1. SSO 사용자 이름 열이 비어 있는 경우 사용자의 SSO 사용자 이름을 업데이트하십시오.

   ![](assets/users-with-sso-field-updated.png)

   SSO에 대한 사용자 업데이트에 대한 지침은 [SSO에 대한 사용자 업데이트](#update-your-users-for-sso)를 참조하십시오.
