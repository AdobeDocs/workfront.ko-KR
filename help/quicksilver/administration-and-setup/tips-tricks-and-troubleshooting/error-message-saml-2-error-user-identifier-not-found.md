---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '오류 메시지: SAML 2.0 오류: 사용자 식별자를 찾을 수 없음'
description: ADFS에 성공적으로 연결할 수 없습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 1%

---

# 오류 메시지: SAML 2.0 오류: 사용자 식별자를 찾을 수 없음

## 문제

ADFS에 성공적으로 연결할 수 없습니다.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>성공적인 테스트 연결을 설정하고 여전히 문제가 발생하는 경우 잘못된 속성 매핑이나 페더레이션 ID에 문제가 있을 수 있습니다. 고객 지원에 문의

## 원인:

ADFS 서버의 클레임이 잘못되었습니다.

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

ADFS 서버에서 이름 ID에 대한 클레임이 있는지 확인합니다.

1. Windows에서 **[!UICONTROL 시작]** > **[!UICONTROL 관리]** > **[!UICONTROL ADFS 2.0 관리]**.\
   ADFS 2.0 관리 대화 상자가 표시됩니다.

1. 선택 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** 왼쪽 창에 있습니다.

1. Adobe Workfront과 관련된 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 클레임 규칙 편집]**.
1. 클레임에 권한이 있는지 확인합니다. **[!UICONTROL 발신 클레임 유형]** 의 **[!UICONTROL 이름 ID]**.

![1.png](assets/1-350x287.png)
