---
title: 프로젝트 코디네이터 공동 작업자 사용
content-type: reference
description: 프로젝트 상태를 모니터링하고 지연 작업을 후속 처리하는 즉시 사용 가능한 AI 공동 작업자인 프로젝트 코디네이터를 사용하는 방법에 대해 알아봅니다.
author: Becky
feature: Work Management, Projects
source-git-commit: a4dfe29c0cf85f6029fd5f4398942c60bd3d6b5a
workflow-type: tm+mt
source-wordcount: '351'
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
   <td>제품 코디네이터를 할당하려면 프로젝트에 대한 관리 권한이 있어야 합니다.</td> 
  </tr>
  </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 코디네이터 개요

프로젝트 코디네이터는 프로젝트를 모니터링하고 주도적으로 작업을 추적하는 데 도움이 되는 가상 프로젝트 관리자(VPM)입니다. 프로젝트 소유자로 할당되면 다음과 같은 결과가 발생합니다.

* 프로젝트 상태를 검토하고 기한 초과 및 정체 작업을 식별합니다
* 작업 소유자에게 상태 업데이트 요청을 보냅니다.
* 기본 필드 및 사용자 정의 양식의 불완전한 정보에 플래그 지정
* 승인 문제, 양식 누락 또는 비활성 문서에 대한 모니터링
* 전임 작업이 종속 항목을 위험에 빠뜨릴 때 작업 종속성 및 플래그를 추적합니다.
* 프로젝트 업데이트 스트림에 업데이트 및 후속 작업을 게시합니다.
* 프로젝트 소유자에게 프로젝트 문제를 알립니다.

공동 작업자가 수행하는 작업과 프로젝트 상태를 확인하는 빈도를 포함하여 동작을 구성할 수 있습니다.

## 프로젝트에 프로젝트 코디네이터 추가

프로젝트 코디네이터 필드는 기본적으로 프로젝트 헤더에 나타납니다. 프로젝트에 프로젝트 코디네이터를 할당하려면 다음 작업을 수행하십시오.

1. 프로젝트 코디네이터를 지정할 프로젝트로 이동합니다.
1. 프로젝트 헤더에서 **프로젝트 코디네이터** 필드를 클릭합니다.
1. 할당할 프로젝트 코디네이터를 선택합니다.

   선택한 프로젝트 코디네이터에 대한 설명과 프로젝트 코디네이터가 수행하는 작업이 창에 표시됩니다.
1. **적용**&#x200B;을 클릭합니다.

## 프로젝트 코디네이터 구성

프로젝트 코디네이터 구성에 대한 지침은 AI 공동 작업자 구성 문서의 [프로젝트 코디네이터 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-the-project-coordinator)을 참조하십시오.
