---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드 인쇄
description: 대시보드를 인쇄하거나 .PDF 파일로 내보낼 수 있습니다. 대시보드를 인쇄하려면 대시보드를 볼 권한이 있어야 합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 대시보드 인쇄

<!-- Audited: 1/2025 -->

대시보드를 인쇄하거나 .PDF 파일로 내보낼 수 있습니다. 대시보드를 인쇄하려면 대시보드를 볼 권한이 있어야 합니다.

>[!NOTE]
>
>이 기능은 표준 대시보드 보기에서만 사용할 수 있습니다. 프로젝트 영역에 포함되어 있거나 사용자 정의 탭으로 설정된 대시보드에는 사용할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스</strong></td> 
      <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>작업 이상</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>보고서, 대시보드 및 캘린더에 대한 액세스 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong>/td&gt; 
   <td> <p>대시보드에 대한 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

대시보드를 인쇄하려면 먼저 만들어야 합니다.

대시보드를 만드는 방법에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)를 참조하십시오.

## 대시보드를 인쇄할 때 인쇄되는 정보 이해

대시보드를 인쇄하거나 .PDF 파일로 저장할 때 대시보드의 일부 정보는 Adobe Workfront 웹 애플리케이션에 표시되므로 인쇄되거나 내보낸 파일에 표시되지 않을 수 있습니다.

* [표시되는 항목](#what-is-displayed)
* [표시되지 않는 것은 무엇입니까?](#what-is-not-displayed)

### 표시되는 항목 {#what-is-displayed}

인쇄되거나 내보낸 대시보드 파일에는 다음 정보가 포함됩니다.

* 대시보드 제목
* 보고서 제목
* 보고서가 마지막으로 생성된 시간의 타임스탬프
* 목록 보기, 외부 웹 페이지, 보고서 및 달력을 포함한 대시보드의 모든 오브젝트
* Workfront 관리자가 전역 탐색 모음에서 회사 로고를 사용자 정의한 경우, 회사의 로고. Workfront 사이트 브랜딩에 대한 자세한 내용은 [Adobe Workfront 인스턴스 브랜딩](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)을 참조하십시오.

### 표시되지 않는 것은 무엇입니까? {#what-is-not-displayed}

다음 정보는 인쇄되거나 내보낸 대시보드 파일에 포함되지 않습니다.

* Workfront 탐색 모음
* Workfront과 관련된 기타 모든 서식
* 보고서의 크기와 개별 열의 수 및 너비에 따라 대시보드를 내보내고 인쇄하면 일부 열이 잘릴 수 있습니다.

## 대시보드 인쇄

1. 인쇄할 대시보드로 이동합니다.
1. 다음 중 하나를 수행합니다.

   * **대시보드 작업** > **인쇄 미리 보기**&#x200B;를 클릭합니다.

   * **Ctrl+P**(Windows의 경우) 또는 **Command+P**(Mac의 경우)을 누릅니다

     >[!IMPORTANT]
     >
     >* 대시보드가 사용자 정의 탭에 임베드된 경우에는 이 두 옵션을 모두 사용할 수 없습니다. 사용자 지정 탭 만들기에 대한 자세한 내용은 [사용자 지정 탭 또는 섹션 만들기](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)를 참조하십시오.
     >* Internet Explorer 브라우저를 사용하는 경우에는 키보드 단축키 옵션을 사용할 수 없습니다.

1. **대상** 필드에서 사용 가능한 다양한 인쇄 옵션 중에서 선택합니다.\
   인쇄 옵션은 사용하는 브라우저 및 브라우저 버전에 따라 다릅니다.

1. (선택 사항) 대시보드를 .PDF 파일로 저장한 다음 **저장**&#x200B;을 클릭하여 .PDF을 저장합니다.\
   대시보드를 .dashboard 파일로 저장하는 방법에 대해 알아보려면 [PDF 내보내기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)를 참조하십시오.

1. **인쇄**&#x200B;를 클릭합니다.
