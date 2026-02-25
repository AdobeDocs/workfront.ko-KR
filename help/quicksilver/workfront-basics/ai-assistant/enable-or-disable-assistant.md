---
title: AI Assistant 활성화 또는 비활성화
content-type: reference
description: 조직에서 AI Assistant에 액세스할 수 있는 액세스 수준을 제어할 수 있습니다.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---

# AI Assistant 활성화 또는 비활성화

Workfront 관리자는 조직에서 AI Assistant를 활성화할 사용자를 제어할 수 있습니다. 액세스 수준을 통해 관리됩니다.

액세스 수준에 대해 AI 도우미를 활성화하려면 먼저 조직에 대해 AI 도우미를 활성화해야 합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 조직에 대해 AI Assistant 활성화 또는 비활성화

조직에 대해 AI Assistant를 활성화하려면 다음과 같이 하십시오.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **기본 설정**&#x200B;을 선택하십시오.
1. 아래로 스크롤하여 **AI 환경 설정** 섹션으로 이동합니다.
1. **AI 활성화** 토글을 켭니다.

>[!IMPORTANT]
>
>AI Assistant를 사용하려면 Adobe과 파일에 대해 서명된 Gen AI 계약이 있어야 합니다.
>Gen AI 계약에 대한 자세한 내용은 Workfront의 AI Assistant 문서에서 [Adobe Gen AI 계약에 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.

## 액세스 수준에 대해 AI Assistant 활성화 또는 비활성화

지정된 액세스 수준에 대해 AI Assistant를 활성화하려면 다음과 같이 하십시오.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **액세스 수준**&#x200B;을 선택합니다.
1. 원하는 액세스 수준을 선택한 다음 목록 위에 있는 **편집** ![편집 아이콘](assets/edit-icon.png) 아이콘을 클릭합니다.
1. **액세스 수준 편집** 상자의 **추가 제한 설정...** 영역에서 **Workfront AI Assistant 사용 안 함** 확인란의 선택을 취소합니다.
1. **저장**&#x200B;을 클릭합니다.
1. AI Assistant를 활성화하려는 각 액세스 레벨에 대해 3~5단계를 반복합니다.



>[!NOTE]
>
>* 관리자가 아닌 사용자는 기본적으로 AI Assistant를 사용할 수 없습니다.
>* 관리자가 아닌 사용자가 Workfront에서 AI Assistant 아이콘과 상호 작용하는 경우 관리자가 아닌 사용자에게 약관에 동의할 것을 요청하는 AI Assistant 계약이 표시됩니다. 계약에 동의하면 레이아웃 템플릿에서 AI Assistant가 비활성화되어 있어도 사용할 수 있습니다.

