---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 등급 카드 관리
description: 요금 카드를 사용하면 위치에 따라 역할당 여러 청구 요금을 정의할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 961e0451ce9011a8a9f511d7d5da99368d22d6fb
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# 등급 카드 관리

{{highlighted-preview-article-level}}

요금 카드를 사용하면 위치에 따라 역할당 여러 청구 요금을 정의할 수 있습니다. 각각 청구 요금이 다른 파리에 본사를 둔 디자이너와 뉴욕에 본사를 둔 두 번째 디자이너 역할이 있을 수 있습니다. 하지만 요금 카드의 작업 역할에는 위치가 필요하지 않습니다. 요금 카드의 작업 역할(및 가능한 위치)에 대한 청구 요금에는 유효 날짜도 포함될 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>기존 계획: [!UICONTROL 계획]</p>
       <p>현재 계획: [!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!UICONTROL 재무 데이터]에 대한 액세스 편집</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>공유된 요금 카드를 편집하려면 요금 카드에 대한 관리 권한이 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

## 요금 카드 추가

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**].
1. 클릭 [!UICONTROL **새 요금 카드**]&#x200B;을(를) 클릭한 다음, [!UICONTROL **등급 카드**] 필드입니다. &quot;제목 없는 비율 카드&quot;를 바꿉니다.
1. 카드 화면에서 다음을 클릭합니다. [!UICONTROL **작업 역할 추가**].
1. 대화 상자에서 [!UICONTROL **작업 역할**] 에 대한 청구 요율을 정의합니다.

   기본 청구 요금이 정의된 경우 이 작업 역할에 대한 시스템 레벨 요금을 표시합니다.

   ![새 청구 요금 대화 상자](assets/location-rate-for-rate-card.png)

1. 선택 [!UICONTROL **통화**] 작업 역할의 경우.
1. (선택 사항) [!UICONTROL **위치**] 작업 역할의 경우.
1. 다음에서 [!UICONTROL **청구 요금 1**] 필드에 이 위치에 대한 청구 요금을 입력합니다. 그런 다음 을 클릭합니다. [!UICONTROL **저장**] 청구 요율을 한 번 재정의합니다.

   또는

   클릭 [!UICONTROL **비율 추가**] 유효 일자가 있는 위치별 청구 요율을 더 추가하려면.

1. (조건부) 이 위치에 대해 두 개 이상의 청구 요율을 추가하는 경우 다음 정보를 입력합니다.

   * **[!UICONTROL 청구 요금 1], 2 등:** 해당 기간에 대한 청구 요금 값.
   * **[!UICONTROL 시작일]:** 요금 재정의가 시작되는 날짜입니다.
   * **[!UICONTROL 종료일]:** 요금 재정의가 종료되는 날짜.

     청구 요금 1에는 시작 일자가 없으며 마지막 청구 요금에 종료 일자가 없습니다. 일부 날짜는 자동으로 추가됩니다. 예를 들어, 청구 요금 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 청구 요금 2를 추가하는 경우, 2023년 4월 30일인 종료 일자가 청구 요금 1에 추가되므로 간격이 없습니다.

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.
1. (선택 사항) 다른 위치의 동일한 작업 역할이나 별도의 작업 역할에 대해 다른 청구 요금을 추가하려면 [!UICONTROL **작업 역할 추가**].
1. (선택 사항) 청구 요금을 편집하려면 요금 카드에서 요금을 선택하고 **편집** 아이콘.

## 요금 카드 복사

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**].
1. 목록에서 요금 카드 옆에 있는 확인란을 선택하고 **복사** 아이콘 ![복사 아이콘](assets/copy-icon.png).

   중복 요금 카드가 추가되었습니다. 목록에서 요금 카드 이름을 클릭하여 이름을 변경합니다.

## 전체 요금 카드 삭제

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**].
1. 목록의 요금 카드 옆에 있는 확인란을 선택하고 **삭제** 아이콘 ![삭제 아이콘](assets/delete.png).

   >[!NOTE]
   >
   >프로젝트에 첨부된 요금 카드가 프로젝트에서 삭제됩니다.
