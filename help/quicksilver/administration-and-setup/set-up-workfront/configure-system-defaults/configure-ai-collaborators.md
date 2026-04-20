---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: AI 공동 작업자 구성
description: Adobe Workfront 관리자는 AI 공동 작업자를 구성하고 프로젝트 및 작업에 할당할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: d20215ae2d535ba98ca27ce62aaa28fd372e935a
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 2%

---

# AI 공동 작업자 구성

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

>[!IMPORTANT]
>
>현재 콘텐츠 검토자는 AI Collaborator 유형만 사용할 수 있습니다. 향후 더 많은 AI Collaborator 기능을 사용할 수 있습니다.

AI 공동 작업자는 프로젝트 및 작업에 AI 에이전트를 온보딩하는 방법입니다. AI 공동 작업자를 구성한 다음 사용자와 마찬가지로 할당할 수 있습니다.

예를 들어 브랜드 지침으로 검토자 유형 AI Collaborator를 구성한 다음 해당 Collaborator에 문서를 검토하도록 지정할 수 있습니다.

사용 가능한 AI Collaborator 유형은 다음과 같습니다.

* 검토자: 브랜드 또는 Adobe Brand Intelligence를 사용하여 공동 작업자를 만든 다음 해당 공동 작업자를 에셋에 대한 검토자로 할당합니다.

  자세한 내용은 [Workfront 콘텐츠 검토자 시작](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)을 참조하세요.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Standard, Prime 또는 Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
  </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

* 파일에 Adobe Gen AI 계약에 서명해야 합니다.

  자세한 내용은 Workfront의 AI Assistant 문서에서 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.
* 검토자 유형 AI 공동 작업자에 사용하려면 먼저 Workfront에서 브랜드를 구성해야 합니다.

  지침은 [콘텐츠 검토자를 위한 브랜드 만들기 및 관리](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)를 참조하십시오.
* <span class="preview">검토자 AI 공동 작업자에 Adobe Brand Intelligence를 사용하려면 조직에서 Workfront의 통합 검토 및 승인 환경을 사용해야 합니다. </span>

  <span class="preview">자세한 내용은 [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)을 참조하세요. </span>

## 새 검토자 유형 AI 공동 작업자 만들기

검토자 AI 공동 작업자는 Workfront 브랜드 또는 Adobe Brand Intelligence를 사용하도록 구성할 수 있습니다.

* **브랜드**: 브랜드는 Workfront에서 만들어집니다. 브랜드 지침이 포함된 PDF 파일을 업로드하거나 브랜드 요소를 수동으로 입력하여 Workfront에서 브랜드를 만들 수 있습니다.
* <span class="preview">**Adobe Brand Intelligence**: AI 공동 작업자가 Adobe Brand Intelligence를 사용하여 에셋을 검토할 때 Frame.io에서 검토자가 작성한 댓글을 볼 수 있습니다.  </span>

>[!NOTE]
>
>샌드박스 환경에서는 콘텐츠 검토자를 사용할 수 없습니다.


{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **새 공동 작업자**&#x200B;를 클릭합니다.
1. **검토자**&#x200B;를 클릭한 다음 **계속**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >현재 검토자 유형만 사용할 수 있습니다. 향후 더 많은 AI 공동 작업자 유형을 사용할 수 있습니다.

1. Collaborator Name 필드에 Collaborator의 이름을 입력합니다. 작업에서 사용 가능한 할당자 목록에 표시되는 이름입니다.
1. <span class="preview">검토에 공동 작업자가 브랜드를 사용할지 Adobe Brand Intelligence를 사용할지 여부를 선택합니다.</span>
1. (조건부) AI 공동 작업자가 브랜드를 사용하는 경우 사용할 브랜드 및 브랜드 지침을 선택합니다.
1. **저장**&#x200B;을 클릭합니다.

## AI 공동 작업자 관리

기존 AI 공동 작업자를 편집, 복사 및 삭제할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. (조건부) Collaborator를 편집하려면 편집할 Collaborator의 이름을 클릭하고 Collaborator 편집 창에서 편집한 다음 **저장**&#x200B;을 클릭합니다.
1. (조건부) Collaborator를 복사하려면 복사할 AI Collaborator 행에서 복사 아이콘 ![복사 아이콘](assets/copy-ai-collaborator.png)을 클릭하고 복사 이름을 클릭한 다음 Collaborator 편집 창에서 편집을 수행하고 **저장**&#x200B;을 클릭합니다.
1. (조건부) Collaborator를 삭제하려면 삭제하려는 AI Collaborator 행에서 삭제 아이콘 ![삭제 아이콘](assets/delete-collaborator-icon.png)을 클릭한 다음 **삭제**&#x200B;를 클릭합니다.
