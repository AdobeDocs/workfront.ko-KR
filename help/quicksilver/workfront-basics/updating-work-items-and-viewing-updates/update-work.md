---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 작업 업데이트
description: Adobe Workfront 개체(프로젝트, 작업 또는 문제)에 업데이트를 추가하여 개체의 진행 상황을 전달할 수 있습니다. 객체에 할당되거나 가입된 사용자는 업데이트를 볼 수 있습니다. 또한 사용자에게 업데이트에 관심을 갖도록 태그를 지정할 수도 있습니다.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 1%

---

# 작업 업데이트

<!-- Drafted for commenting experience: 

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the way you update work when using the Updates section of an object. 
>You can access the new design by enabling the commenting Beta. 
>Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

업데이트 섹션에서 Adobe Workfront의 대부분의 개체에 주석을 추가할 수 있습니다. 업데이트 섹션을 표시하는 객체에 대한 자세한 내용은 [업데이트 섹션 개요](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

개체에 주석을 달 때 Workfront 개체(프로젝트, 작업 또는 문제)에 업데이트를 추가하여 개체의 진행 상황을 전달할 수 있습니다. 객체에 할당되거나 가입된 사용자는 업데이트를 볼 수 있습니다. 또한 사용자에게 업데이트에 관심을 갖도록 태그를 지정할 수도 있습니다. 태그가 지정된 사용자는 인앱 알림 및 업데이트에 대한 이메일을 받게 됩니다.

이 페이지의 정보는 Workfront 개체에 대해 주석을 달 수 있는 방법과 프로젝트, 작업 및 문제를 업데이트하는 방법에 대해 설명합니다. 목표에 대한 댓글 달기에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 주석 관리](../../workfront-goals/goal-management/manage-goal-comments.md). Workfront 목표에 액세스하려면 추가 라이센스가 있어야 합니다.


Workfront의 다음 영역에서 프로젝트, 작업 및 문제에 대한 업데이트를 추가할 수 있습니다.

* Workfront 개체의 업데이트 섹션에 있습니다
* 홈 영역에서(작업 및 문제)
* 객체 목록의 요약 패널에서 작업 및 문제
* 작업표에서(작업 및 문제)

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
이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>문제 및 문서에 대한 요청 이상 다른 모든 객체에 대해 검토 또는 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>업데이트가 있는 객체에 대한 액세스 보기 또는 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>객체에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 항목에 업데이트 추가

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects

Adding an update to a work item differs depending on what version of the Updates section and what object you choose. 

### Add an update to a work item in the current Updates section

>[!NOTE]
>
>The following functionality is available for all objects except for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. 업데이트를 제공할 작업 항목(예: 프로젝트, 작업 또는 문제)으로 이동합니다.
1. 을(를) 클릭합니다. **업데이트** 섹션을 참조하십시오.
1. 클릭 **새 업데이트 시작,** 그런 다음 업데이트를 입력합니다.
1. (선택 사항) 리치 텍스트를 사용하거나 업데이트에 이모지, 링크 또는 이미지를 추가하여 컨텐츠를 개선합니다. 자세한 내용은 이 문서의 &quot;Workfront 업데이트에서 리치 텍스트 사용&quot; 섹션을 참조하십시오
1. (선택 사항) 작업 항목에 대한 다음 정보를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>알림</strong></td> 
      <td>업데이트에 대한 알림을 받아야 하는 사용자를 식별합니다. 업데이트되면 개체에 할당되거나 구독한 사용자가 자동으로 알림을 받습니다.<br><p>업데이트에 다른 사용자를 포함하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">업데이트에 다른 사용자에게 태그 지정</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>커밋 일자</strong></td> 
      <td>날짜 선택기에서 작업 항목을 완료하기 위해 커밋하는 날짜를 선택합니다. 커밋 날짜에 대한 자세한 내용은 <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">커밋 날짜 개요</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상황</strong></td> 
      <td>작업 또는 문제에 대한 새 조건을 선택합니다. 조건 선택에 대한 자세한 내용은 <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">작업 및 문제에 대한 조건 업데이트</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태</strong></td> 
      <td>현재 상태 옆의 화살표를 클릭한 다음 드롭다운 메뉴에서 원하는 상태를 선택합니다. 상태 설정에 대한 자세한 내용은 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">작업 상태 업데이트</a>.<p>작업 항목의 상태를 업데이트해도 프로젝트의 상태가 자동으로 변경되지 않습니다. 프로젝트 설정 방식에 따라 프로젝트 상태를 별도로 업데이트해야 할 수 있습니다. 다양한 프로젝트 업데이트 유형에 대한 자세한 내용은 <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형을 선택합니다 </a>.</p><p><b>메모</b>

   작업 항목이 승인 대기 중 상태인 동안에는 작업 항목의 상태를 변경할 수 없습니다.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>완료 표시줄</strong></td> 
      <td>(작업에서만 사용 가능) 진행률 표시줄을 원하는 비율로 슬라이딩하여 완료된 작업의 백분율을 나타냅니다. 완료 표시줄을 두 번 클릭하고 완료율을 입력할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>내 회사에 비공개</strong></td> 
      <td> <p>회사 외부의 사용자가 이 업데이트를 볼 수 없도록 하려면 이 옵션을 비활성화하십시오.</p> 
      <p><b>메모</b></p>
      <p>이 옵션은 사용자가 회사와 연결된 경우에만 표시됩니다.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **업데이트** Workfront 개체에 업데이트를 추가하려면 다음을 수행하십시오.

   >[!NOTE]
   >
   >클릭 후 7초 동안 작은 팝업 창이 나타납니다 **업데이트**&#x200B;업데이트를 실행 취소하고 업데이트가 게시되기 전에 편집 창으로 돌아갈 수 있도록 합니다. 실행 취소 팝업을 취소하거나, 업데이트가 사라질 때까지 기다리거나, 페이지에서 멀리 이동하는 경우 업데이트가 게시됩니다.
   >
   >Workfront 관리자가 액세스 수준에서 &quot;사용자가 주석을 삭제할 수 없음&quot; 설정을 선택하면 설명을 실행 취소할 수 없습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 및 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. 업데이트에 응답하려면 다음을 참조하십시오 [업데이트에 회신](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--

### Add an update to a work item using the commenting Beta experience


>[!NOTE]
>
>The functionality described in this section is available for the following objects:
>
>* <span class="preview">Issues, when you enable the commenting Beta experience.</span>
>
>   <span class="preview">This functionality is available only for the Updates section of issues, and it is not available for the following areas:</span>
>
>   * <span class="preview">Home</span>
>   * <span class="preview">Summary panel in lists</span>
>   * <span class="preview">Summary panel in timesheets</span>
>* Goals
>
>   The commenting experience Beta is the default current experience for goals.
>   You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


1. Locate the object you want to update, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Click **Try out the commenting Beta** button in the lower-right corner of the Updates area, then click **Agree** on the Beta agreement. This switches the Updates area to the commenting Beta experience. 
   The **Comments** tab is selected by default. 
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any of the following options from the **Rich Text** toolbar to enhance your text: 

   * Bold
   * Italics
   * Underline
   * Link
   * Bulleted List
   * Numbered List
   * Add attachment (mark this parenthesis as draft: ************ this might be renamed)
   
   For more information, see the "Use Rich Text in a Workfront update" section in this article.

   >[!TIP]
   >
   >   If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
   >
   > ![](assets/real-time-new-red-indicator-unified-commenting.png)



1. Click **Submit** to add the update to the Workfront object. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment, or remove any of the tagged users. 
   You can edit your comment within 15 from submitting it. An "Edited" indicator is added to the left of the date stamp that displays when the comment was updated. 

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********). For information about replying to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Optional) Click the **Like** icon![](assets/like-icon.png). The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When the object or any of its children are updated, Workfront generates a note about that update and displays it in the System Activity tab. 

   For more information see [Updates section  overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >You cannot add a comment to a system update.
-->


## Workfront 업데이트에서 리치 텍스트 사용

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.

>[!NOTE]
>
>Some of the options in the Rich Text toolbar are not available for the commenting Beta experience.-->


리치 텍스트를 사용하거나 이모지, 링크 또는 이미지와 같은 다양한 항목을 추가하여 업데이트를 향상시킬 수 있습니다.

1. 업데이트 영역으로 이동하여 댓글을 입력을 시작합니다.
1. (선택 사항) 업데이트에 서식 있는 텍스트 서식을 추가하려면 **리치 텍스트** 입력할 때 도구 모음

   | **속성** | **도구 모음 단추** | **Mac 바로 가기 키** | **PC 바로 가기 키** |
   |---|---|---|---|
   | 볼드체 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 기울임꼴 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 밑줄 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | 하이퍼링크 | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl+K |
   | 글머리 기호 목록 | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 번호 매기기 목록 | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | 견적 차단 | ![](assets/block-quote-icon-large.png) | Shift ⌘+9 | Ctrl+Shift+9 |

   텍스트 서식을 중지하려면 **리치 텍스트** 도구 모음

   >[!NOTE]
   >
   >* 또한 사용자 업데이트가 포함된 이메일 알림 사용자가 받는 모든 전자 메일 알림에 서식이 표시됩니다.
   >* 전자 메일의 업데이트에 적용된 리치 텍스트 서식은 업데이트 탭에서 볼 때 업데이트에 표시되지 않습니다.
   >* 조직에서 Internet Explorer와 함께 Workfront을 사용하는 경우 업데이트에 붙여넣은 서식이 지정된 텍스트는 리치 텍스트 서식을 잃고 일반 텍스트로 표시됩니다. 리치 텍스트 도구 모음의 특성을 사용하여 텍스트 서식을 다시 지정할 수 있습니다.
   >* 작업표 영역에서 업데이트하거나 보고서에 표시된 메모 및 마지막 조건 개체에 대해서는 서식 있는 텍스트 서식을 사용할 수 없습니다.


1. (선택 사항) 이전 업데이트나 다른 출처의 텍스트를 포함하고 자신의 업데이트와 구분하려면 블록 인용으로 표시할 수 있습니다. 을(를) 클릭합니다. **블록 인용** 아이콘 ![](assets/block-quote-small.png) 인용할 텍스트를 입력합니다. 인용된 텍스트는 세로 회색 선으로 표시됩니다. 을(를) 클릭합니다. **블록 인용** 아이콘을 다시 클릭하여 일반 형식으로 돌아갑니다.

   ![](assets/block-quote-marked-350x144.png)

1. (선택 사항) 업데이트에 이모지를 추가합니다.

   >[!NOTE]
   >
   >* Workfront은 다음과 같은 구두점 이모티콘을 이모지로 대체하지 않습니다.
   >* 작업표 영역에서 수행한 업데이트나 보고서에 표시된 메모 및 마지막 조건 개체에 대해서는 이모지를 사용할 수 없습니다.
   >* Workfront의 이모지 기능은 유니코드 문자를 사용하며, 따라서 유니코드 코드 포인트를 지원하는 브라우저 및 운영 체제에만 표시됩니다. 다른 플랫폼, 브라우저 또는 운영 체제 버전의 사용자는 동일한 이모지에 액세스할 수 없습니다.
   >* 지원되지 않는 이모지는 검정색 또는 흰색 상자로 표시됩니다.
   >* Windows 7에서는 흑백 이모지만 지원합니다.
   >* 이메일을 통해 작성된 업데이트에 적용되는 이모지는 업데이트 영역에서 볼 때 업데이트에 표시되지 않습니다.


1. (선택 사항) 추가 정보 소스에 URL 링크를 추가하려면 다음을 수행합니다.

   1. 링크를 삽입할 업데이트를 클릭합니다.
   1. 설정 **리치 텍스트** 도구 모음에서 **하이퍼링크** 아이콘. ![](assets/link-icon.png)

   1. 에서 **링크 만들기** 표시되는 상자 **URL**&#x200B;를 채울 소스의 URL을 입력하거나 붙여넣습니다.

   1. 아래 **표시할 텍스트**&#x200B;링크 텍스트를 입력하거나 붙여넣습니다.
   1. **저장**&#x200B;을 클릭합니다.

1. (선택 사항) 업데이트에 이미지를 첨부하려면 **이미지** 아이콘 ![](assets/addimageicon-35x32.png) 컴퓨터에서 이미지를 찾습니다.\
   또는\
   이미지를 업데이트 영역으로 드래그합니다.

   >[!NOTE]
   >
   >* 이미지 아이콘을 보려면 Workfront 관리자가 이미지 추가를 활성화해야 합니다.
   >* 최대 이미지 파일 크기는 7MB입니다. 지원되는 이미지 파일 유형은 .jpg, .gif 및 .png입니다.
   >* 이미지는 객체의 업데이트 탭에서만 액세스할 수 있으며 문서 탭에서 사용할 수 없습니다.
   >* 이미지를 업데이트하여 텍스트를 전송할 수 없습니다.

1. 클릭 **업데이트**  <!--<span class="preview">or **Submit**</span>, in the commenting Beta experience-->.


## 업데이트 정보 복사

<!--drafted for beta release toggle - remove when copying an update will be available: 

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

업데이트를 복사할 수 있는 방법에는 몇 가지가 있습니다. 링크를 복사한 후 다른 사용자와 링크를 공유하여 업데이트에 연결할 수 있습니다.

* [업데이트 복사](#copy-the-update)
* [스레드 링크 복사](#copy-the-thread-link)
* [업데이트 링크 복사](#copy-the-update-link)

### 업데이트 복사 {#copy-the-update}

이 옵션은 특정 업데이트의 텍스트를 클립보드에 복사합니다.

1. 복사하려는 업데이트 또는 응답으로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴를 클릭한 다음 **본문 복사**.

   ![본문 복사 를 선택합니다](assets/update-stream-copy-body-text-350x152.png)

### 스레드 링크 복사 {#copy-the-thread-link}

이 옵션은 클립보드에 전체 스레드 링크를 복사하므로 다른 사용자와 스레드를 공유할 수 있습니다.

1. 복사할 업데이트 스레드로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴를 클릭한 다음 **스레드 링크 복사**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### 업데이트 링크 복사 {#copy-the-update-link}

이 옵션은 특정 업데이트 링크를 클립보드에 복사합니다. 업데이트 링크를 공유하면 업데이트 주위에 테두리가 표시됩니다.

1. 복사하려는 업데이트 또는 응답으로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 개별 업데이트 옆에 있는 메뉴를 클릭한 다음 **업데이트 링크 복사**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## 업데이트 또는 회신 삭제

Workfront 관리자가 제공하는 액세스 권한에 따라 개체의 업데이트 탭에서 추가한 업데이트를 삭제할 수 있습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 기사 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Workfront 사용자(Workfront 관리자 포함)는 다른 사용자가 수행한 업데이트를 삭제할 수 없습니다. 그러나 사용자의 액세스 수준에서 사용자가 자신의 업데이트를 삭제할 수 있도록 허용하는 경우 Workfront 관리자는 해당 사용자로 로그인하고 업데이트를 삭제할 수 있습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 및 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 삭제할 업데이트나 응답으로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 삭제할 업데이트 또는 회신 옆에 있는 메뉴를 클릭한 다음 **삭제**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 표시되는 메시지에서 **확인** <!--<span class="preview">or **Delete**</span>, in the commenting Beta experience-->.

>[!NOTE]
>
>첨부된 이미지로 업데이트를 삭제하면 주석과 이미지가 모두 삭제됩니다.

## 작업표에 업데이트 추가

1. 업데이트를 만들 작업표로 이동합니다.
1. 작업표를 클릭하여 엽니다.
1. 작업표 하단에서 **댓글 포함**.
1. 작업표 하단에 표시되는 상자에 업데이트를 입력합니다.

   ![작업표_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (조건부) 승인을 위해 작업표를 제출하지 않고 업데이트를 저장하려면 **나중에 저장**.

   또는

   업데이트를 저장하고 승인을 위한 작업표를 제출하려면 **승인을 위한 제출**.

   또는

   작업표가 승인자로 설정되지 않은 경우 **작업표 저장 및 닫기** 업데이트를 저장하려면 다음을 수행하십시오.

## 시스템 업데이트 활성화 또는 비활성화

<!--remove preview with 23.2 production: 

<div class="preview">
>[!NOTE]
>
>It is not possible to disable system updates when using the Beta commenting experience. 
>The information in this section refers only to functionality available in the current Updtes section. 
>For more information about system updates in the Beta version, see [Updates section overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md) 
</div>
-->

Workfront 개체의 업데이트 섹션에는 두 가지 유형의 정보가 표시됩니다.

* **사용자 업데이트:** 사용자 업데이트는 사용자 및 시스템에 있는 다른 사용자가 입력하는 주석입니다.

   ![](assets/user-update-cl-350x277.png)

* **시스템 업데이트:** 시스템 업데이트는 자산 제거, 버전 추가 또는 삭제, 승인 요청 첨부 또는 제거, 객체 문서에 대한 편집 또는 변경 사항을 기록합니다.

   ![](assets/system-updates-cl-350x277.png)

Workfront 라이선스에 따라 시스템 업데이트가 기본적으로 활성화되어 있을 수 있습니다. Workfront 관리자는 [시스템 추적 업데이트](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). 모든 객체에 대한 사용자 업데이트만 표시되도록 시스템 업데이트나 활동을 필터링할 수도 있습니다.

사용자 및 시스템 업데이트 간의 차이에 대한 자세한 내용은 [시스템 추적 업데이트](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

시스템 업데이트를 활성화 또는 비활성화하려면

1. 을(를) 클릭합니다. **업데이트** 탭에서 사용할 수 있습니다.
1. 클릭 **시스템 업데이트 표시** 스위치를 왼쪽(비활성화) 또는 오른쪽(활성화)으로 슬라이딩하려면

   ![](assets/show-system-updates-qs-350x55.png)

   이 옵션은 Workfront의 모든 개체에서 지속되며, Workfront에서 로그아웃해도 선택한 위치에 유지됩니다.

