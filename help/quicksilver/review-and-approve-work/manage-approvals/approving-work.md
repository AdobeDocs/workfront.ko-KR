---
product-area: projects
navigation-topic: approvals
title: 작업 승인
description: 작업 승인
author: Courtney
feature: Work Management
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# 작업 승인

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

승인자로 설정된 경우 승인을 기다리는 작업을 정기적으로 검토해야 합니다.

승인 프로세스 생성에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Workfront에서 승인과 작업 연결에 대한 자세한 내용은 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

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
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>승인과 연관된 객체에 대한 보기 이상의 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>승인과 연관된 객체에 대한 권한 보기 또는 그 이상의 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## Adobe Workfront에서 승인 찾기

Workfront의 다양한 영역에서 승인을 보고 관리할 수 있습니다.

승인을 기다리는 항목 또는 승인을 위해 직접 제출한 항목을 보는 방법에 대한 자세한 내용은 [승인 보기](../../review-and-approve-work/manage-approvals/view-approvals.md).

## 홈 영역에서 작업 승인

1. 을(를) 클릭합니다. **홈** 아이콘 ![](assets/home-icon-30x29.png) Adobe Workfront의 왼쪽 위 모서리에서

   >[!NOTE]
   >
   >Workfront 관리자는 사용자 환경에서 홈 아이콘을 다음과 같이 변경할 수 있습니다.
   >
   >   
   >* 조직을 보여주기 위해 사용자 지정된 이미지로 바꿉니다. 이 경우 이 문서에 표시된 아이콘의 모양이 다릅니다.
   >* 연결된 페이지를 다른 페이지로 바꿉니다. 이 경우 **기본 메뉴** ![](assets/main-menu-icon.png) 페이지의 오른쪽 위 모서리에서 을(를) 클릭하고 **홈**.


1. 을(를) 클릭합니다. **필터** 드롭다운 메뉴

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 선택 **승인**.\
   승인이 필요한 모든 작업 항목이 표시됩니다. 

   >[!NOTE]
   >
   >작업 역할 또는 그룹에 할당된 승인이 홈에 표시되지 않습니다. 팀에 할당된 승인은 작업 목록의 팀 요청 그룹에 표시됩니다.

1. (선택 사항) 문서의 &quot;날짜, 프로젝트 또는 우선 순위&quot; 섹션에 설명된 대로 승인이 표시되는 순서를 변경합니다 [홈 영역의 작업 목록에 항목을 표시합니다.](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. 승인 결정을 내릴 품목을 선택합니다.

   ![](assets/task-approval-home-350x127.png)

1. 오른쪽 패널에서 승인 결정을 할 때 사용할 수 있는 옵션 중 하나를 클릭합니다. 승인하려는 항목 유형에 따라 페이지의 오른쪽 위 모서리에 다음 옵션이 표시됩니다.

   * **프로젝트:** 클릭 **승인** 또는 **거부**.

   * **작업:** 클릭 **승인** 또는 **거부** .

   * **문제:** 클릭 **승인** 또는 **거부** .

   * **작업표:** 클릭 **승인** 또는 **거부** .

   * **문서:** 클릭 **승인**, **거부**, 또는 **변경 사항**.\
       승인을 볼 때 다음 사항을 고려하십시오.

      * 문서에서 &quot;증명 링크 공유&quot; 섹션에 설명된 대로 사용자가 증명을 공유할 때 증명 승인이 여기에 표시됩니다 [Adobe Workfront에서 증명 공유](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Workfront 환경이 Workfront Proof Premium 계정과 통합된 경우에만 홈 영역에 언어 교정 승인이 표시됩니다. 여기에 설명된 대로 언어 보호를 사용할 수 없는 경우 Workfront 관리자에게 문의하십시오.
      * 앱 내 알림을 수신하여 언어 교정 승인을 알려줍니다.\
         인앱 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * 승인을 요청한 사용자의 이름이 홈 영역의 축소판 이미지 옆에 다음 텍스트로 표시됩니다.\
         &quot;*사용자 A* ...에 대한 당신의 승인을..&quot;

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

         사용자 이름을 사용할 수 없으면 다음 텍스트가 표시됩니다.\
         &quot;새로운 버전의 증명을 볼 준비가 되었습니다.&quot;
      * 증명에 대한 승인 결정을 내리려면 **증명으로 이동**&#x200B;를 클릭합니다. **검토 완료**&#x200B;을 클릭한 다음 사용 가능한 옵션 중 하나를 클릭합니다. 증명을 승인할 때 사용할 수 있는 옵션은 다음과 같습니다. **승인됨**, **변경 사항이 있는 승인됨**, **필요한 변경 사항**, 및 **관련 없음**.

      * 증명에 대한 결정이 수행된 후 를 클릭할 때까지 &quot;의사 결정&quot;이라는 텍스트가 있는 My Approvals 탭에 증명이 유지됩니다. **새로 고침** 단추를 클릭하거나 브라우저 페이지를 새로 고칠 때까지 선택합니다.

         증명 검토에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 검토](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
   * **액세스:** 에서 부여할 액세스 권한 수준을 선택합니다 **액세스 변경** 드롭다운 메뉴를 클릭한 다음 **액세스 권한 부여**. 또는 **무시**.


## 프로젝트, 작업 또는 문제와 직접 작업 승인

프로젝트, 작업 또는 문제가 승인 보류 중인 경우 프로젝트, 작업 또는 문제 등에서 직접 승인을 승인하거나 거부할 수 있습니다. 승인 프로세스에 대한 세부 사항을 볼 수도 있습니다.

프로젝트, 작업 또는 문제와 직접 작업을 승인하려면

1. 승인이 필요한 프로젝트, 작업 또는 문제로 이동합니다.

   프로젝트, 태스크 또는 문제의 현재 승인 프로세스에 대한 승인 정보가 품목 헤더에 표시됩니다.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   다음 승인 정보를 사용할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">상태</td> 
      <td>프로젝트, 작업 또는 문제의 현재 상태입니다. 승인 보류 중인 항목의 현재 상태입니다. 승인 프로세스의 각 단계가 승인되면 상태가 승인됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 단계</td> 
      <td>승인 프로세스의 단계입니다. <br>승인 보류 중인 현재 단계가 보류 중으로 표시됩니다. 이미 승인된 단계는 승인됨으로 표시됩니다. 아직 승인되지 않은 단계는 시작되지 않음으로 표시됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **승인** 또는 **거부**&#x200B;승인 프로세스를 승인할지 또는 거부할지를 결정합니다.\
   승인이 보류 중인 승인 단계가 승인되고 승인 프로세스가 다음 단계로 이동합니다. 모든 단계가 승인되면 상태가 승인됩니다.

## 문서에서 직접 문서 승인 

1. 승인이 필요한 문서가 포함된 문서 영역으로 이동합니다.
1. 문서를 선택한 다음 **승인**, **변경 사항**, 또는 **거부**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (선택 사항) 문서에 대한 증명을 생성한 경우 다음 설명에 따라 교정 인터페이스 내에서 문서를 승인할 수 있습니다. [증명으로 문서 승인](#approve-a-document-from-a-proof).

## 승인 알림 이메일에서 문서 승인

알림 설정에 따라 다른 사용자가 승인 결정을 내려야 하는 문서에 대해 알리는 이메일을 받을 수 있습니다. 가 포함된 이메일을 받는 경우 **승인 결정** 버튼을 사용하면 이메일에서 직접 승인 프로세스를 시작할 수 있습니다.

1. 이메일에서 **승인 결정** 증명을 위한 문서 세부 사항 페이지를 열려면 다음을 수행하십시오.
1. 문서를 검토하려면 다음 중 하나를 수행합니다.

   * 문서에 대한 메타데이터를 봅니다.
   * 마크업 및 주석이 있는 문서를 검토하기 위한 증명을 만든 경우 **공개 증명** ![](assets/open-proof-icon-qs.png) 오른쪽 상단 모서리에서 증명을 검토합니다.

      <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

      증명 검토에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 검토](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. 클릭 **결정** 오른쪽 위 모서리의 옵션을 사용하여 문서를 승인, 변경 내용 승인 또는 거부할 수 있습니다.

## 증명으로 문서 승인 {#approve-a-document-from-a-proof}

교정 뷰어 내에서 문서를 승인할 수 있습니다. 자세한 내용은 [교정 뷰어의 증명 결정](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) 기사 [교정 뷰어의 증명 결정](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
