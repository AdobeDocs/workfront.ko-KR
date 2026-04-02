---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 위치 구성
description: 비율 카드의 작업 역할에 속성으로 지정할 수 있는 기본 위치를 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
source-git-commit: 3fe3313bd545d51be7aa0fb021dd0bb0f91b4321
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 5%

---

# 위치 구성

{{highlighted-preview-article-level}}

비율 카드의 작업 역할에 속성으로 지정할 수 있는 기본 위치를 구성할 수 있습니다. 이렇게 하면 요금 카드가 각 위치의 시장 요금을 정확하게 반영합니다.

요금 카드를 사용하면 조직에서 프로젝트의 청구 요율을 쉽게 관리할 수 있습니다. 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)를 참조하십시오.

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
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 위치 추가

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **위치**]&#x200B;를 클릭합니다.
1. 목록 맨 아래에 있는 [!UICONTROL **위치 추가**]&#x200B;를 클릭합니다.
1. 위치 이름과 설명을 입력합니다.
1. 시작 영역 외부를 클릭하여 위치를 저장합니다.
1. 위치를 삭제하려면 목록에서 해당 위치를 선택하고 **삭제** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.

>[!NOTE]
>
>비율 카드의 작업 역할과 연결된 위치는 삭제할 수 없습니다.

## 하위 위치 추가

기존 위치에 하위 위치를 추가할 수 있습니다. 예를 들어 이미 영국 위치가 있는 경우 London이 하위 위치가 될 수 있습니다.

세 가지 수준의 하위 위치가 허용됩니다. 국가, 시/도 및 도시는 하위 위치의 일반적인 사용입니다.

각 하위 위치는 최상위 위치와 동일한 방식으로 비율 카드에 속성으로 추가하여 해당 위치의 특정 작업 역할에 대한 비율을 정의할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **위치**]&#x200B;를 클릭합니다.
1. 목록에서 기존 위치를 선택하고 **하위 위치 추가**&#x200B;를 클릭합니다.
1. 위치 이름과 설명을 입력합니다.
1. 시작 영역 외부를 클릭하여 위치를 저장합니다.

   하위 위치는 최상위 수준 위치 아래에 들여씁니다.

   ![위치 및 하위 위치](assets/locations-sublocations.png)


