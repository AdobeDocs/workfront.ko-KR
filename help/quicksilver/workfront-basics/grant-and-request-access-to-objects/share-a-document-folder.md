---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 문서 폴더 공유
description: 문서 영역에서 폴더와 해당 컨텐츠를 공유할 수 있습니다.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 842c61cf6dfee0c79b1c95ff84888083c9f5b5a4
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 문서 폴더 공유

문서 영역에서 폴더와 해당 컨텐츠를 공유할 수 있습니다.

>[!NOTE]
>
>* 폴더는 객체의 폴더 계층 구조 상위 5개 수준에 있어야 합니다. 여섯 번째 수준 또는 그 이하의 각 폴더는 바로 위의 폴더에서 공유 구성을 상속합니다.
>
>  하위 폴더를 추가하여 폴더 계층 구조를 만드는 방법에 대한 자세한 내용은 문서 [문서 폴더 만들기](../../documents/organizing-documents/create-documents-folder.md)에서 [폴더 및 하위 폴더 만들기](../../documents/organizing-documents/create-documents-folder.md#creating-folders) 섹션을 참조하십시오.
>
>* 스마트 폴더를 공유할 수 없습니다.
>* 템플릿 내의 문서 폴더에 대한 공유 옵션을 구성한 다음 누군가가 해당 템플릿에서 프로젝트를 만드는 경우 공유 구성이 새 프로젝트의 문서 폴더로 전송되지 않습니다.
>* 작업 항목 내의 문서 폴더에 대한 공유 옵션을 구성한 다음 작업 항목을 복사하면 공유 구성이 새 작업 항목의 문서 폴더로 전송되지 않습니다.
>

## 액세스 요구 사항

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td> <p>문서에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>오브젝트에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 폴더 공유

1. Adobe Workfront의 오른쪽 상단에 있는 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **문서**&#x200B;를 클릭합니다.

   또는

   Workfront 개체를 연 상태에서 왼쪽 패널에서 **문서**&#x200B;를 클릭합니다.

1. 폴더를 선택한 다음 도구 모음에서 공유 아이콘 ![](assets/share-icon.png)을(를) 클릭합니다.

   폴더는 개체에 있는 폴더 계층의 상위 5개 수준에 있어야 하며 스마트 폴더일 수 없습니다.

1. 표시되는 상자에서 **폴더 액세스 권한 부여**&#x200B;에 폴더를 공유할 사용자, 팀, 작업 역할, 그룹 또는 회사의 이름을 입력한 다음 이름이 표시되면 **Enter**&#x200B;를 누릅니다.
1. 방금 추가한 사용자, 팀, 작업 역할, 그룹 또는 회사에 대한 액세스를 조정하려면 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 사용 가능한 다음 옵션 중 하나와 고급 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보기</td> 
      <td> <p>폴더 및 해당 컨텐츠를 볼 수 있습니다.</p> <p>다음을 허용할지 여부를 지정하려면 <strong>고급 설정</strong>을 클릭하십시오.</p> 
       <ul> 
        <li><strong>다운로드</strong>: 폴더 및 해당 컨텐츠를 ZIP 파일로 다운로드하는 기능</li> 
        <li> <p><strong>공유</strong>: 시스템의 다른 사용자와 폴더를 공유하는 기능</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리함</td> 
      <td> <p>폴더 및 해당 컨텐츠를 보고 편집하는 기능</p> <p><strong>고급 설정</strong>을 클릭하여 사용자가 다음 작업을 수행하도록 허용할지 여부를 지정합니다.</p> 
       <ul> 
        <li><strong>삭제</strong>: 시스템에서 폴더 및 해당 컨텐츠를 삭제합니다.</li> 
        <li><b>다운로드</b>: 폴더 및 해당 콘텐츠를 ZIP 파일로 다운로드합니다.</li> 
        <li><strong>공유</strong>: 폴더 및 해당 컨텐츠를 시스템의 다른 사용자와 공유</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 3-4단계를 반복하여 목록에 다른 이름을 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) 시스템의 모든 사용자가 폴더 및 해당 컨텐츠를 볼 수 있도록 하려면 공유 상자의 오른쪽 위 모서리에 있는 톱니바퀴 아이콘 ![](assets/gear-icon-settings-with-dn-arrow.jpg)을(를) 클릭한 다음 **이 항목을 시스템 전체에 표시합니다.**

   마음이 바뀌면 **시스템 전체 액세스 제거**(기본 옵션)를 클릭할 수 있습니다.

## 사용자가 공유된 폴더의 콘텐츠에 액세스하는 방법

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

현재 폴더를 공유할 때 수신자의 문서 영역에 폴더가 표시되지 않습니다. 그러나 문서 보고서를 실행하여 해당 문서에 액세스할 수 있습니다.

보고서 실행에 대한 자세한 내용은 문서 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)의 [개체에 대한 보고서](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 섹션을 참조하십시오. [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)도 참조하세요.

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## 폴더가 포함된 오브젝트를 공유할 때 상속된 권한

문서 폴더가 있는 객체를 공유하면 수신자도 폴더에 액세스할 수 있습니다.

* 수신자에게 상위 객체에 대한 보기 액세스 권한을 부여하는 경우, 상위 객체는 폴더에 대한 보기 액세스 권한을 갖게 됩니다.
* 받는 사람에게 상위 객체에 대한 기여 또는 관리 액세스 권한을 부여하는 경우 해당 사용자는 폴더에 대한 관리 액세스 권한을 갖게 됩니다.
* 상위 객체에 한 가지 액세스 유형(보기, 기여 또는 관리)을 부여하고 폴더에 다른 유형을 부여하는 경우 수신자는 폴더 내의 문서에 대한 두 가지 액세스 유형 중 가장 높은 액세스 유형을 갖게 됩니다

  예를 들어 상위 객체를 보기 권한으로 공유하고 폴더를 관리 권한으로 공유하는 경우 수신자는 폴더에 있는 문서에 대해 관리 권한을 갖게 됩니다.

  >[!NOTE]
  >
  >첨부된 문서는 첨부된 객체에서만 권한을 상속합니다. 개체에서 폴더를 만들고 문서를 폴더로 이동하면 해당 폴더의 권한이 상속됩니다. 그러나 상위 또는 최상위 개체에 폴더를 만들어 해당 폴더로 문서를 이동하면 해당 폴더의 권한이 상속되지 않습니다.

* 수신자의 액세스 수준에 &quot;프로젝트, 작업, 문제 등에서 문서 액세스 권한을 상속하지 않음&quot; 옵션이 활성화되어 있으면 공유 폴더의 문서에 대한 권한이 상속되지 않습니다. 폴더에 있는 문서에 대한 액세스 권한을 부여하려면 문서를 공유해야 합니다.

  &quot;상속 안 함&quot; 옵션에 대한 자세한 내용은 [Adobe Workfront 액세스 구성](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)을 참조하십시오.

  문서 공유에 대한 자세한 내용은 [문서 공유](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)를 참조하십시오.
