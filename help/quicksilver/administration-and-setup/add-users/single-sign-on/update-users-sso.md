---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: 단일 사인온용 사용자 업데이트
description: Workfront에서 단일 사인온용으로 사용자를 업데이트할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# 단일 사인온용 사용자 업데이트

{{important-admin-console-onboard}}

Adobe Workfront 인스턴스에서 SSO(Single Sign-On)가 활성화되면 SSO 자격 증명으로 Workfront에 로그인할 수 있습니다.

SSO 자격 증명과 연결된 사용자로 이미 채워진 기존 시스템이 있는 경우, CSV(쉼표로 구분된 값) 파일을 Workfront으로 가져와서 사용자의 ID를 Workfront으로 가져올 수 있습니다.

Workfront과 SSO 시스템의 통합에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 단일 사인온 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## SSO 사용자 이름

사용하는 SSO 솔루션에 따라 SSO 환경의 사용자 이름을 다음 중 하나로 호출할 수 있습니다.

* SSO 사용자 이름
* Federation ID
* 페더레이션 사용자 이름

Workfront에서 이러한 모든 이름은 사용자 개체의 SSO 사용자 이름 필드에 저장됩니다.

사용자가 SSO 자격 증명을 사용하여 Workfront에 로그인할 수 있도록 Workfront 사용자 이름 외에 SSO 사용자 이름을 포함하도록 프로필을 업데이트해야 합니다.

Workfront 관리자는 사용자 이름 목록을 사용하여 Workfront에서 가져와서 Workfront 사용자의 SSO 사용자 이름 필드를 대량으로 업데이트할 수 있습니다. 이 목록에는 각 사용자의 해당 SSO 사용자 이름과 Workfront 사용자 ID(GUID)가 포함되어 있어야 하며 CSV 또는 TSV 파일로 저장해야 합니다. 이 프로세스는 Workfront의 기존 SSO 사용자 이름을 업데이트하거나, 사용자에 대해 누락된 경우 새 SSO 사용자 이름을 추가합니다.

## 가져오기 파일 준비 {#prepare-the-import-file}

SSO 사용자 이름 필드가 업데이트되어야 하는 Workfront의 모든 사용자에 대한 보고서를 작성하여 가져오기 파일 준비를 시작할 수 있습니다.

1. Workfront에서 사용자 보고서를 작성합니다.

   Workfront에서 사용자 보고서를 작성하는 방법에 대한 지침은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 보고서에서 다음 필드를 선택합니다.

   | 이름 | Workfront 사용자의 전체 이름입니다. |
   |---|---|
   | ID | ID는 Workfront 영숫자 GUID입니다. |
   | SSO 사용자 이름 | 가져오기로 덮어쓰는 사용자 이름이 없도록 하려면 SSO 사용자 이름 필드를 선택합니다. 사용자가 SSO용으로 아직 업데이트되지 않은 경우 이 필드는 모든 사용자에 대해 비어 있어야 합니다. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. 보고서를 저장합니다.
1. 클릭 **내보내기** 를 클릭하여 보고서를 Excel로 내보냅니다.
1. 내보낸 Excel 파일을 열고 SSO 사용자 이름 열의 보고서에서 각 사용자에 대한 SSO 사용자 이름 추가를 시작합니다.

   >[!IMPORTANT]
   >
   >SSO 사용자 이름은 대소문자를 구분합니다.

1. Excel 파일을 제외한 모든 열 제거 **ID** 그리고 **SSO 사용자 이름** 열.

1. 열 헤더를 제거하고 보고서 맨 위에 빈 행이 없는지 확인합니다.

   SSO 사용자 이름으로 Workfront 사용자를 업데이트하는 데 사용하는 파일에는 다음 순서로 2열만 포함해야 합니다.

   * 첫 번째 열에는 Workfront 사용자 ID(Workfront에 있는 대로 사용자 GUID)가 표시됩니다.
   * 두 번째 열에는 SSO 시스템에 표시되는 SSO 사용자 이름이 포함되어야 합니다.
   * 열에는 헤더가 없어야 하며 이름 목록 맨 위에 빈 행이 있으면 안 됩니다.

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. 보고서를 컴퓨터에 CSV 또는 TSV 파일로 저장합니다.

## SSO용 사용자 업데이트 {#update-your-users-for-sso}

SSO용 사용자를 업데이트하는 프로세스는 SSO 사용자 이름 필드가 없는 경우 Workfront 사용자에게 추가되거나, 사용자와 이미 연결된 값이 있는 경우 해당 필드의 값을 업데이트합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** 그런 다음 **Sso용 사용자 업데이트**.

1. 클릭 **파일 선택** 준비된 파일을 찾아보려면

   이 파일을 준비하는 방법에 대한 자세한 내용은 [가져오기 파일 준비](#prepare-the-import-file).

1. 컴퓨터에 저장된 파일을 선택한 다음 **열기**.

   이렇게 하면 모든 사용자가 SSO 자격 증명을 사용하여 Workfront에 로그인할 수 있습니다.

   다음 **허용만 `<SSO Configuration>` 인증** csv에 포함된 모든 사용자에 대해 설정이 활성화됩니다.

## 사용자의 Workfront 사용자 이름 SSO 확인

SSO 사용자 이름 정보가 포함된 사용자 보고서 작성에 대한 지침은 [가져오기 파일 준비](#prepare-the-import-file).

1. SSO 사용자 이름 정보가 포함된 사용자 보고서를 실행합니다.

   SSO 사용자 이름 열은 각 사용자에 대해 채워져 있습니다.

1. SSO 사용자 이름 열의 값이 SSO 서버의 SSO 사용자 이름과 일치하는지 확인합니다.
1. SSO 사용자 이름 열이 비어 있으면 사용자의 SSO 사용자 이름을 업데이트합니다.

   ![](assets/users-with-sso-field-updated.png)

   SSO용 사용자 업데이트에 대한 지침은 [SSO용 사용자 업데이트](#update-your-users-for-sso).
