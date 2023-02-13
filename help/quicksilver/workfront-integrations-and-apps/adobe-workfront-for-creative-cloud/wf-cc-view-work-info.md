---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Adobe Workfront 플러그인을 사용하여 작업 항목 정보 보기
description: Adobe Creative Cloud 애플리케이션에서 프로젝트, 작업, 문제 및 문서에 대한 정보를 볼 수 있습니다.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: a53a716f-4faf-4ea7-a4fc-ad8d87634267
source-git-commit: fc3eb30cef2e17524b5cbd50219861f293a2ea9d
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 3%

---

# 을 사용하여 작업 항목 정보 보기 [!DNL Adobe Workfront] 플러그인

프로젝트, 작업, 문제 및 문서에 대한 정보는 다음과 같습니다 [!DNL Adobe Creative Cloud] 애플리케이션:

{{cc-app-list}}

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <!--<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">제품</td> 
   <td>다음을 수행해야 합니다. [!DNL Adobe Creative Cloud] 라이센스 [!DNL Workfront] 라이센스.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 작업 또는 문제에 대한 [!UICONTROL 보기] 액세스</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보려는 객체에 대한 액세스를 봅니다. </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

{{cc-install-prereq}}

## 세부 사항 및 사용자 지정 양식 데이터 보기

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/go-back-to-work-list-350x314.png)

1. 보려는 작업 항목을 선택합니다.

   >[!TIP]
   >
   >를 사용하십시오 **[!UICONTROL 메뉴]** 아이콘 - 작업 항목의 상위 객체로 이동합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 세부 사항]** 아이콘 ![](assets/details.png) 탐색 막대에서 다음을 볼 수 있습니다.

   * [!UICONTROL 설명]
   * [!UICONTROL 계획된 완료 일자]
   * [!UICONTROL 상태]
   * [!UICONTROL 할당 대상:]
   * [!UICONTROL 프로젝트 소유자] (프로젝트만)
   * 사용자 지정 양식 데이터

## 문서 세부 정보 보기

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/go-back-to-work-list-350x314.png)

1. 보려는 작업 항목을 선택합니다.

   >[!TIP]
   >
   >를 사용하십시오 **[!UICONTROL 메뉴]** 아이콘 - 작업 항목의 상위 객체로 이동합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 문서]** 아이콘 ![](assets/documents.png) 탐색 막대에서 문서를 두 번 클릭하여 봅니다.

   * [!UICONTROL 설명]
   * [!UICONTROL 파일 유형]
   * [!UICONTROL 증명 상태] (증명에만 사용 가능)
   * [!UICONTROL 버전]
   * [!UICONTROL 크기]
   * 사용자 지정 양식 데이터

## 증명 세부 정보 보기

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/go-back-to-work-list-350x314.png)

1. 보려는 작업 항목을 선택합니다.

   >[!TIP]
   >
   >를 사용하십시오 **[!UICONTROL 메뉴]** 아이콘 - 작업 항목의 상위 객체로 이동합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 문서]** 아이콘 ![](assets/documents.png) 탐색 막대에서 증명을 두 번 클릭합니다.

1. 축소판의 오른쪽 위 모서리에 있는 화살표 아이콘을 클릭하여 증명 세부 정보를 [!DNL Workfront].

![Workfront에서 증명 세부 사항 페이지를 엽니다.](assets/go-to-proof-details.png)

## 증명 상태 보기

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/go-back-to-work-list-350x314.png)

1. 보려는 작업 항목을 선택합니다.

   >[!TIP]
   >
   >를 사용하십시오 **[!UICONTROL 메뉴]** 아이콘 - 작업 항목의 상위 객체로 이동합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 문서]** 아이콘 ![](assets/documents.png) 탐색 막대에서 증명을 두 번 클릭합니다.

1. 증명의 현재 상태를 보려면 아래쪽으로 스크롤하십시오. 전송, 열림, 주석, 결정(SOCD) 세부 정보에 대한 자세한 내용은 [문서 세부 정보 개요](/help/quicksilver/documents/managing-documents/document-details-overview.md).

![](assets/proof-status.png)

## 하위 작업 및 문제 보기

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/go-back-to-work-list-350x314.png)

1. 보려는 작업 항목을 선택합니다.

   >[!TIP]
   >
   >를 사용하십시오 **[!UICONTROL 메뉴]** 아이콘 - 작업 항목의 상위 객체로 이동합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 문제]** 아이콘 ![](assets/issues.png) 또는 **하위 작업** 아이콘 ![](assets/subtasks.png).

1. 작업 또는 문제를 선택한 다음 **[!UICONTROL 세부 사항]** 아이콘 ![](assets/details.png) 탐색 막대에서 다음을 볼 수 있습니다.

   * [!UICONTROL 계획된 완료 일자]
   * [!UICONTROL 상태]
   * [!UICONTROL 할당 대상:]
   * 사용자 지정 양식 데이터
