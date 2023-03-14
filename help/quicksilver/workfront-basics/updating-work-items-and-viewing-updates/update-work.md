---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 작업 업데이트
description: Adobe Workfront 개체(프로젝트, 작업 또는 문제)에 업데이트를 추가하여 개체의 진행 상황을 전달할 수 있습니다. 개체를 할당받거나 구독 중인 사용자는 업데이트를 볼 수 있습니다. 사용자에 태그를 지정하여 업데이트에 주의를 기울일 수도 있습니다.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: d7ae3d47cbc4426630260ab5e726380e4775096a
workflow-type: tm+mt
source-wordcount: '1774'
ht-degree: 1%

---

# 작업 업데이트

<!-- Drafted for commenting experience: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for a limited number of objects.</span> -->

Adobe Workfront 개체(프로젝트, 작업 또는 문제)에 업데이트를 추가하여 개체의 진행 상황을 전달할 수 있습니다. 개체를 할당받거나 구독 중인 사용자는 업데이트를 볼 수 있습니다. 사용자에 태그를 지정하여 업데이트에 주의를 기울일 수도 있습니다.

Workfront의 다음 영역에서 오브젝트에 업데이트를 추가할 수 있습니다.

* Workfront 개체의 업데이트 섹션에서
* 홈 영역에서(작업 및 문제의 경우)
* 오브젝트 목록의 요약 패널에서 시작(작업 및 문제용)
* 타임시트에서(작업 및 문제의 경우)

## 액세스 요구 사항

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>문제 및 문서에 대해 요청 이상, 기타 모든 오브젝트에 대해 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>업데이트가 있는 오브젝트에 대한 보기 또는 편집 액세스 권한</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>오브젝트에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 항목에 업데이트 추가

<!--drafted for the commenting experience - change the NOTE at the top of this paragraph with every new release to other objects

Adding an update to a work item differs depending on what environment and what object you choose. 

### Add an update to a work item in the Production environment

>[!NOTE]
>
>The following functionality is available for all objects except for goals, in the Production and Preview environements. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. 업데이트를 제공할 작업 항목(예: 프로젝트, 작업 또는 문제)으로 이동합니다.
1. 다음을 클릭합니다. **업데이트** 섹션.
1. 클릭 **새 업데이트 시작,** 그런 다음 업데이트를 입력합니다.

1. (선택 사항) 업데이트에 서식 있는 텍스트 서식을 추가하려면 **리치 텍스트** 입력할 때 도구 모음

   | **속성** | **도구 모음 단추** | **Mac 바로 가기 키** | **PC 바로 가기 키** |
   |---|---|---|---|
   | 볼드체 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 기울임체 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 밑줄 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | 하이퍼링크 | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl+K |
   | 글머리 기호 목록 | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 번호 매기기 목록 | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | 견적 차단 | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   텍스트 서식을 중지하려면 **리치 텍스트** 도구 모음

   >[!NOTE]
   >
   >* 서식은 사용자가 업데이트를 포함하여 받는 모든 이메일 알림에도 표시됩니다.
   >* 전자 메일의 업데이트에 적용된 서식 있는 텍스트 서식을 업데이트 탭에서 보면 업데이트에 표시되지 않습니다.
   >* 조직에서 Internet Explorer와 함께 Workfront을 사용하는 경우 업데이트에 붙여넣은 서식 있는 텍스트 서식이 손실되고 일반 텍스트로 표시됩니다. 리치 텍스트 도구 모음의 속성을 사용하여 텍스트 서식을 다시 지정할 수 있습니다.
   >* 타임시트 영역에서 수행한 업데이트 또는 보고서에서 본 메모 및 마지막 조건 개체에 대해 서식 있는 텍스트 서식을 사용할 수 없습니다.


1. (선택 사항) 이전 업데이트 또는 다른 소스의 텍스트를 포함하여 자신의 업데이트와 구분하려면 해당 텍스트를 블록 인용으로 표시할 수 있습니다. 다음을 클릭합니다. **견적 차단** 아이콘 ![](assets/block-quote-small.png) 인용 텍스트를 입력합니다. 인용된 텍스트가 세로 회색 선으로 표시됩니다. 다음을 클릭합니다. **견적 차단** 아이콘을 다시 클릭하여 일반적인 서식으로 돌아갑니다.

   ![](assets/block-quote-marked-350x144.png)

1. (선택 사항) 업데이트에 이모지를 추가합니다.

   >[!NOTE]
   >
   >* Workfront은 :)와 같은 구두점 이모티콘을 이모티콘으로 대체하지 않습니다.
   >* 타임시트 영역에서 수행한 업데이트 또는 보고서에서 본 메모 및 마지막 조건 개체에 대해 이모지를 사용할 수 없습니다.
   >* Workfront의 이모지 기능은 유니코드 문자를 사용하며, 따라서 유니코드 코드 포인트를 지원하는 브라우저와 운영 체제에만 표시됩니다. 사용자의 버전과 다른 플랫폼, 브라우저 또는 운영 체제 버전의 사용자는 동일한 이모지에 액세스할 수 없습니다.
   >* 지원되지 않는 이모지는 검은색 또는 흰색 상자로 표시됩니다.
   >* Windows 7에서는 흑백 이모티콘만 지원합니다.
   >* 이메일을 통해 수행한 업데이트에 적용되는 이모지는 업데이트 영역에서 볼 때 업데이트에 표시되지 않습니다.


1. (선택 사항) 추가 정보 소스에 URL 링크를 추가하려면 다음을 수행합니다.

   1. 링크를 삽입할 업데이트를 클릭합니다.
   1. 다음에서 **리치 텍스트** 도구 모음에서 **하이퍼링크** 아이콘. ![](assets/link-icon.png)

   1. 다음에서 **링크 만들기** 아래에 나타나는 상자 **URL**&#x200B;을(를) 클릭하거나 연결할 소스의 URL을 입력하거나 붙여넣습니다.

   1. 아래 **표시할 텍스트**, 링크 텍스트를 입력하거나 붙여넣습니다.
   1. **저장**&#x200B;을 클릭합니다.



1. (선택 사항) 이미지를 업데이트에 첨부하려면 **이미지** 아이콘 ![](assets/addimageicon-35x32.png) 컴퓨터에서 이미지를 찾습니다.\
   또는\
   이미지를 업데이트 영역으로 드래그합니다.

   >[!NOTE]
   >
   >* 이미지 아이콘을 보려면 Workfront 관리자가 이미지 추가를 활성화해야 합니다.
   >* 최대 이미지 파일 크기는 7MB입니다. 지원되는 이미지 파일 유형은 .jpg, .gif 및 .png입니다.
   >* 이미지는 개체의 업데이트 탭에서만 액세스할 수 있으며 문서 탭에서는 사용할 수 없습니다.
   >* 텍스트가 아닌 이미지로 업데이트를 보낼 수 있습니다.


1. (선택 사항) 다음 항목 중 하나를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>알림</strong></td> 
      <td>업데이트에 대한 알림을 받아야 하는 사용자를 식별합니다. 개체를 할당하거나 구독하는 사용자는 업데이트가 있을 때 자동으로 알림을 받습니다.<br><p>업데이트에 다른 사용자를 포함하는 방법에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">업데이트에 다른 사용자 태그 지정</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>커밋 일자</strong></td> 
      <td>날짜 선택기에서 작업 항목을 완료하기로 약정한 날짜를 선택합니다. 커밋 일자에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">커밋 일자 개요</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상황</strong></td> 
      <td>작업 또는 문제에 대한 새 조건을 선택합니다. 조건 선택에 대한 자세한 내용은 <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">작업 및 문제에 대한 상태 업데이트</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태</strong></td> 
      <td>현재 상태 옆의 화살표를 클릭한 다음, 드롭다운 메뉴에서 원하는 상태를 선택합니다. 상태 설정에 대한 자세한 내용은 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">작업 상태 업데이트</a>.<p>작업 항목의 상태를 업데이트해도 프로젝트의 상태가 자동으로 변경되지 않습니다. 프로젝트 설정 방법에 따라 프로젝트 상태를 별도로 업데이트해야 할 수 있습니다. 다양한 프로젝트 업데이트 유형에 대한 자세한 내용은 을 참조하십시오. <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형 선택 </a>.</p><p><b>메모</b>

   작업 항목이 승인 보류 중 상태인 동안에는 상태를 변경할 수 없습니다.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>완료 막대</strong></td> 
      <td>(작업에서만 사용 가능) 진행률 표시줄을 원하는 비율로 밀어 완료된 작업의 비율을 나타냅니다. 완료 표시줄을 두 번 클릭하고 완료율을 입력할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>내 회사에 비공개</strong></td> 
      <td> <p>회사 외부의 사용자가 이 업데이트를 볼 수 있는 액세스 권한을 보유하지 못하도록 하려면 이 옵션을 비활성화하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **업데이트** Workfront 개체에 업데이트를 추가합니다.

   >[!NOTE]
   >
   >을 클릭하면 7초 동안 작은 팝업 창이 나타납니다. **업데이트**&#x200B;를 클릭하여 업데이트를 실행 취소하고 업데이트가 게시되기 전에 편집 창으로 돌아갈 수 있습니다. 실행 취소 팝업을 취소하거나, 팝업이 사라질 때까지 기다리거나, 페이지에서 벗어나면 업데이트가 게시됩니다.
   >
   >Workfront 관리자가 액세스 수준에서 &quot;사용자가 주석을 삭제하는 것을 허용하지 않음&quot; 설정을 선택하면 주석을 실행 취소할 수 없습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 및 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. 업데이트에 회신하려면 다음을 참조하십시오. [업데이트에 대한 회신](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--
### Add an update to a work item in the Preview environment

>[!NOTE]
>
> In the Preview environment, the following functionality is available only for issues, after opting in the Beta program for the new commenting experience.
> 
> In the Production environment, the following functionality is available for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md). 

1. Locate the object you want to add comments to, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Activate the **Beta** toggle in the upper-right corner of the Updates area. This switches the Updates area to the new commenting experience. 
1. Click the **Comments** tab in the upper-left corner of the Updates area.
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any attributes on the **Rich Text** toolbar as you type.

   | **Attribute** |**Toolbar Button** |**Mac Shortcut Keys** |**PC Shortcut Keys** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png)|⌘+b |Ctrl+B |
   | Italics | ![mceclip9.png](assets/mceclip9.png)|⌘+i |Ctrl+I |
   | Underline | ![mceclip8.png](assets/mceclip8.png)|⌘+u |Ctrl+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png)|⌘+K |Ctrl+K |
   | Bulleted List | ![mceclip6.png](assets/mceclip6.png)|⌘+Shift+8 |Ctrl+Shift+8 |
   | Numbered List | ![mceclip5.png](assets/mceclip5.png)|⌘+Shift+7 |Ctrl+Shift+7 |
   | Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |Ctrl+Shift+9 |

    To stop formatting text, deselect the attribute on the **Rich Text** toolbar.

   >[!NOTE]
   >
   >* Formatting also displays in any email notification users receive containing your update.
   >* Rich Text formatting applied to an update in an email does not display on the update when viewed in the Updates tab.  
   >* If your organization uses Workfront with Internet Explorer, any formatted text pasted into an update loses its Rich Text formatting and displays as plain text. You can reformat the text using the attributes on the Rich Text toolbar.
   >* Rich Text formatting is not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.

   ************ HIDE THIS ********* 1. (Optional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting.

   ********  HIDE THIS ******** 1. (Optional) Add any emojis to your update.

   >[!NOTE]
   >
   >* Workfront does not replace punctuation emoticons such as :) with emojis.
   >* Emojis are not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.
   >* The emoji feature in Workfront utilizes Unicode characters and, as such, displays only on browsers and operating systems that support Unicode code points. Users on a platform, browser, or operating system version different than yours might not have access to the same emojis.
   >* An unsupported emoji is represented by a black or white box.
   >* Windows 7 supports only black and white emojis.  
   >* Emojis that are applied to an update made via email do not display on the update when viewed in the Updates area.

1. (Optional) To add a URL link to additional information sources:

   1. Click in your update where you want to insert a link.
   1. On the **Rich Text** toolbar, click the **Hyperlink** icon. ![](assets/link-icon.png)  

   1. In the **Create Link** box that appears, under **URL**, type or paste the URL of the source to which you want to link.
   
   1. Under **Text to display**, type or paste the link text.
   1. Click **Save**.   
1. Click **Submit**. 
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********)
1. (Optional) Click the **Like** icon![](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes.

1. (Optional) Click the **System Activity** tab to view updates logged by the system. When a goal is updated, Workfront generates a note about that update that and displays it in the System Activity tab. Workfront also records a system update when a result, activity, or project is added to the goal or when it is updated. 

1. (Conditional and Optional) If you included additional people in your comment, click on the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

-->



## 업데이트 정보 복사

업데이트를 복사할 수 있는 방법에는 여러 가지가 있습니다. 링크를 복사한 후 다른 사용자와 링크를 공유하여 업데이트를 표시할 수 있습니다.

* [업데이트 복사](#copy-the-update)
* [스레드 링크 복사](#copy-the-thread-link)
* [업데이트 링크 복사](#copy-the-update-link)

### 업데이트 복사 {#copy-the-update}

이 옵션은 특정 업데이트의 텍스트를 클립보드로 복사합니다.

1. 복사하려는 업데이트 또는 회신으로 이동합니다.
1. 다음을 클릭합니다. **자세히** 메뉴를 선택한 다음 **본문 복사**.

   ![본문 복사 를 선택합니다](assets/update-stream-copy-body-text-350x152.png)

### 스레드 링크 복사 {#copy-the-thread-link}

이 옵션은 스레드를 다른 사용자와 공유할 수 있도록 전체 스레드 링크를 클립보드에 복사합니다.

1. 복사할 업데이트 스레드로 이동합니다.
1. 다음을 클릭합니다. **자세히** 메뉴를 선택한 다음 **스레드 링크 복사**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### 업데이트 링크 복사 {#copy-the-update-link}

이 옵션은 특정 업데이트 링크를 클립보드에 복사합니다. 업데이트 링크를 공유하면 해당 링크를 따르는 사용자에게 업데이트 주위에 테두리가 표시됩니다.

1. 복사하려는 업데이트 또는 회신으로 이동합니다.
1. 다음을 클릭합니다. **자세히** 개별 업데이트 옆에 있는 메뉴를 클릭한 다음 **업데이트 링크 복사**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## 업데이트 또는 회신 삭제

Workfront 관리자가 제공하는 액세스 권한에 따라, 오브젝트의 업데이트 탭에서 추가한 업데이트를 삭제할 수 있습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 이 문서에서 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Workfront 사용자(Workfront 관리자 포함)는 다른 사용자가 업데이트한 내용을 삭제할 수 없습니다. 그러나 사용자의 액세스 수준에서 자체 업데이트를 삭제할 수 있는 경우 Workfront 관리자가 해당 사용자로 로그인하여 수행한 업데이트를 삭제할 수 있습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 및 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 삭제할 업데이트 또는 회신으로 이동합니다.
1. 다음을 클릭합니다. **자세히** 삭제할 업데이트 또는 답글 옆에 있는 메뉴를 클릭한 다음 **삭제**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 표시되는 메시지에서 다음을 클릭합니다. **확인**.

>[!NOTE]
>
>이미지가 첨부된 업데이트를 삭제하면 댓글과 이미지가 모두 삭제됩니다.

## 타임시트에 업데이트 추가

1. 업데이트할 타임시트로 이동합니다.
1. 타임시트를 클릭하여 엽니다.
1. 타임시트 하단에서 **주석 포함**.
1. 타임시트의 맨 아래에 표시되는 상자에 업데이트를 입력합니다.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (조건부) 승인을 위해 타임시트를 제출하지 않고 업데이트를 저장하려면 **나중에 저장**.

   또는

   업데이트를 저장하고 승인을 위해 타임시트를 제출하려면 **승인을 위해 제출**.

   또는

   타임시트가 승인자와 함께 설정되지 않은 경우 다음을 클릭하십시오. **타임시트 저장 및 닫기** 업데이트를 저장합니다.

## 시스템 업데이트 활성화 또는 비활성화

Workfront 개체의 업데이트 탭에는 두 가지 유형의 정보가 표시됩니다.

* **사용자 업데이트:** 사용자 업데이트는 사용자와 시스템의 다른 사용자가 입력하는 주석입니다.

   ![](assets/user-update-cl-350x277.png)

* **시스템 업데이트:** 시스템은 객체의 문서에 대한 편집 또는 변경 사항뿐만 아니라 에셋 제거, 버전 추가 또는 삭제, 승인 요청 첨부 또는 제거를 기록하는 레코드를 업데이트합니다.

   ![](assets/system-updates-cl-350x277.png)

Workfront 라이선스에 따라 시스템 업데이트가 기본적으로 활성화될 수 있습니다. Workfront 관리자는에 설명된 대로 시스템 업데이트에서 추적되는 항목을 결정할 수 있습니다. [시스템 추적 업데이트](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). 모든 객체에 대한 사용자 업데이트만 표시되도록 시스템 업데이트 또는 활동을 필터링할 수도 있습니다.

사용자 업데이트와 시스템 업데이트의 차이점에 대한 자세한 내용은 [시스템 추적 업데이트](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

시스템 업데이트를 활성화하거나 비활성화하려면 다음 작업을 수행하십시오.

1. 다음을 클릭합니다. **업데이트** 개체의 탭입니다.
1. 클릭 **시스템 업데이트 표시** 스위치를 왼쪽(비활성화) 또는 오른쪽(활성화)으로 밀어서 놓습니다.

   ![](assets/show-system-updates-qs-350x55.png)

   이 옵션은 Workfront 전체의 모든 오브젝트에서 영구적이며 Workfront에서 로그아웃한 경우에도 선택한 위치에 유지됩니다.
