---
product-area: projects
navigation-topic: approvals
title: 작업 승인
description: 작업 승인
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 7366e3dd37b686a3566ca6d39e28eb6762c6d1ff
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---

# 작업 승인

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

승인자로 설정된 경우 승인 대기 중인 작업을 정기적으로 검토해야 합니다.

승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

Workfront에서 승인을 작업과 연결하는 방법에 대한 자세한 내용은 [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>승인과 연관된 객체에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>승인과 연관된 오브젝트에 대한 이상 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## Adobe Workfront에서 승인 찾기

Workfront의 다양한 영역에서 승인을 보고 관리할 수 있습니다.

승인 대기 중인 항목 또는 직접 승인을 위해 제출한 항목을 보는 방법에 대한 자세한 내용은 [승인 보기](../../review-and-approve-work/manage-approvals/view-approvals.md)를 참조하십시오.

## 홈 영역에서 작업 승인

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 승인** 위젯을 추가합니다.
1. (조건부) **필터** 드롭다운 메뉴를 클릭한 다음 **모두**&#x200B;를 선택하여 귀하에게 할당 및 위임된 승인을 확인합니다.

   >[!NOTE]
   >
   >작업 역할 또는 그룹에 할당된 승인이 홈에 표시되지 않습니다. 팀에 할당된 승인은 각 팀 구성원의 내 승인 위젯에 표시됩니다.


1. 승인 결정을 내릴 품목을 선택합니다.

   ![](assets/my-approvals-widget.png)

1. 오른쪽 패널에서 승인 결정을 내릴 때 사용할 수 있는 옵션 중 하나를 클릭합니다. 승인하는 항목의 유형에 따라 페이지의 오른쪽 상단에 다음 옵션이 표시됩니다.

   <table>
   <tr>
      <td>
      <p><strong>액세스</strong></p>
      </td>
      <td>
      <p><strong>작업 항목</strong></p>
      </td>
      <td>
      <p><strong>문서</strong></p>
      </td>
      <td>
      <p><strong>교정쇄</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>부여</li>
      <li>무시</li>
      </ul>
      원하는 경우 <b>액세스 변경</b> 드롭다운 메뉴에서 액세스 수준을 조정할 수 있습니다.
      </td>
      <td>
         <ul>
         <li>승인</li>
         <li>거부</li>
         </ul>
      결정 버튼의 드롭다운 메뉴를 클릭하여 결정과 함께 주석을 남길 수 있습니다.
      </td>
      <td>
   승인자로 할당됨
         <ul>
         <li>승인</li>
         <li>변경 사항과 함께 승인</li>
         <li>작업 필요</li>
         </ul>
   검토자로 할당됨
         <ul>
         <li>내 리뷰 완료</li>
         </ul>
      이 열의 옵션은 새 문서 승인에만 적용됩니다. 기존 문서 승인은 작업 항목 승인과 동일하게 표시됩니다. 
      </td>
      <td>
         <ul>
         <li>증명으로 이동</li>
         </ul>
         증명 뷰어에서 결정을 내립니다. 증명 검토에 대한 자세한 내용은 <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Adobe Workfront 내에서 증명 검토</a>를 참조하십시오.
      </td>
   </tr>
   </table>

결정을 내리면 내 승인 위젯에서 승인이 제거됩니다.


## 프로젝트, 작업 또는 문제에서 직접 작업 승인

프로젝트, 작업 또는 문제가 승인 보류 중일 때 프로젝트, 작업 또는 문제에서 직접 승인을 승인하거나 거부할 수 있습니다. 승인 프로세스에 대한 세부 사항을 볼 수도 있습니다.

프로젝트, 작업 또는 문제에서 직접 작업을 승인하려면 다음 작업을 수행하십시오.

1. 승인이 필요한 프로젝트, 작업 또는 문제로 이동합니다.

   프로젝트, 작업 또는 문제의 현재 승인 프로세스에 대한 승인 정보가 항목 헤더에 표시됩니다.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   다음 승인 정보를 사용할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">상태</td> 
      <td>프로젝트, 작업 또는 문제의 현재 상태. 현재 승인 보류 중인 항목의 상태입니다. 승인 프로세스의 각 단계가 승인되면 상태가 승인됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 단계</td> 
      <td>승인 프로세스의 단계입니다. <br>승인 보류 중인 현재 단계가 보류 중으로 표시됩니다. 이미 승인된 단계는 승인됨으로 표시되고, 아직 승인되지 않은 단계는 시작되지 않음으로 표시됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 승인 프로세스를 승인 또는 거부할지 여부에 따라 **승인** 또는 **거부**&#x200B;를 클릭합니다.\
   이제 승인 보류 중이던 승인 단계가 승인되고, 승인 진행이 다음 단계로 넘어간다. 모든 단계가 승인된 후 상태가 승인됩니다.

## 문서에서 직접 문서 승인

1. 승인이 필요한 문서가 포함된 문서 영역으로 이동합니다.
1. 문서를 선택한 다음 **승인**, **변경** 또는 **거부**&#x200B;를 클릭합니다.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (선택 사항) 문서에 대한 증명이 생성된 경우 [증명에서 문서 승인](#approve-a-document-from-a-proof)에 설명된 대로 증명 인터페이스 내에서 문서를 승인할 수 있습니다.

## 승인 알림 이메일에서 문서 승인

알림 설정에 따라 다른 사용자가 승인 결정을 내려야 하는 문서에 대해 알리는 이메일을 받을 수 있습니다. **승인 결정** 버튼이 포함된 전자 메일을 받으면 전자 메일에서 직접 승인 프로세스를 시작할 수 있습니다.

1. 이메일에서 **승인 결정**&#x200B;을 클릭하여 증명에 대한 문서 세부 정보 페이지를 엽니다.
1. 다음 중 하나를 수행하여 문서를 검토하십시오.

   * 문서에 대한 메타데이터를 봅니다.
   * 마크업과 댓글이 있는 문서를 검토할 수 있는 증명이 만들어졌다면 오른쪽 상단 모서리에서 **증명 열기** ![](assets/open-proof-icon-qs.png)를 클릭하고 증명을 검토하십시오.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     증명 검토에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 검토](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)를 참조하십시오.

1. 문서를 승인하거나, 변경 내용으로 승인하거나, 거부하려면 오른쪽 상단의 **결정** 옵션을 클릭하십시오.

## 증명에서 문서 승인 {#approve-a-document-from-a-proof}

증명 뷰어 내에서 문서를 승인할 수 있습니다. 자세한 내용은 문서 [증명 뷰어에서 증명 결정](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)의 [증명 뷰어에서 증명 결정](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)을 참조하십시오.
