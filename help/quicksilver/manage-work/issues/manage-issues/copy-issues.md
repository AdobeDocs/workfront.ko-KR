---
product-area: projects
navigation-topic: manage-issues
title: 문제 복사
description: 문제 또는 요청을 복사하고 동일하거나 다른 프로젝트에 저장할 수 있습니다. 작업에서 다른 프로젝트로 문제를 복사할 수도 있습니다.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# 문제 복사

문제 또는 요청을 복사하고 동일하거나 다른 프로젝트에 저장할 수 있습니다. 작업에서 다른 프로젝트로 문제를 복사할 수도 있습니다.

다음 개체에서 문제를 복사할 수 있습니다.

* 프로젝트에서 동일한 프로젝트로(동일한 프로젝트에 복제됨)
* 작업에서 동일한 작업에 이르기까지(동일한 작업에 있을 경우 복제)
* 프로젝트에서 다른 프로젝트로
* 작업에서 프로젝트로

>[!TIP]
>
>&quot;문제&quot; 및 &quot;요청&quot;은 Workfront에서 서로 교환하여 사용됩니다. 프로젝트 및 작업 모두에 문제를 기록하여 해결해야 하는 예상치 못한 작업을 나타낼 수 있습니다. 요청 큐로 지정된 프로젝트에서 문제로 기록된 요청을 제출할 수도 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> <p>프로젝트의 Issues 섹션에서 문제를 복사하려면 더 높은 라이선스를 검토하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 액세스 수준의 문제에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>문제 추가 기능을 사용하여 문제를 복사하려는 항목에 대한 권한을 제공합니다.</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문서 또는 요청 큐 관련 문제에 대한 고려 사항

문서 또는 요청 큐와 연관된 문제를 복사할 때에는 다음 사항을 고려하십시오.

* **문제가 요청 큐와 연결된 경우:** 문제를 다른 개체에 복사하고 문제가 요청 큐와 연결되어 있으면 복사한 문제가 첫 번째 문제의 원본 큐와 더 이상 연결되지 않습니다.
* **문서가 문제에 첨부된 경우:** 문제를 다른 객체에 복사하고 문제에 문서에 첨부된 문서가 있으면 문서와 해당 버전도 새 문제로 이동합니다. 문서와 연결된 증명 또는 승인은 이동하지 않습니다.
* **문제가 문서 또는 폴더에 연결되어 있는 경우:** Google Drive와 같은 타사 서비스에 연결된 문서 또는 폴더가 있는 문제를 복사하면 해당 문서에 연결된 링크가 복사된 문제로 전송됩니다. 

## 목록의 문제 복사

문제 목록 또는 문제 보고서에서 하나 또는 여러 문제를 복사할 수 있습니다.

1. 복사하려는 문제 또는 문제가 포함된 프로젝트로 이동합니다.

   또는

   문제 보고서로 이동합니다.

1. 프로젝트로 이동하려면 **문제** 왼쪽 패널에 표시됩니다.
1. 복사할 문제 또는 문제를 선택하고 **추가 메뉴** 문제 목록의 맨 위에서 을 클릭합니다. **복사 대상**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. 섹션에 설명된 대로 문제를 계속 복사합니다 [단일 문제 복사](#copy-a-single-issue) 2단계 시작.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:&nbsp;ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## 단일 문제 복사 {#copy-a-single-issue}

문제를 볼 때 한 문제를 복사할 수 있습니다.

1. 복사할 문제로 이동한 다음 **자세히** 메뉴 ![](assets/more-icon.png) 문제 이름의 오른쪽에 있는 다음 **복사** 대상.

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   다음 **문제 복사** 상자가 표시됩니다.

   ![](assets/copy-issue-box-nwe-350x285.png)

1. 에서 **대상 프로젝트 선택** 섹션에서 문제를 복사할 프로젝트의 이름을 지정합니다. 기본적으로 현재 프로젝트의 이름이 표시됩니다.

   >[!TIP]
   >
   >목록에 100개의 프로젝트만 표시됩니다.

1. (조건부) 클릭 **요청 액세스** 프로젝트에 문제를 복사할 수 있는 액세스 권한이 없는 경우.
1. (조건부) 대상 프로젝트의 작업 중 하나에 문제를 추가할 수 있는 액세스 권한이 있는 경우 액세스를 요청하지 않고 선택한 대상 프로젝트에 문제를 계속 복사합니다.

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Workfront 관리자가 이러한 프로젝트에 문제를 추가할 수 없을 때 선택한 프로젝트가 승인 보류 중, 완료 또는 사용 중지 상태인 경우 유사한 메시지가 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (선택 사항)에서 **옵션** 섹션에서 아래 표에 나열된 항목을 선택 취소하여 새 작업에서 제거합니다. 기본적으로 모든 옵션이 선택됩니다.

   >[!NOTE]
   이는 원래 문제가 아닌 복사된 문제에만 영향을 줍니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당</td> 
      <td>문제에 할당된 사용자, 작업 역할 또는 팀을 제거합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">진행</td> 
      <td>문제의 완료율이 있는 경우 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서</td> 
      <td><span style="line-height: 1.5;">문서 버전, 링크된 문서 및 폴더를 포함하여 문서 탭의 모든 항목을 제거합니다.</span> <br>기본적으로 문서 증명 및 승인을 다른 문제에 복사할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">권한</td> 
      <td>문제가 공유되는 엔터티를 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">업데이트</td> 
      <td>문제의 업데이트 섹션에서 주석을 제거합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 데이터</td> 
      <td>문제에 대한 사용자 지정 양식에서 정보를 제거하고 문제와 함께 복사된 경우 문제에 첨부된 문서와 연결된 사용자 지정 양식에 대한 정보를 제거합니다. 사용자 지정 양식은 문제 및 문서에 첨부되지만 양식의 정보는 새 문제로 이어지지 않습니다. </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항)에서 **작업 선택** 섹션에서 문제를 이동할 작업을 선택합니다.
1. 클릭 **복사 문제** 또는 **복사 문제** 목록에서 여러 문제를 선택한 경우.

   복사된 문제가 지정된 프로젝트에 추가됩니다.

 
