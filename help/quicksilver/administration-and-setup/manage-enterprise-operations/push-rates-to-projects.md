---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 프로젝트에 대한 푸시 비율 변경
description: 요금 카드는 작업을 완료할 작업 역할에 대해 시간당 요금이 정의된 고객과의 계약 계약을 나타냅니다. 요금 카드에서 속성을 기준으로 작업 역할당 여러 청구 요금을 정의할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 6%

---

# 프로젝트에 대한 푸시 비율 변경

요금 카드가 <!--or a staffing plan--> 프로젝트에 첨부된 경우에도 요금 카드의 요금을 조정할 수 있습니다. 그런 다음 선택적으로 해당 요금을 요금 카드가 첨부된 <!--and staffing plans --> 프로젝트에 푸시할 수 있습니다. 새 요금을 푸시하지 않으면 원래 요금이 <!-- or staffing plan--> 프로젝트에 유지됩니다.

프로젝트에 요금 카드를 첨부하는 방법에 대한 자세한 내용은 [프로젝트에 요금 카드 첨부](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td>워크플로 얼티밋</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 등급 카드]에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>공유된 요금 카드를 편집하려면 요금 카드에 대한 관리 권한이 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트에 대한 푸시 비율 변경

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**]&#x200B;를 클릭합니다.
1. 비율 카드 목록에서 비율 카드 이름을 클릭합니다.
1. 비율 카드 > 작업 역할 및 비율 화면에서 비율이 올바른지 확인하고 필요에 따라 비율을 편집합니다.
1. [!UICONTROL **변경 내용 밀어넣기**]&#x200B;를 클릭합니다.
1. [!UICONTROL **모든 프로젝트에 적용**]<!--/staffing plans--> 대화 상자에서 이 요금 카드를 사용하는 모든 <!--and staffing plans --> 프로젝트가 기본적으로 선택됩니다. <!--or staffing plan --> 프로젝트에서 요율 변경 사항을 적용하지 않으려면 선택을 취소해야 합니다.
1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   이제 요금 카드를 사용하는 프로젝트 <!--and staffing plans -->에 새 요금이 반영됩니다.
