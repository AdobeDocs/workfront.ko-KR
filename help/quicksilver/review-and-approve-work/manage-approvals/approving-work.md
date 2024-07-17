---
product-area: projects
navigation-topic: approvals
title: 작업 승인
description: 작업 승인
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# 작업 승인

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

승인자로 설정된 경우 승인 대기 중인 작업을 정기적으로 검토해야 합니다.

승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

Workfront에서 승인을 작업과 연결하는 방법에 대한 자세한 내용은 [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 액세스 요구 사항

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

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## Adobe Workfront에서 승인 찾기

Workfront의 다양한 영역에서 승인을 보고 관리할 수 있습니다.

승인 대기 중인 항목 또는 직접 승인을 위해 제출한 항목을 보는 방법에 대한 자세한 내용은 [승인 보기](../../review-and-approve-work/manage-approvals/view-approvals.md)를 참조하십시오.

## 홈 영역에서 작업 승인

1. Adobe Workfront의 왼쪽 위 모서리에 있는 **Home** 아이콘 ![](assets/home-icon-30x29.png)을(를) 클릭합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 사용자 환경의 홈 아이콘을 다음과 같이 변경할 수 있습니다.
   >
   >   
   >* 조직 설명을 위해 사용자 지정된 이미지로 대체합니다. 이 경우 아이콘은 이 문서에 표시된 것과 다르게 표시됩니다.
   >* 연결된 페이지를 다른 페이지로 바꿉니다. 이 경우 페이지의 오른쪽 상단에 있는 **기본 메뉴** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **홈**&#x200B;을(를) 클릭합니다.

1. **필터** 드롭다운 메뉴를 클릭합니다.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. **승인**&#x200B;을 선택합니다.\
   승인이 필요한 모든 작업 항목이 표시됩니다. 

   >[!NOTE]
   >
   >작업 역할 또는 그룹에 할당된 승인이 홈에 표시되지 않습니다. 팀에 할당된 승인은 작업 목록의 팀 요청 그룹에 표시됩니다.

1. (선택 사항) 문서 [홈 영역의 작업 목록에 항목 표시](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)의 &quot;날짜, 프로젝트 또는 우선 순위별로 그룹화 및 정렬&quot; 섹션에 설명된 대로 승인이 표시되는 순서를 변경합니다.
1. 승인 결정을 내릴 품목을 선택합니다.

   ![](assets/task-approval-home-350x127.png)

1. 오른쪽 패널에서 승인 결정을 내릴 때 사용할 수 있는 옵션 중 하나를 클릭합니다. 승인하는 항목의 유형에 따라 페이지의 오른쪽 상단에 다음 옵션이 표시됩니다.

   * **프로젝트:** **승인** 또는 **거부**&#x200B;를 클릭합니다.

   * **작업:** **승인** 또는 **거부** 을 클릭합니다.

   * **문제:** **승인** 또는 **거부** 을 클릭합니다.

   * **타임시트:** **승인** 또는 **거부** 을 클릭합니다.

   * **문서:** **승인**, **거부** 또는 **변경**&#x200B;을 클릭합니다.\
      볼 때 다음 사항을 고려하십시오  승인:

      * 사용자가 [Adobe Workfront 내에서 증명 공유](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) 문서의 &quot;증명 링크 공유&quot; 섹션에 설명된 대로 증명을 공유할 때 증명 승인이 여기에 표시됩니다.
      * 증명 승인은 Workfront 환경이 Workfront Proof Premium 계정과 통합된 경우에만 홈 영역에 표시됩니다. 여기에 설명된 대로 증명을 사용할 수 없는 경우 Workfront 관리자에게 문의하십시오.
      * 증명 승인을 알리는 인앱 알림을 받게 됩니다.\
        인앱 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)를 참조하십시오.

      * 승인을 요청한 사용자의 이름은 홈 영역의 썸네일 이미지 옆에 표시되며 다음과 같은 텍스트가 표시됩니다.\
        &quot;*사용자 A*&#x200B;이(가) 다음에 대한 승인을 원합니다.&quot;

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        사용자 이름을 사용할 수 없는 경우 다음 텍스트가 표시됩니다.\
        &quot;증명의 새 버전을 볼 준비가 되었습니다.&quot;
      * 증명에 대한 승인 결정을 내리려면 **증명으로 이동**&#x200B;을 클릭하고 **검토 완료**&#x200B;를 클릭한 다음 사용 가능한 옵션 중 하나를 클릭하십시오. 증명을 승인할 때 사용할 수 있는 옵션은 **승인됨**, **변경 사항과 함께 승인됨**, **변경 필요** 및 **관련 없음**&#x200B;입니다.

      * 증명에 대한 결정이 내려지면 **새로 고침** 단추를 클릭하거나 브라우저 페이지를 새로 고칠 때까지 증명이 &quot;결정됨&quot; 텍스트와 함께 내 승인 탭에 유지됩니다.

        증명 검토에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 검토](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)를 참조하십시오.

   * **액세스:** **액세스 권한 변경** 드롭다운 메뉴에서 부여할 액세스 수준을 선택한 다음 **액세스 권한 부여**&#x200B;를 클릭합니다. 또는 **무시**&#x200B;를 클릭합니다.

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
