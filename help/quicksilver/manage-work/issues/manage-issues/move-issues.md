---
product-area: projects
navigation-topic: manage-issues
title: 문제 이동
description: 프로젝트와 작업 간에 문제를 이동할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# 문제 이동

다음 개체 간에 문제를 이동할 수 있습니다.

* 프로젝트에서 다른 프로젝트로
* 작업에서 동일한 프로젝트 또는 다른 프로젝트의 다른 작업에 이르기까지
* 작업에서 프로젝트 또는 다른 프로젝트로
* 프로젝트에서 동일한 프로젝트의 작업이나 다른 프로젝트의 작업에 이르기까지

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
   <td> <p>요청 이상</p> <p>프로젝트의 Issues 섹션에서 문제를 이동하려면 더 높은 라이선스를 검토하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 액세스 수준의 문제에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>문제를 추가할 수 있는 기능을 사용하여 문제를 이동하는 항목에 권한을 부여합니다.</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 이동 문제에 대한 고려 사항

문서가 포함되거나 요청 큐와 연관된 문제를 이동할 때는 다음 사항을 고려하십시오.

* **문제가 요청 큐와 연결된 경우:** 문제를 다른 개체로 이동하고 문제가 요청 큐와 연결되어 있으면 이동된 문제가 첫 번째 문제가 발생한 원래 큐와 더 이상 연결되지 않습니다.
* **문서가 문제에 첨부된 경우:** 문제를 다른 개체로 이동하고 문제에 첨부된 문서가 있으면 문서, 버전 및 증명도 새 문제로 이동합니다. 문서와 연관된 모든 승인이 이동되지 않습니다.
* **문제가 문서 또는 폴더에 연결되어 있는 경우:** Google Drive와 같은 타사 서비스에 연결된 문서나 폴더가 있는 문제를 이동하면 해당 문서에 대한 링크가 문제와 함께 이동합니다.

## 목록에서 문제 이동

문제 목록 또는 문제 보고서에서 하나 또는 여러 문제를 이동할 수 있습니다.

1. 이동할 문제 또는 문제가 포함된 프로젝트로 이동합니다.

   또는

   문제 보고서로 이동합니다.

1. 프로젝트로 이동하려면 **문제** 왼쪽 패널에 표시됩니다.
1. 이동할 문제 또는 문제를 선택하고 **추가 메뉴** 문제 목록의 맨 위에서 을 클릭합니다. **이동 위치**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. 섹션에 설명된 대로 문제를 계속 이동합니다 [단일 문제 이동](#move-a-single-issue) 2단계 시작.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## 단일 문제 이동 {#move-a-single-issue}

한 문제를 볼 때 이동할 수 있습니다.

### 미리 보기 환경에서 단일 문제 이동

1. 복사할 문제로 이동하여 **자세히** 메뉴 ![](assets/more-icon.png)문제 이름의 오른쪽에 있는 를 선택한 다음 **이동** 대상.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   다음 **문제 이동** 상자가 표시됩니다.

   ![](assets/move-issue-box-nwe-350x280.png)

1. 에서 **대상 프로젝트 선택** 섹션에서 문제를 이동할 프로젝트의 이름을 지정합니다. 기본적으로 현재 프로젝트의 이름이 표시됩니다.

   >[!TIP]
   >
   >목록에 100개의 프로젝트만 표시됩니다.

1. (조건부) 클릭 **요청 액세스** 문제를 프로젝트로 이동할 수 있는 액세스 권한이 없는 경우
1. (조건부) 대상 프로젝트의 작업 중 하나에 문제를 추가할 수 있는 액세스 권한이 있는 경우 액세스를 요청하지 않고 선택한 대상 프로젝트에서 문제를 계속 이동합니다.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Workfront 관리자가 이러한 프로젝트에 문제를 추가할 수 없을 때 선택한 프로젝트가 승인 보류 중, 완료 또는 사용 중지 상태인 경우 유사한 메시지가 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (선택 사항)에서 **옵션** 섹션에서 아래 표에 나열된 항목을 선택 취소하여 이동한 문제와 제거합니다. 기본적으로 모든 옵션이 선택됩니다.

   >[!IMPORTANT]
   >
   >옵션 목록에서 항목을 선택 해제하면 데이터가 손실됩니다. 기존 문제의 정보는 제거되며 복구할 수 없습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두 선택</td> 
      <td>새 위치로 이동할 때 문제의 모든 정보를 제거하려면 이 옵션을 선택 취소합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">할당</td> 
      <td>문제에 할당된 사용자, 작업 역할 또는 팀을 제거합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">진행</td> 
      <td>문제의 완료율이 있는 경우 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>문서</p></td> 
      <td> <p>문서 버전, 링크된 문서 및 폴더를 포함하여 문서 탭의 모든 항목을 제거합니다.

   <b>메모</b>

   이 문제와 함께 문서를 이동하지 않도록 선택하면 문서가 삭제되어 30일 동안 휴지통에 보관됩니다. 관리자가 복원할 수 있으며 이동한 문제에 대해 복원됩니다.

   문제가 이동되면 복원된 문서가 복원되는 관리자의 사용자 페이지의 문서 영역에 배치됩니다.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">권한</td> 
      <td>문제가 공유되는 엔터티를 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">업데이트</td> 
      <td>문제의 업데이트 섹션에서 주석을 제거합니다.</td> 
     </tr> 
    </tbody> 
   </table>


1. (선택 사항)에서 **작업 선택** 섹션에서 문제를 이동할 작업을 선택합니다.
1. 클릭 **문제 이동** 또는 **이동 문제**: 목록에서 여러 문제를 선택한 경우.

   이동된 문제가 지정된 프로젝트에 추가됩니다.




