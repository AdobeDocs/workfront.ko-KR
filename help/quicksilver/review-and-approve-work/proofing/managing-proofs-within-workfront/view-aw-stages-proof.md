---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명의 자동화된 워크플로우 단계 보기
description: 자동 워크플로우로 구성된 증명 진행 상황을 간편하게 추적할 수 있습니다. 증명의 단계에서 이미 수행된 작업을 보고, 수정하고, 추가하고, 시작하고, 잠글 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# 증명의 자동화된 워크플로우 단계 보기

자동 워크플로우로 구성된 증명 진행 상황을 간편하게 추적할 수 있습니다. 증명의 단계에서 이미 수행된 작업을 보고, 수정하고, 추가하고, 시작하고, 잠글 수 있습니다.

자동화된 워크플로우를 사용하여 증명에 단계 및 사용자를 추가하는 방법에 대한 자세한 내용은 [증명의 자동화된 워크플로우에 단계 및 사용자 추가](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Select 또는 Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 자동화된 워크플로우 다이어그램 보기

1. 문서가 포함된 문서 목록에서 문서가 포함된 행을 마우스로 가리킨 다음 **교정 워크플로**.

   자동화된 워크플로우의 다이어그램은 워크플로우 제목 바로 아래에 표시됩니다.

   다이어그램의 단계는 다음과 같이 표시됩니다.

   ![dot.png](assets/dot.png) 활성 단계

   ![gray_dot.png](assets/grey-dot.png) 비활성 단계\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  비공개 단계

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  잠긴 단계

   단계 사이의 선은 단계 간의 종속성을 나타냅니다. 비활성 단계로 이어지는 선은 단계가 활성화될 때까지 점선으로 표시됩니다.

   다이어그램의 스테이지 위로 마우스를 가져가면 진행 상태를 표시할 수 있습니다. 스테이지가 활성화되어 있지 않고 스테이지에 편집 권한이 있는 경우 단계 활성화 단추를 클릭할 수 있습니다 ![](assets/activate-stage-btn.png) 무대를 시작하기 위해. 스테이지가 활성 상태이고 스테이지에 편집 권한이 있는 경우 스테이지를 잠글 수 있습니다. ![](assets/lock-stage-btn.png) 진행률 표시줄(S, O, C, D)에 대한 자세한 내용은  [Workfront 증명의 진행 상황과 상태 보기](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## 스테이지 보기

1. 문서가 포함된 문서 목록에서 문서가 포함된 행을 마우스로 가리킨 다음 **교정 워크플로**.
1. 다이어그램에서 보려는 단계를 클릭합니다.

   ![](assets/view-stage-diagram-350x204.png)

1. 스테이지에 대한 세부 정보를 확장하려면 해당 이름 아래의 옆쪽 화살표를 클릭합니다.

   ![](assets/stage-details-caret-350x167.png)

## 모든 단계 보기

자동화된 워크플로우에서 모든 단계를 보려면

1. 페이지 상단에 있는 보기 변경 단추를 클릭합니다 ![](assets/change-view-btn.png)를 클릭한 다음 **모든 단계 보기**.

   자동화된 워크플로우의 모든 단계는 섹션에 나열되지만, 세부 사항은 숨겨집니다.

1. 스테이지의 세부 정보를 확장하려면 해당 이름 아래에 있는 옆쪽 화살표를 클릭합니다.

## 모든 단계를 자세히 보기

세부 사항이 확장되어 자동화된 워크플로우의 모든 단계를 보려면 다음을 수행하십시오.

1. 페이지 상단에 있는 보기 변경 단추를 클릭합니다 ![](assets/change-view-btn.png)를 클릭한 다음 **모든 단계를 자세히 보기**.
1. 스테이지의 세부 정보를 보려면 해당 이름 아래의 아래쪽 화살표를 클릭합니다.
