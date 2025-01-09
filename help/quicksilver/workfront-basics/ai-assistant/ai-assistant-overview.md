---
title: AI Assistant 개요
content-type: reference
description: AI Assistant 개요
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 47469f684bf3be6c6a9d3c39ba3960ca13e43578
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 1%

---

# AI Assistant 개요

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리보기 환경과 월별 릴리스를 활성화한 고객의 프로덕션 환경에서 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

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

<div class="preview">

* Workfront에서 특정 항목을 찾습니다.

  자세한 내용은 [AI Assistant를 사용하여 프로젝트, 작업 및 문제 작업](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md)을 참조하십시오.

</div>

* 계산된 사용자 정의 필드의 수식 생성 또는 세분화

  >[!NOTE]
  >
  >이 기능은 Prime 또는 Ultimate Workfront 플랜의 조직만 사용할 수 있습니다.

  자세한 내용은 [AI Assistant를 사용하여 계산된 필드 수식 생성 또는 수정](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md)을 참조하십시오.

<div class="preview">
* 업데이트, 업로드된 문서 및 기타 주목할 만한 프로젝트 변경 내용을 24시간, 3일, 7일(우선순위) 기간 내에 요약합니다.

자세한 내용은 [우선 순위에서 작업 따라잡기](/help/quicksilver/workfront-basics/priorities/catch-me-up.md)를 참조하십시오.

</div>

## AI Assistant에 사용 가능한 객체 유형

사용자에게 Workfront에서 유효한 권한이 있는 경우 AI 어시스턴트는 다음 오브젝트 유형과 연관된 데이터를 쿼리할 수 있습니다.

* 포트폴리오
* 프로그램
* 프로젝트
* 작업
* 문제
* 사용자 정의 양식
* 사용자
* Workfront 계획 레코드


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
