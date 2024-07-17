---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 액세스 수준에서 외부 사용자 라이선스 유형 누락
description: 설정의 액세스 수준에 외부 사용자 라이선스 유형이 더 이상 표시되지 않습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 액세스 수준에서 외부 사용자 라이선스 유형 누락

## 문제

설정의 액세스 수준에 외부 사용자 라이선스 유형이 더 이상 표시되지 않습니다.

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

1. **[!UICONTROL 설정]** > **[!UICONTROL 시스템]** > **[!UICONTROL 환경 설정]**(으)로 이동합니다.

1. **[!UICONTROL 보안]** 섹션에서 **[!UICONTROL 전자 메일 주소를 사용하여 Workfront 계정이 없는 사람들과 공동 작업]** 옵션이 활성화되어 있는지 확인하십시오.

   이 옵션을 활성화하지 않으면 외부 사용자가 액세스 수준 설정에 나타나지 않습니다.
