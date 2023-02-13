---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드 인쇄
description: 대시보드를 인쇄하거나 .PDF 파일로 내보낼 수 있습니다. 대시보드를 인쇄하려면 대시보드를 볼 수 있는 권한이 있어야 합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: efae17458f2aa08ca2286ef5e43c68d1f9334b7b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# 대시보드 인쇄

대시보드를 인쇄하거나 .PDF 파일로 내보낼 수 있습니다. 대시보드를 인쇄하려면 대시보드를 볼 수 있는 권한이 있어야 합니다.

>[!NOTE]
>
>이 기능은 표준 대시보드 보기에서만 사용됩니다. 프로젝트 영역에 포함되거나 사용자 지정 탭으로 설정된 대시보드에는 사용할 수 없습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>보고서, 대시보드 및 달력에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong>/td&gt; 
   <td> <p>대시보드에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

대시보드를 인쇄하려면 먼저 대시보드를 만들어야 합니다.

대시보드 만들기에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 대시보드를 인쇄할 때 인쇄되는 정보 이해

대시보드를 인쇄하거나 .PDF 파일로 저장할 때 Adobe Workfront 웹 응용 프로그램에 표시되는 대시보드의 일부 정보가 인쇄되거나 내보낸 파일에 표시되지 않을 수 있습니다.

* [어떤 것이 표시됩니까?](#what-is-displayed)
* [표시되지 않는 것은 무엇입니까?](#what-is-not-displayed)

### 어떤 것이 표시됩니까? {#what-is-displayed}

인쇄되거나 내보낸 대시보드 파일에는 다음 정보가 포함됩니다.

* 대시보드 제목
* 보고서 제목
* 보고서가 마지막으로 생성된 시간의 타임스탬프
* 목록 보기, 외부 웹 페이지, 보고서 및 달력을 포함하여 대시보드의 모든 개체
* Workfront 관리자가 전역 탐색 막대에서 사용자 지정한 경우 회사의 로고입니다. Workfront 사이트 브랜딩에 대한 자세한 내용은 [Adobe Workfront 인스턴스 브랜딩](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### 표시되지 않는 것은 무엇입니까? {#what-is-not-displayed}

다음 정보는 인쇄되거나 내보낸 대시보드 파일에 포함되지 않습니다.

* Workfront 탐색 모음
* Workfront과 관련된 다른 모든 서식
* 보고서 크기와 개별 열의 수 및 너비에 따라 대시보드를 내보내고 인쇄하면 일부 열이 잘릴 수 있습니다.

## 대시보드 인쇄

1. 인쇄할 대시보드로 이동합니다.
1. 다음 중 하나를 수행합니다.

   * 클릭 **대시보드 작업** > **인쇄**

   * 누르기 **Ctrl+P** (Windows의 경우) 또는 **Command+P** (Mac에서)

      >[!IMPORTANT]
      >
      >* 대시보드가 사용자 지정 탭에 포함된 경우 이 두 선택 사항 중 어느 것도 사용할 수 없습니다. 사용자 지정 탭 만들기에 대한 내용은 [사용자 지정 탭 또는 섹션 만들기](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
      >* Internet Explorer 브라우저를 사용하는 경우에는 키보드 단축키 옵션을 사용할 수 없습니다.


1. 에서 **대상** 필드, 사용 가능한 다양한 인쇄 옵션 중에서 선택합니다.\
   인쇄 옵션은 사용하는 브라우저 및 브라우저 버전에 따라 다릅니다.

1. (선택 사항) 대시보드를 .PDF 파일로 저장한 다음 **저장** .PDF을 저장합니다.\
   대시보드를 .PDF 파일로 저장하는 방법에 대해 알아보려면 [대시보드 내보내기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. 클릭 **인쇄**.
