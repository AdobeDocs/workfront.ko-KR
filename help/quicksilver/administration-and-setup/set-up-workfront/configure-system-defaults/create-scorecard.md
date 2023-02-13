---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 스코어카드 만들기
description: 스코어카드는 프로젝트가 이전에 설정한 포트폴리오 기준에 얼마나 잘 정렬되는지 측정합니다. 스코어카드는 조직의 임무, 가치 및 전략적 목표를 반영하기도 합니다.Portfolio 관리자는 일반적으로 스코어카드 질문과 답변을 정의하여 프로젝트 우선 순위 지정 및 선택 시 의미있고 유용하도록 합니다. An [!DNL Adobe Workfront] 관리자는 포트폴리오 관리자의 권장 사항을 기반으로 스코어카드를 작성합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 스코어카드 만들기

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

스코어카드는 프로젝트가 이전에 설정한 포트폴리오 기준에 얼마나 잘 정렬되는지 측정합니다. 스코어카드는 조직의 사명, 가치 및 전략적 목표를 종종 반영합니다.

Portfolio 관리자는 일반적으로 스코어카드 질문과 답변을 정의하여 프로젝트 우선 순위 지정 및 선택 시 유용하고 의미 있는 결과를 제공합니다. An [!DNL Adobe Workfront] 관리자는 포트폴리오 관리자의 권장 사항을 기반으로 스코어카드를 작성합니다.

서로 다른 프로젝트를 비교하기 위해 정렬 값을 제공하려면 스코어카드에 대해 선택한 질문과 답변을 수량화할 수 있어야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>[!UICONTROL Business] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
 </tbody> 
</table>

## 스코어카드 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 스코어카드]**&#x200B;를 클릭한 다음 **[!UICONTROL 새 스코어카드]** 새 스코어카드를 만들고 스코어카드 빌더를 시작하려면 다음을 수행하십시오.

1. 을(를) 지정합니다 **[!UICONTROL 스코어카드 이름]** 그리고 **[!UICONTROL 설명]**.

   스코어카드를 프로젝트와 연결하면 이름이 표시됩니다. 스코어카드 목록의 스코어카드 이름 옆에 설명이 표시됩니다.

1. 을(를) 클릭합니다. **[!UICONTROL 질문 추가]** 드롭다운 메뉴를 클릭하여 [!UICONTROL 스코어카드 질문] 섹션을 선택한 다음 질문에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Question]</td> 
      <td>스코어카드에 포함할 질문을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>이 질문에 가능한 최대 점을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 음점]</td> 
      <td>이 옵션을 선택하여 [!DNL Workfront] 가능한 총 포인트에서 빼야 합니다. 스코어카드의 가능한 최대 포인트에 음수 점수를 추가할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 표시 유형]</td> 
      <td>선택 <strong>[!UICONTROL 값(0-100)]</strong> 사용자가 0~100 사이의 값을 지정할 수 있는 스코어카드에 숫자 필드를 표시하려면 이 필드를 표시할 수 있습니다.<p>또는 을 선택합니다 <strong>[!UICONTROL 드롭다운]</strong> 또는 <strong>[!UICONTROL 라디오 단추]</strong> 응답 만들기 위해 사용자는 해당 컨트롤을 사용하여 지정할 수 있습니다. 클릭 <strong>[!UICONTROL 답변 추가]</strong>를 입력한 다음 를 입력합니다 <strong>[!UICONTROL Value]</strong> 이 응답이 이행되었을 경우 이 응답에 대한 백분율 포인트. 100%를 선택하면 이 문제에 할당된 포인트 수가 모두 충족됩니다. 이 질문에 할당된 총 포인트 금액의 일부만 이 응답에 포함된다는 것을 나타내려면 낮은 백분율 값을 선택합니다. 예를 들어, 질문 값이 10포인트인 경우 이 대답이 해당 포인트 중 5포인트를 차지하도록 하려면 값에 대해 50%를 선택합니다.</p>
      <p>선택 <strong>[!UICONTROL Default]</strong> 이 응답이 기본 응답임을 나타내려면</strong></p>
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 질문 추가]** 스코어카드에 대한 추가 질문 및 답변을 추가하려면 동일한 단계를 따르십시오.

   >[!NOTE]
   >
   >질문을 올바른 순서로 끌어다 놓아 스코어카드에서 질문을 다시 정렬할 수 있습니다.

1. 클릭 **[!UICONTROL 저장]** 데이터 입력을 마치면 됩니다.

## 프로젝트에 스코어카드 적용

을 사용하는 사용자 [!UICONTROL 관리] 프로젝트에 대한 권한은 스코어카드가 [!DNL Workfront] 관리자

프로젝트에 대한 비즈니스 사례를 만드는 과정의 일부로 스코어카드가 프로젝트에 추가됩니다. 프로젝트에 스코어카드를 추가하는 방법에 대한 자세한 내용은 [프로젝트에 스코어카드를 적용하고 정렬 점수를 생성합니다](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

스코어카드 만들기에 대한 자세한 내용은 [스코어카드 만들기](#create-a-scorecard).

프로젝트 권한에 대한 자세한 내용은 [에서 프로젝트 공유 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
