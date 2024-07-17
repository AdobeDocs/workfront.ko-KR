---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "오류: 자동 제공된 사용자가 로그인할 수 없음"
description: 자동 프로비저닝된 사용자가 처음으로 로그인을 시도하고 시스템에서 액세스 수준을 할당하지 않는다는 오류 메시지가 표시되는 경우, 이는 시스템에 요청 라이선스와 연결된 액세스 수준이 부족하기 때문일 수 있습니다. 자동 프로비저닝은 요청 라이선스 유형을 사용하므로 요청 라이선스와 연결된 액세스 수준을 생성하여 이 문제를 해결할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# 오류: 자동 제공된 사용자가 로그인할 수 없음

자동 프로비저닝된 사용자가 처음으로 로그인하려고 하면 다음과 같은 오류가 표시됩니다.

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 문제

시스템이 새 사용자에게 액세스 수준을 할당하지 않습니다.

기본적으로 자동 프로비저닝은 요청 라이선스 유형을 사용합니다. 요청 라이선스가 있는 액세스 수준이 없는 경우 시스템에서 사용자에게 액세스 수준을 할당할 수 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

요청 라이선스를 사용하여 기본 액세스 수준 만들기:

1. **[!UICONTROL 설정]** > **[!UICONTROL 액세스 수준]**(으)로 이동합니다.

1. **[!UICONTROL 새 액세스 수준]**&#x200B;을 클릭하세요.
1. **[!UICONTROL 이름]**&#x200B;을(를) 입력하십시오.
1. **[!UICONTROL 라이선스 유형]** 드롭다운 메뉴에서 요청을 선택합니다.
1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.

요청 라이선스를 사용하여 액세스 수준을 만든 후 사용자에게 SSO 자격 증명으로 로그인하도록 합니다.


