---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 액세스 수준에서 외부 사용자 라이선스 유형이 누락됨
description: 설치 프로그램의 액세스 수준 아래에 외부 사용자 라이선스 유형이 더 이상 표시되지 않습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 액세스 수준에서 외부 사용자 라이선스 유형이 누락됨

## 문제

설치 프로그램의 액세스 수준 아래에 외부 사용자 라이선스 유형이 더 이상 표시되지 않습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

1. 이동 **[!UICONTROL 설정]** > **[!UICONTROL 시스템]** > **[!UICONTROL 기본 설정]**.

1. 에서 **[!UICONTROL 보안]** 섹션에서 옵션을 확인합니다. **[!UICONTROL 이메일 주소를 사용하여 Workfront 계정이 없는 사람과 공동 작업]** 이 활성화되어 있습니다.

   이 옵션을 활성화하지 않으면 외부 사용자가 액세스 수준 설정에 나타나지 않습니다.
