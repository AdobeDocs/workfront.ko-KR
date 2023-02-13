---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 사용자 지정 비용 유형 만들기
description: 로서의 [!DNL Adobe Workfront] 관리자는 사용자 정의 비용 유형을 만들어 작업 및 프로젝트와 관련된 비용을 정의하고 추적할 수 있습니다. 비용은 업무 또는 프로젝트와 연계될 수 있는 비인적 비용입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# 사용자 지정 비용 유형 만들기

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

로서의 [!DNL Adobe Workfront] 관리자는 사용자 정의 비용 유형을 만들어 작업 및 프로젝트와 관련된 비용을 정의하고 추적할 수 있습니다. 비용은 업무 또는 프로젝트와 연계될 수 있는 비인적 비용입니다.

생성한 비용 유형을 편집하거나 삭제할 수 있습니다. 기본 제공 항목은 삭제하거나 편집할 수 없습니다 [!DNL Workfront] 비용 유형.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 비용 유형

에 있는 비용 유형 [!DNL Workfront] 기본적으로 다음을 포함하거나 삭제하거나 편집할 수 없습니다.

* [!UICONTROL 광고]
* [!UICONTROL 컨설팅]
* [!UICONTROL 엔터테인먼트]
* [!UICONTROL 일반]
* [!UICONTROL 자료]
* [!UICONTROL 여행]

## 사용자 지정 비용 유형 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront].
1. 클릭 **[!UICONTROL 비용 유형]**.
1. 클릭 **[!UICONTROL 새 비용 유형]**.
1. 에서 **[!UICONTROL 새 비용 유형]** 표시되는 상자에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>비용 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>비용에 대한 설명을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>드롭다운 목록에서 비용 유형에 대한 측정 단위를 선택합니다.</p> <p>다음 측정 단위를 사용할 수 있습니다.</p> 
       <ul> 
        <li>마일</li> 
        <li>킬로미터</li> 
        <li>킬로그램</li> 
        <li>달러</li> 
        <li>달러</li> 
        <li>일</li> 
        <li>기타 - 이 옵션을 선택하면 측정 단위에 이름을 지정하고 측정 단위를 조직에 익숙한 것으로 정의하라는 메시지가 표시됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">요금</td> 
      <td> <p>단위당 가격을 지정합니다. 통화 형식 필드이며, <strong>[!UICONTROL Calculated Unit]</strong> 필드. </p> <p>비율에는 소수점 뒤에 최대 4개의 숫자를 사용하는 숫자 값이 포함될 수 있습니다. 예, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 비용 유형 생성]**.\
   이제 사용자가 프로젝트 및 작업에 대한 비용과 비용 유형을 연결할 수 있습니다.

## 사용자 지정 비용 유형 수정

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront].
1. 클릭 **[!UICONTROL 비용 유형]**.
1. 수정할 비용 유형을 선택한 다음 **[!UICONTROL 편집]**.

   다음 **[!UICONTROL 비용 유형 편집]** 대화 상자가 표시됩니다.

1. 원하는 대로 변경한 다음 **[!UICONTROL 변경 내용 저장]**.\
   이제 사용자가 프로젝트 및 작업에 대한 비용과 비용 유형을 연결할 수 있습니다.

비용 사용 방법 및 프로젝트 비용에 영향을 줄 수 있는 방법에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 비용 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md).
