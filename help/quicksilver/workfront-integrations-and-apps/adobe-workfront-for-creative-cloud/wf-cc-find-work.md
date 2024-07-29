---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Adobe Workfront 플러그인을 사용하여 작업 찾기
description: Adobe Creative Cloud 애플리케이션을 종료하지 않고 Adobe Workfront에서 자신에게 할당된 작업을 찾습니다.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 4abb3257-5f6a-45f6-933b-f3bfb3728f1c
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront] 플러그인을 사용하여 작업 찾기

다음 [!DNL Adobe Creative Cloud]개의 응용 프로그램을 종료하지 않고 [!DNL Adobe Workfront]에서 자신에게 할당된 작업을 찾으십시오.

{{cc-app-list}}

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">제품</td> 
   <td>[!DNL Workfront] 라이선스 외에 [!DNL Adobe Creative Cloud] 라이선스가 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

+++

## 전제 조건

{{cc-install-prereq}}

## [!UICONTROL 작업 목록]을(를) 사용하여 중요 정보에 액세스하세요.

[!UICONTROL 작업 목록]을(를) 통해 할당된 모든 작업과 문제를 한 곳에서 볼 수 있습니다. [!UICONTROL 정렬 기준] 옵션을 사용하여 항목을 함께 그룹화한 다음 [!UICONTROL 필터]를 사용하여 완료해야 하는 작업에 집중할 수 있습니다.

### [!DNL Sort By] 옵션과 함께 유사한 작업 항목 그룹화

[!UICONTROL 정렬 기준] 옵션을 사용하여 [!UICONTROL 작업 목록]에서 유사한 항목을 그룹화합니다. 다음을 기준으로 정렬할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>[!UICONTROL 기한]</li> 
     <li>[!UICONTROL 이름]</li> 
     <li>[!UICONTROL 프로젝트 이름]</li> 
     <li>[!UICONTROL 내 우선 순위]</li> 
    </ul> </td> 
   <td> <img src="assets/copy-of-sort-by-350x606.png" style="width: 350;height: 606;"> </td> 
  </tr> 
 </tbody> 
</table>

### 필터로 초점 좁히기

[!UICONTROL 필터]를 사용하여 특정 작업 항목에 대한 포커스 범위를 좁힙니다. 필터를 사용하는 두 가지 방법이 있습니다.

 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>첫 번째는 작업 항목 유형 또는 속성만을 기반으로 하는 필터링입니다.</p> 
    <ul> 
     <li><strong>작업 항목</strong>: 작업, 하위 작업, 문제 또는 개인 작업</li> 
     <li><strong>작업 항목 상태</strong>: [!UICONTROL 작업 중], [!UICONTROL 시작 준비 완료] 또는 [!UICONTROL 준비 안 됨]</li> 
    </ul> <p>두 번째는 작업 항목과 작업 항목 상태를 함께 사용하여 필터링하는 것입니다. 예를 들어 작업 및 [!UICONTROL 시작할 준비 완료]를 선택하여 작업 목록에서 작업 준비가 된 모든 작업을 찾을 수 있습니다.</p> <p>[!UICONTROL Field Match]를 사용하여 필터 집합 내의 특정 항목을 검색할 수도 있습니다. </p> </td> 
   <td> <img src="assets/copy-of-filter-p-350x603.png" style="width: 350;height: 603;"> </td> 
  </tr> 
 </tbody> 
</table>

## 작업 검색

[!UICONTROL 검색] 막대를 사용하여 필요한 프로젝트, 작업, 문제 및 문서를 찾습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>최근 항목 보기: Workfront의 데스크탑 또는 플러그인 버전을 통해 액세스되는 최신 작업 항목 중 최대 5개를 볼 수 있습니다.</li> 
     <li>고정 항목 찾기: 새 Adobe Workfront 경험에 고정한 프로젝트, 작업, 문제 및 문서에 액세스할 수 있습니다.</li> 
     <li>즐겨찾기 찾기: 즐겨찾기로 저장한 프로젝트, 작업, 문제 또는 문서를 볼 수 있습니다.</li> 
    </ul> </td> 
   <td> <img src="assets/copy-of-search-p.png"> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 메뉴]를 사용하여 프로젝트 탐색

[!UICONTROL 메뉴] 아이콘을 사용하여 프로젝트의 상위 항목으로 이동할 수 있습니다.

![](assets/go-back-to-work-list-350x314.png)
