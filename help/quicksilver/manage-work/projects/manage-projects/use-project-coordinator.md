---
title: 프로젝트 코디네이터 공동 작업자 사용
content-type: reference
description: 프로젝트 상태를 모니터링하고 지연 작업을 후속 처리하는 즉시 사용 가능한 AI 공동 작업자인 프로젝트 코디네이터를 사용하는 방법에 대해 알아봅니다.
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 4%

---
# 프로젝트 코디네이터 공동 작업자 사용

{{highlighted-preview-article-level}}

프로젝트 코디네이터는 프로젝트를 모니터링하고 중요한 상태 정보에 대해 이해 당사자에게 알리는 즉시 사용 가능한 AI 공동 작업자입니다.

프로젝트 코디네이터를 사용하면 Workfront 외부에서 에이전트를 구성할 필요가 없습니다.

프로젝트 코디네이터 구성에 대한 지침은 AI 공동 작업자 구성 문서의 [프로젝트 코디네이터 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)을 참조하십시오.

일반적으로 AI 공동 작업자에 대한 정보는 [AI 공동 작업자 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)을 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Select, Prime 또는 Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>프로젝트 코디네이터를 할당하려면 프로젝트에 대한 관리 권한이 있어야 합니다.</td> 
  </tr>
  </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 코디네이터 개요

프로젝트 코디네이터는 프로젝트를 모니터링하고 작업을 계속 진행할 수 있도록 도와줍니다. 프로젝트에 할당되면 관리자가 구성하는 일정에 따라 프로젝트 업데이트를 보냅니다. 업데이트에는 다음이 포함될 수 있습니다.

* 진행률 요약
* 프로젝트 상태
* 지연 또는 위험 상태의 작업 또는 승인
* 누락된 필드 또는 할당

프로젝트 코디네이터는 프로젝트 및 해당 작업에 대해 댓글을 달 수도 있습니다.

관리자는 업데이트 전송 빈도, 전송 시간 및 수신 사용자를 구성합니다.

프로젝트 업데이트에서 프로젝트 코디네이터를 언급하여 요청 시 실행할 수도 있습니다. 해당 시간에 실행하도록 예약되지 않았더라도 언급되면 프로젝트 코디네이터가 실행됩니다.

>[!NOTE]
>
>일반 공급 전에 프로젝트 코디네이터 동작이 변경될 수 있습니다.

## 프로젝트에 프로젝트 코디네이터 추가

먼저 관리자가 프로젝트 코디네이터를 만들고 레이아웃 템플릿의 프로젝트 헤더에 **프로젝트 코디네이터** 필드를 추가해야 합니다. 그러면 프로젝트 헤더에 필드가 나타납니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

프로젝트에 프로젝트 코디네이터를 할당하려면 다음 작업을 수행하십시오.

1. 프로젝트 코디네이터를 지정할 프로젝트로 이동합니다.
1. 프로젝트 헤더에서 **프로젝트 코디네이터** 필드를 클릭합니다.
1. 할당할 프로젝트 코디네이터를 선택합니다.

   선택한 프로젝트 코디네이터에 대한 설명과 프로젝트 코디네이터가 수행하는 작업이 창에 표시됩니다.
1. **적용**&#x200B;을 클릭합니다.

## 프로젝트 코디네이터를 언급하여 실행

예약된 업데이트 외에도 언제든지 프로젝트 코디네이터를 프로젝트의 업데이트에 @mentioning 트리거할 수 있습니다. 프로젝트 코디네이터는 해당 시간에 실행하도록 예약되지 않았더라도 언급되는 즉시 실행됩니다.

프로젝트 코디네이터를 언급하려면

1. 프로젝트 코디네이터가 할당된 프로젝트로 이동합니다.
1. 프로젝트의 **업데이트** 영역을 엽니다.
1. 업데이트 필드에 **@**&#x200B;을(를) 입력하고 프로젝트 코디네이터를 선택합니다.
1. 메시지를 추가한 다음 업데이트를 게시합니다.

   프로젝트 코디네이터가 를 실행하고 응답을 게시합니다.

>[!NOTE]
>
>프로젝트로 트리거하려면 먼저 프로젝트 코디네이터가 프로젝트에 할당되어야 @mention.

## 프로젝트 코디네이터 구성

프로젝트 코디네이터 구성에 대한 지침은 AI 공동 작업자 구성 문서의 [프로젝트 코디네이터 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)을 참조하십시오.
