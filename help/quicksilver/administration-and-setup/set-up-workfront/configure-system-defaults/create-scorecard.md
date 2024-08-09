---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 스코어카드 만들기
description: 스코어카드는 프로젝트가 이전에 설정한 포트폴리오 기준에 얼마나 잘 부합하는지 측정합니다. 스코어카드는 종종 조직의 임무, 가치 및 전략적 목표를 반영합니다. Portfolio 관리자는 일반적으로 스코어카드 질문과 답변을 정의하여 프로젝트 우선 순위 지정 및 선택 시 의미 있고 가치 있는 질문을 하도록 합니다.  [!DNL Adobe Workfront] 관리자가 포트폴리오 관리자의 권장 사항을 기반으로 스코어카드를 작성합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 1%

---

# 스코어카드 만들기

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

스코어카드는 프로젝트가 이전에 설정한 포트폴리오 기준에 얼마나 잘 부합하는지 측정합니다. 스코어카드는 종종 조직의 임무, 가치 및 전략적 목표를 반영합니다.

Portfolio 관리자는 일반적으로 스코어카드 질문과 답변을 정의하여 프로젝트 우선 순위 지정 및 선택 시 의미 있고 가치 있는 질문이 되도록 합니다. [!DNL Adobe Workfront] 관리자는 포트폴리오 관리자의 권장 사항을 기반으로 스코어카드를 만듭니다.

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

1. **[!UICONTROL 스코어카드]**&#x200B;를 클릭한 다음 **[!UICONTROL 새 스코어카드]**&#x200B;를 클릭하여 스코어카드 빌더를 시작하고 스코어카드를 만듭니다.

1. **[!UICONTROL 스코어카드 이름]** 및 **[!UICONTROL 설명]**&#x200B;을 지정하십시오.

   스코어카드를 프로젝트와 연결할 때 이름이 표시됩니다. 스코어카드 목록의 스코어카드 이름 옆에 설명이 표시됩니다.

1. **[!UICONTROL 질문 추가]** 드롭다운 메뉴를 클릭하여 [!UICONTROL 스코어카드 질문] 섹션을 연 다음 질문에 대해 다음 정보를 지정하십시오.

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
      <td>[!DNL Workfront]이(가) 가능한 총 포인트에서 빼야 함을 나타내려면 이 옵션을 선택하십시오. 스코어카드의 최대 가능한 점수에 음수 점수를 추가할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 표시 유형]</td> 
      <td>사용자가 0-100 사이의 값을 지정할 수 있는 스코어카드에 숫자 필드를 표시하려면 <strong>[!UICONTROL Value(0-100)]</strong>을(를) 선택합니다.<p>또는 <strong>[!UICONTROL Drop Down]</strong> 또는 <strong>[!UICONTROL Radio Buttons]</strong>을(를) 선택하여 사용자가 해당 컨트롤을 사용하여 지정할 수 있는 답변을 만듭니다. <strong>[!UICONTROL 답변 추가]</strong>를 클릭한 다음, 충족되는 경우 이 답변에 대한 <strong>[!UICONTROL 값]</strong>(백분율 포인트)을 입력하십시오. 100%를 선택하면 이 질문에 할당된 점수는 완전히 달성됩니다. 이 질문에 할당된 총 점수의 일부만 포함되어 있음을 나타내려면 낮은 백분율 값을 선택합니다. 예를 들어 질문이 10포인트로 평가되고 이 답변이 5포인트로 표시되도록 하려면 값에 대해 50%를 선택합니다.</p>
      <p>이 답변이 기본 답변임을 나타내려면 <strong>[!UICONTROL Default]</strong>을(를) 선택하십시오.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 질문 추가]**&#x200B;를 클릭하여 같은 단계에 따라 스코어카드에 더 많은 질문과 답변을 추가합니다.

   >[!NOTE]
   >
   >질문을 올바른 순서로 끌어다 놓아 스코어카드의 질문을 재정렬할 수 있습니다.

1. 모든 정보 입력을 마치면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이렇게 하면 스코어카드가 만들어지고 프로젝트 관리자는 이제 스코어카드를 프로젝트 비즈니스 사례에 첨부할 수 있습니다.

## 프로젝트에 스코어카드 적용

[!DNL Workfront] 관리자가 스코어카드를 만든 후에는 프로젝트에 대한 [!UICONTROL 관리] 권한이 있는 사용자가 스코어카드를 프로젝트에 적용할 수 있습니다.

프로젝트에 대한 비즈니스 사례를 만드는 과정의 일부로 스코어카드가 프로젝트에 추가됩니다. 프로젝트에 스코어카드를 추가하는 방법에 대한 자세한 내용은 [프로젝트에 스코어카드 적용 및 정렬 점수 생성](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)을 참조하십시오.

프로젝트 권한에 대한 자세한 내용은 [프로젝트 공유 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)를 참조하십시오.
