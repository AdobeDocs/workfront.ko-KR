---
title: 'AI Assistant 개요'
content-type: reference
description: AI Assistant 개요
author: Becky
feature: Get Started with Workfront
source-git-commit: 3db36df88d4bb716cf4c37cd76b6d058a5a6f9b6
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# AI Assistant 개요

Workfront의 AI 어시스턴트는 자연어 대화에서 인앱 정보와 제안을 제공하여 작업을 완수하도록 도와줍니다. AI Assistant는 다음을 통해 더욱 원활한 작업 경험을 제공할 수 있습니다.

* 작업 항목 또는 문서 요약
* 작업 프로세스에 대한 지침 또는 참조 자료 찾기
* 계산된 필드에 대한 수식 생성 또는 확인

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: 사용할 수 없음</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 사용할 수 없음</p></td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.## AI Assistant 사전 요구 사항

## AI Assistant 사전 요구 사항

조직에서 AI Assistant를 활성화하려면 다음 중 **모두**&#x200B;을(를) 적용해야 합니다.

* 조직이 Adobe IMS(Identity Management System)로 마이그레이션되었어야 합니다.
* Adobe 통합 경험을 활성화해야 합니다.
* 조직에 Select, Prime 또는 Ultimate Workfront 플랜이 있어야 합니다.
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.

  계약 서명에 대한 자세한 내용은 이 문서에서 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.

## AI Assistant에 대한 고려 사항

* AI 어시스턴트는 사용자가 연 페이지에 대한 컨텍스트에 따라 다릅니다. 예를 들어 프로젝트 페이지에서 AI Assistant에 &quot;이 프로젝트 요약&quot;을 입력하면 해당 특정 프로젝트에 대한 요약이 반환됩니다.
* Workfront 관리자는 조직의 사용자를 위해 AI Assistant를 활성화해야 합니다. AI Assistant는 액세스 수준을 통해 활성화됩니다.

  자세한 내용은 [AI Assistant 사용 또는 사용 안 함](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)을 참조하십시오.

* Workfront Planning AI Assistant에는 Workfront AI Assistant와 다른 기능이 있습니다.

  Workfront Planning의 AI Assistant에 대한 자세한 내용은 [Adobe Workfront Planning AI Assistant 개요](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)를 참조하십시오.


## AI Assistant에서 사용 가능한 기능

AI Assistant는 현재 다음과 같은 기능을 제공합니다.

* 프로젝트, 작업, 문제 또는 문서 요약

  자세한 내용은 [AI Assistant를 사용하여 요약](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)을 참조하십시오.

* Adobe Experience League의 Workfront 설명서에서 가져온 지침 또는 참조 정보를 제공합니다.

  자세한 내용은 [AI Assistant에서 도움 받기](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)를 참조하십시오.

* 계산된 사용자 정의 필드에 대한 공식을 생성하거나 세분화합니다.

  >[!NOTE]
  >
  >이 기능은 Prime 또는 Ultimate Workfront 플랜의 조직만 사용할 수 있습니다.

  자세한 내용은 [AI Assistant를 사용하여 계산된 필드 수식 생성 또는 수정](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md)을 참조하십시오.

## AI Assistant 액세스

1. Workfront 페이지 맨 위에서 AI Assistant 아이콘 ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)을(를) 클릭합니다.
1. 화면의 오른쪽에 있는 패널에 질문이나 프롬프트를 입력합니다.

   이 패널에 입력할 수 없는 경우 조직은 파일에 서명된 Adobe Gen AI 계약이 없습니다.

1. AI 도우미가 필요한 답변을 제공하지 않는 경우 프롬프트를 세분화하고 다시 시도하십시오.

## Adobe Gen AI 계약 서명

조직에 파일에 대한 서명된 Adobe Gen AI 계약이 없는 경우 조직에 대해 AI Assistant를 활성화할 수 없습니다.

Adobe Gen AI 계약이 서명되지 않은 상태에서 사용자가 AI Assistant를 사용하려고 하면 다음과 같은 메시지가 표시됩니다.

* 사용자: 사용자는 조직에 대해 AI Assistant가 활성화되지 않았으며 Workfront 관리자에게 문의하여 해당 조직에 대해 요청할 수 있다는 알림을 받게 됩니다.
* 관리자: 관리자는 서명된 Adobe Gen AI 계약이 없다는 알림을 받고, 서명을 위해 계약 사본을 보내도록 요청할 수 있습니다.

Adobe Gen AI 계약을 요청하려면

1. Workfront 관리자로서 AI Assistant 아이콘 ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)을(를) 클릭합니다.
1. AI Assistant 패널에서 입력을 시작합니다.
1. Adobe Gen AI 계약 메시지가 나타나면 **계약 검토**&#x200B;를 클릭하십시오.
1. Adobe Gen AI 계약에 서명할 조직의 개인 이름과 이메일 주소를 입력합니다.

   계약서는 서명을 위해 이 개인에게 전송됩니다. 서명되고 반환되면 조직에 대해 AI 비서가 활성화됩니다.

