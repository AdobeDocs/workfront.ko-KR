---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 스코어카드 만들기
description: 스코어카드는 프로젝트가 이전에 설정한 포트폴리오 기준에 얼마나 잘 부합하는지 측정합니다. 스코어카드는 종종 조직의 임무, 가치 및 전략적 목표를 반영합니다. Portfolio 관리자는 일반적으로 스코어카드 질문과 답변을 정의하여 프로젝트 우선 순위 지정 및 선택 시 의미 있고 가치 있는 질문을 하도록 합니다. An [!DNL Adobe Workfront] 관리자는 포트폴리오 관리자의 권장 사항을 기반으로 스코어카드를 작성합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# 스코어카드 만들기

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

스코어카드는 프로젝트가 이전에 설정한 포트폴리오 기준에 얼마나 잘 부합하는지 측정합니다. 스코어카드는 종종 조직의 임무, 가치 및 전략적 목표를 반영합니다.

Portfolio 관리자는 일반적으로 스코어카드 질문과 답변을 정의하여 프로젝트 우선 순위 지정 및 선택 시 의미 있고 가치 있는 질문이 되도록 합니다. An [!DNL Adobe Workfront] 관리자는 포트폴리오 관리자의 권장 사항을 기반으로 스코어카드를 작성합니다.

서로 다른 프로젝트를 비교할 수 있는 정렬 값을 제공하려면 스코어카드에 대해 선택한 질문과 답변을 수량화할 수 있어야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>현재: [!UICONTROL Business] 이상</p> 
   또는
   <p>새로운 기능: [!UICONTROL Prime] 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td><p>현재: [!UICONTROL Plan]</p>
   또는
   <p>새로운 기능: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

+++

## 스코어카드 만들기

{{step-1-to-setup}}

1. 클릭 **[!UICONTROL 스코어카드]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 새 스코어카드]** 스코어카드 빌더를 시작하고 스코어카드를 만듭니다.

1. 지정 **[!UICONTROL 스코어카드 이름]** 및 a **[!UICONTROL 설명]**.

   스코어카드를 프로젝트와 연결할 때 이름이 표시됩니다. 스코어카드 목록의 스코어카드 이름 옆에 설명이 표시됩니다.

1. 다음을 클릭합니다. **[!UICONTROL 질문 추가]** 드롭다운 메뉴를 사용하여 [!UICONTROL 스코어카드 질문] 섹션에서 질문에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 질문]</td> 
      <td>스코어카드에 포함할 질문을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>이 질문에 가능한 최대 점수를 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 음수 점]</td> 
      <td>이 옵션을 선택하여 다음을 나타냅니다. [!DNL Workfront] 는 가능한 총 포인트에서 뺍니다. 스코어카드의 최대 가능한 점수에 음수 점수를 추가할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 표시 유형]</td> 
      <td>선택 <strong>[!UICONTROL 값(0-100)]</strong> 사용자가 0에서 100 사이의 값을 지정할 수 있는 스코어카드에 숫자 필드를 표시하려는 경우.<p>또는 을 선택합니다 <strong>[!UICONTROL 드롭다운]</strong> 또는 <strong>[!UICONTROL 라디오 단추]</strong> 답변을 만들려면 사용자는 해당 컨트롤을 사용하여 지정할 수 있습니다. 클릭 <strong>[!UICONTROL 답변 추가]</strong>을(를) 입력한 다음 <strong>[!UICONTROL 값]</strong> 이 답변이 충족된 경우 백분율 포인트입니다. 100%를 선택하면 이 질문에 할당된 점수는 완전히 달성됩니다. 이 질문에 할당된 총 점수의 일부만 포함되어 있음을 나타내려면 낮은 백분율 값을 선택합니다. 예를 들어 질문이 10포인트로 평가되고 이 답변이 5포인트로 표시되도록 하려면 값에 대해 50%를 선택합니다.</p>
      <p>선택 <strong>[!UICONTROL 기본값]</strong> 이 답변이 기본 답변임을 표시하려는 경우.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 질문 추가]** 스코어카드에 더 많은 질문과 답변을 추가하려면 동일한 단계를 따르십시오.

   >[!NOTE]
   >
   >질문을 올바른 순서로 끌어다 놓아 스코어카드의 질문을 재정렬할 수 있습니다.

1. 클릭 **[!UICONTROL 저장]** 모든 정보 입력을 마치면

   이렇게 하면 스코어카드가 만들어지고 프로젝트 관리자는 이제 스코어카드를 프로젝트 비즈니스 사례에 첨부할 수 있습니다.

## 프로젝트에 스코어카드 적용

을 가진 사용자 [!UICONTROL 관리] 프로젝트에 대한 권한은 프로젝트에 스코어카드를 적용할 수 있습니다. 스코어카드는 다음에 의해 생성됩니다. [!DNL Workfront] 관리자.

프로젝트에 대한 비즈니스 사례를 만드는 과정의 일부로 스코어카드가 프로젝트에 추가됩니다. 프로젝트에 스코어카드를 추가하는 방법에 대한 자세한 내용은 [프로젝트에 스코어카드를 적용하고 정렬 점수 생성](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

프로젝트 권한에 대한 자세한 내용은 [에서 프로젝트 공유 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
