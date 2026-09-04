---
title: Workfront에서 CX Coworker 사용
content-type: reference
description: Workfront에서 CX Coworker를 사용하는 방법을 알아봅니다.
author: Becky
feature: Get Started with Workfront
source-git-commit: b88f894ad1d30382e9cb62e680d8eb87a858610f
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 3%

---

# Workfront에서 CX Coworker 사용

{{preview-fast-release-general}}

>[!IMPORTANT]
>
>CX Coworker 는 현재 의료 서비스, 금융 기관 또는 중요한 데이터가 있는 기타 업계 조직에서 사용할 수 없습니다. 이러한 조직에서는 AI Assistant를 사용할 수 있습니다. 자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.

Workfront 내에서 CX Coworker에 액세스할 수 있습니다.

Workfront에서 Coworker를 사용할 때 다음과 같은 정보 및 개체로 작업할 수 있습니다.

* Workfront 또는 Workfront Planning입니다.
* 에 대한 권한이 있습니다.

Coworker는 대규모 Adobe CX 엔터프라이즈 에코시스템의 일부이므로 Coworker를 사용하여 Workfront의 오른쪽 레일에서 다른 Adobe 제품의 정보 및 개체로 작업하거나 Workfront에서 Adobe CX Coworker 인터페이스로 이동할 수 있습니다.

Workfront 외부의 Coworker 및 기능에 대한 자세한 내용은 [Adobe CX Enterprise Coworker 채팅 개요](https://experienceleague.adobe.com/ko/docs/cx-enterprise-coworker/content/chat/overview)를 참조하십시오.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

* CX Coworker에서 Workfront 개체와 상호 작용하려면 먼저 해당 개체에 대한 기존 액세스 및 권한이 있어야 합니다. 예를 들어 Coworker에서 프로젝트에 대한 정보를 보려면 적어도 보기 액세스 권한이 있어야 합니다.
* CX Coworker를 통해 Workfront에서 변경 작업을 수행하려면 먼저 Workfront 관리자가 조직의 시스템 환경 설정에서 MCP 작성 도구 옵션을 활성화해야 합니다. 기본적으로 CX Coworker에는 읽기 전용 기능이 있습니다.

  자세한 내용 및 지침은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.


## Workfront에서 CX Coworker 사용

1. Workfront 페이지 맨 위에서 CX Coworker 아이콘 ![AI 아이콘](assets/ai-icon.png)을 클릭합니다.
1. 화면의 오른쪽에 있는 패널에 질문이나 프롬프트를 입력합니다.

1. Coworker에서 필요한 답변을 제공하지 않는 경우 프롬프트를 구체화하고 다시 시도하십시오.

   예를 들어 프롬프트는 문서 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)에서 프롬프트를 참조하십시오.
1. 채팅 입력 상자에서 다음 작업 중 하나를 사용합니다.

   * **+(첨부)**: 첨부 메뉴를 열어 메시지에 파일 또는 데이터 개체를 추가합니다.
   * **계획 모드**: 단계별 계획을 제안하고 실행하기 전에 승인을 일시 중지하도록 동료 채팅에 요청하십시오. 동료 채팅이 직접 작동하도록 하려면 이 기능을 끕니다.
   * **성적 증명서 보기**: Coworker Chat의 내부 활동(보통, 포커스 또는 세부 정보)을 표시할 정도를 제어합니다.
   * **마이크**: 음성 입력으로 메시지를 받아쓰십시오. 레코딩을 중단하려면 다시 선택하십시오.
   * **보내기**: 메시지를 보냅니다. Coworker Chat이 응답하는 동안 이 옵션은 중단하는 데 사용할 수 있는 Stop 컨트롤이 됩니다.

   이러한 작업에 대한 자세한 내용은 Adobe CX 동료 설명서의 [채팅 입력 상자](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide#the-chat-input-box)를 참조하십시오.

1. 이전 채팅을 보고 관리하려면 CX Coworker 패널에서 채트 아이콘 ![채트 아이콘](assets/ai-icon.png)을 클릭하십시오.

   채팅에 대한 자세한 내용은 Adobe CX Coworker 설명서에서 [채팅 관리](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide#manage-your-chats)를 참조하십시오.
1. 출력 목록과 같은 채팅 아티팩트를 보고 관리하려면 아티팩트 아이콘 ![아티팩트 아이콘](assets/artifacts-icon.png)을 클릭하세요.

   CX Coworker의 아티팩트에 대한 자세한 내용은 Adobe CX Coworker 설명서에서 [아티팩트](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide#artifacts)를 참조하십시오.
1. Coworker의 설정을 관리하려면 설정 아이콘 ![설정](assets/coworker-settings-icon.png)을 클릭하세요.
1. Coworker 패널을 확장하려면 확장 아이콘 ![확장 아이콘](assets/coworker-expand-icon.png)을 클릭합니다.
1. Adobe CX Coworker 인터페이스로 이동하려면 페이지 오른쪽 상단에 있는 앱 아이콘 ![앱 아이콘](assets/apps-icon.png)을 클릭하고 사용 가능한 앱 목록에서 Coworker를 선택합니다.
