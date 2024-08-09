---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 사용자 정의 경비 유형 만들기
description: ' [!DNL Adobe Workfront] 관리자는 사용자 지정 경비 유형을 만들어 작업 및 프로젝트와 관련된 경비를 정의하고 추적할 수 있습니다. 경비는 작업 또는 프로젝트와 연관될 수 있는 비인적 비용입니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 3%

---

# 사용자 정의 비용 유형 만들기

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 관리자는 사용자 지정 경비 유형을 만들어 작업 및 프로젝트와 관련된 경비를 정의하고 추적할 수 있습니다. 경비는 작업 또는 프로젝트와 연관될 수 있는 비인적 비용입니다.

생성하는 경비 유형을 편집하거나 삭제할 수 있습니다. 기본 제공 [!DNL Workfront] 경비 유형을 삭제하거나 편집할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 기본 경비 유형

기본적으로 [!DNL Workfront]에 있는 경비 형식은 삭제하거나 편집할 수 없습니다.

* [!UICONTROL Advertising]
* [!UICONTROL 컨설팅]
* [!UICONTROL 엔터테인먼트]
* [!UICONTROL 일반]
* [!UICONTROL 자료]
* [!UICONTROL 여행]

## 사용자 정의 비용 유형 만들기

{{step-1-to-setup}}

1. **[!UICONTROL 경비 유형]**&#x200B;을 클릭하세요.
1. **[!UICONTROL 새 경비 유형]**&#x200B;을 클릭하세요.
1. 표시되는 **[!UICONTROL 새 경비 유형]** 상자에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>경비의 이름을 지정하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>비용에 대한 설명을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>드롭다운 목록에서 경비 유형의 측정 단위를 선택합니다.</p> <p>다음 측정 단위를 사용할 수 있습니다.</p> 
       <ul> 
        <li>마일</li> 
        <li>킬로미터</li> 
        <li>킬로그램</li> 
        <li>달러</li> 
        <li>달러</li> 
        <li>일</li> 
        <li>기타 - 이 옵션을 선택하면 측정 단위의 이름을 지정하고 측정 단위를 조직에 친숙한 것으로 정의하라는 메시지가 표시됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">요금</td> 
      <td> <p>단위당 가격을 지정합니다. 통화 형식의 필드이며 <strong>[!UICONTROL Calculated Unit]</strong> 필드에 설정된 각 단위의 비용을 나타냅니다. </p> <p>비율은 소수점 뒤에 최대 4개의 숫자가 있는 숫자 값을 포함할 수 있습니다. 예: 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 경비 유형 만들기]**&#x200B;를 클릭합니다.\
   이제 사용자가 경비 유형을 프로젝트 및 작업의 경비와 연결할 수 있습니다.

## 사용자 정의 경비 유형 수정

{{step-1-to-setup}}

1. **[!UICONTROL 경비 유형]**&#x200B;을 클릭하세요.
1. 수정할 경비 유형을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

   **[!UICONTROL 경비 유형 편집]** 대화 상자가 표시됩니다.

1. 원하는 대로 변경한 다음 **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.\
   이제 사용자가 경비 유형을 프로젝트 및 작업의 경비와 연결할 수 있습니다.

경비를 사용하는 방법과 이 방법이 프로젝트 비용에 영향을 주는 방법에 대한 자세한 내용은 [프로젝트 경비 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md) 문서를 참조하십시오.
