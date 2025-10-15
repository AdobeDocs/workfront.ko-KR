---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트에 대한 회신
description: 누군가 작업 개체에 대한 업데이트를 추가하거나 답장을 보내면 해당 개체의 업데이트 섹션에 있는 통신 스레드에 답장이 나타납니다. 오브젝트에 대한 보기 액세스 권한이 있는 경우 업데이트 또는 좋아요 표시에 회신을 추가할 수 있습니다.
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 업데이트에 대한 회신

<!-- Audited: April 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

누군가 작업 오브젝트에 대한 댓글 또는 시스템 업데이트에 답글을 달면 해당 답글이 해당 오브젝트의 업데이트 섹션에 있는 댓글 및 모두 탭의 통신 스레드에 나타납니다.

>[!IMPORTANT]
>
>시스템 활동 탭에서 시스템 업데이트에 회신할 수 없습니다. 2024년 4월 11일 이전의 기존 댓글 달기 환경에서 수행된 시스템 업데이트에 대한 모든 답글은 읽기 전용으로 표시됩니다.

이 문서에서는 Workfront에 있는 대부분의 개체에서 댓글에 응답하는 방법에 대해 설명합니다. 다양한 개체의 업데이트 섹션 간의 차이점을 보려면 [업데이트 섹션 개요](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 패키지</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스</strong></td> 
   <td> <p>문제 및 문서의 경우:</p>

<ul><li><p>기여자 이상</p></li>
   <li><p>요청 이상</p></li></ul>

<p>기타 모든 객체의 경우:</p>
   <ul><li><p>밝거나 높음</p></li>
   <li><p>검토 이상</p></li></ul>

</td>  
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>업데이트가 있는 오브젝트에 대한 보기 또는 편집 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>오브젝트에 대한 권한 보기</p> </td> 
  </tr> 
 </tbody> 
   </table>

자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p> 
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Workfront에서 업데이트 또는 회신에 회신

볼 수 있는 오브젝트의 스레드에서 댓글에 답글을 달 수 있습니다. 또는 Workfront 또는 그룹 관리자로 로그인하여 다른 사용자를 대신하여 댓글에 답글을 달 수 있습니다. 자세한 내용은 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)을 참조하십시오.

### 댓글에 회신

오브젝트의 업데이트 섹션에 있는 댓글에 대한 회신은 Workfront에 있는 대부분의 오브젝트에서 유사합니다.

1. 회신을 추가할 객체로 이동합니다.
1. **업데이트**&#x200B;를 클릭한 다음 개체에 대한 **댓글** 탭을 클릭하고 회신할 댓글 또는 회신을 찾습니다

   또는

   **모두** 탭을 클릭한 다음 **댓글에서 답글 작성**&#x200B;을 클릭하여 댓글 탭에서 댓글을 열고 회신합니다. 모두 탭에서 회신할 수 없습니다.

1. (선택 사항) 회신에 이전 업데이트의 텍스트를 포함하려면 회신할 댓글의 오른쪽 상단에 있는 **자세히** 메뉴를 클릭한 다음 **회신 견적**&#x200B;을 클릭합니다. 이전 업데이트의 텍스트가 입력 영역에 세로로 회색 선으로 표시됩니다.
1. **회신**&#x200B;을 클릭합니다.

   ![빈 상자를 업데이트하는 회신](assets/reply-to-update-empty-box.png)

   **회신 추가...** 상자 아래쪽에 대화에 적극적으로 참여한 사용자가 표시되어 더 이상 관련이 없는 사용자를 추가하거나 제거할 수 있습니다. 이러한 사용자는 오브젝트에 가입된 사용자와 함께 오브젝트에 대한 업데이트 또는 회신이 이루어질 때마다 알림을 받습니다. 더 많은 사용자에 태그를 지정하여 회신에 추가할 수도 있습니다.  더 많은 사용자를 태그 지정하려면 [업데이트에 다른 사용자 태그 지정](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.

   >[!TIP]
   >
   >   기존 회신에 회신을 추가하려면 **회신 추가...** 상자에 입력을 시작하거나 원래 댓글에서 **회신**&#x200B;을 클릭할 수 있습니다. 답변은 스레드 끝에 추가됩니다.

1. 답글 입력을 시작하고 리치 텍스트 도구 모음에서 추가 옵션을 사용하십시오. 서식 있는 텍스트나 기타 업데이트 기능에 대한 자세한 내용은 [작업 업데이트](../updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

1. 회신을 저장하려면 **제출**&#x200B;을 클릭하세요.

1. (선택 사항) 회신을 관리할 추가 옵션을 보려면 회신할 댓글의 오른쪽 상단에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭합니다. 자세한 내용은 [작업 업데이트](../updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

<!--
### Reply to an update or reply in the legacy Updates section

1. Go to the object to which you want to add a reply.
1. On the **Updates** tab for the object, find the update or reply to which you want to reply.

1. (Optional) To view an image in the existing update do one of the following:

   * Click the **Preview** icon ![](assets/previewimageicon-31x31.png) on the image thumbnail to open the full-size image in a new browser tab.
   * Click the **Download** icon ![](assets/downloadimageicon.png) on the image thumbnail to download the image.

1. Click **Reply** on the update, then type a reply in the box that appears.

   You can see the users who are actively engaged in the conversation or tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)
   
1. (Optional) To include text from a previous update in your reply, click the **More** menu next to the update or reply you want to quote, then click **Quote Reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. (Optional) Use formatting, emojis, include links, or images as explained in the section "Use Rich Text in a Workfront update" in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Click **Reply** to save the reply.

-->

## 이메일 알림에서 업데이트에 회신

이메일 알림 구성 방식에 따라 액세스 권한이 있는 특정 오브젝트가 업데이트될 때 이메일 알림을 받을 수 있습니다.

다음과 같은 방법으로 이메일 알림에서 업데이트에 회신할 수 있습니다.

* 받은 이메일에 답장을 보냅니다. 답글 이메일이 원래 의견에 대한 Workfront 답글로 추가됩니다.
* 이메일 내의 댓글 버튼을 사용하여 Workfront으로 다시 이동하고 업데이트 영역에서 업데이트에 회신할 수 있습니다.

다음은 작업의 업데이트 탭에서 업데이트한 결과로서 트리거되는 이메일 알림의 예입니다.

![email.png](assets/email-350x202.png)

자세한 내용은 [전자 메일 알림에 회신](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md)을 참조하세요.






