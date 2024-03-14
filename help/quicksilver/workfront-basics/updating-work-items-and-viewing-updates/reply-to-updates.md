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
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# 업데이트에 대한 회신

{{preview-and-fast-release}}

<!--remove legacy and new experience references when we remove the legacy updates in the UI - Jan 2024???-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 

-->

>[!IMPORTANT]
>
>현재 Adobe Workfront의 댓글 달기 환경을 다시 디자인하고 있습니다.
>
>댓글 달기 경험에 액세스하는 객체에 따라 업데이트 섹션에 다음과 같은 기능이 표시될 수 있습니다.
>* 새로운 경험
>* 기존 경험
>* 새로운 및 기존 경험
>
>새 댓글 달기 경험과 사용 가능 여부에 대한 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>새 주석 달기 경험은 Workfront 오브젝트의 업데이트 섹션에만 사용할 수 있고 다음 영역에서 오브젝트에 액세스할 때는 사용할 수 없습니다.
>
> * 홈
> * 목록의 요약 패널
> * 타임시트의 요약 패널
> * 업무 균형자의 요약 패널
>
><span class="preview">새로운 댓글 달기 환경은 빠른 릴리스 프로세스를 선택한 고객을 위해 미리보기 환경의 목록, 타임시트 및 업무 균형자의 요약 패널과 프로덕션 환경에서 사용할 수 있습니다.</span>

누군가 작업 개체에 대한 댓글 또는 시스템 업데이트에 답글을 달면 해당 답글이 해당 개체의 업데이트 섹션에 있는 통신 스레드에 나타납니다.

>[!IMPORTANT]
>
>새 댓글 달기 환경에서 시스템 업데이트에 회신할 수 없습니다. 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--adjust the sentence before the second IMPORTANT and remove this important note when we remove legacy from the system-->

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>문제 및 문서에 대해 요청 이상, 기타 모든 오브젝트에 대해 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>문제 및 문서에 대한 요청자 이상, 기타 모든 오브젝트에 대한 검토자 이상</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>오브젝트에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## Workfront에서 업데이트 또는 회신에 회신

볼 수 있는 오브젝트의 스레드에서 댓글에 답글을 달 수 있습니다. 또는 Workfront 또는 그룹 관리자로 로그인하여 다른 사용자를 대신하여 댓글에 답글을 달 수 있습니다. 자세한 내용은 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

댓글 또는 답글에 대한 답글은 선택한 경험과 개체에 따라 다릅니다.

### 새 댓글 달기 경험을 사용할 때 댓글에 회신

새 댓글 달기 환경에서 사용할 수 있는 기능과 개체에 대한 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. 회신을 추가할 객체로 이동합니다.
1. 클릭 **업데이트**&#x200B;을(를) 클릭하고 **댓글** 개체 탭과 회신할 댓글 또는 회신을 찾습니다.

   또는

   <span class="preview">다음을 클릭합니다. **모두** 탭을 클릭한 다음 를 클릭합니다 **댓글로 회신** 를 클릭하여 댓글 탭에서 댓글을 열고 회신합니다. 모두 탭에서 회신할 수 없습니다.</span>

1. (선택 사항) 회신에 이전 업데이트의 텍스트를 포함하려면 **자세히** 회신할 댓글의 오른쪽 위 모서리에 있는 메뉴를 클릭한 다음 **견적 회신**. 이전 업데이트의 텍스트가 입력 영역에 세로로 회색 선으로 표시됩니다.
1. 클릭 **답변**.

   ![](assets/reply-to-update-empty-box.png)

   대화에 적극적으로 참여하는 사용자를 아래 부분에서 확인할 수 있습니다 **회신 추가...** 상자를 선택하면 더 이상 관련이 없는 항목을 추가하거나 제거할 수 있습니다. 이러한 사용자는 오브젝트에 가입된 사용자와 함께 오브젝트에 대한 업데이트 또는 회신이 이루어질 때마다 알림을 받습니다. 더 많은 사용자에 태그를 지정하여 회신에 추가할 수도 있습니다.  더 많은 사용자에 태그를 지정하려면 다음을 참조하십시오. [업데이트에 다른 사용자 태그 지정](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   기존 회신에 추가 회신을 추가하려면 **회신 추가...** 상자 또는 클릭 **답변** 원래 주석에. 답변은 스레드 끝에 추가됩니다.

1. 답글 입력을 시작하고 리치 텍스트 도구 모음에서 추가 옵션을 사용하십시오. 리치 텍스트 또는 기타 업데이트 기능 사용에 대한 자세한 내용은 [작업 업데이트](../updating-work-items-and-viewing-updates/update-work.md).

1. 클릭 **제출** 회신을 저장합니다.

1. (선택 사항) **자세히** 메뉴 ![](assets/more-menu.png) 답글을 관리할 추가 옵션을 보려면 답글을 달려는 댓글의 오른쪽 상단 모서리에서 을(를) 참조하십시오. 자세한 내용은 [작업 업데이트](../updating-work-items-and-viewing-updates/update-work.md).

### 업데이트에 대한 회신 또는 레거시 업데이트 섹션의 회신

1. 회신을 추가할 객체로 이동합니다.
1. 다음에서 **업데이트** 오브젝트의 탭에서 회신할 업데이트 또는 회신을 찾습니다.

1. (선택 사항) 기존 업데이트에서 이미지를 보려면 다음 중 하나를 수행하십시오.

   * 다음을 클릭합니다. **미리 보기** 아이콘 ![](assets/previewimageicon-31x31.png) 이미지 축소판을 클릭하여 새 브라우저 탭에서 전체 크기 이미지를 엽니다.
   * 다음을 클릭합니다. **다운로드** 아이콘 ![](assets/downloadimageicon.png) 이미지를 다운로드하려면 이미지 썸네일에서 을(를) 선택합니다.

1. 클릭 **답변** 업데이트에서 나타나는 상자에 회신을 입력합니다.

   해당 업데이트 스레드의 맨 위에서 대화에 적극적으로 참여하거나 각 회신에 태그를 지정한 사용자를 볼 수 있습니다. 이러한 사용자는 오브젝트에 가입된 사용자와 함께 오브젝트에 대한 업데이트 또는 회신이 이루어질 때마다 알림을 받습니다. 더 많은 사용자에 태그를 지정하여 회신에 추가할 수도 있습니다.  더 많은 사용자에 태그를 지정하려면 다음을 참조하십시오. [업데이트에 다른 사용자 태그 지정](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (선택 사항) 회신에 이전 업데이트의 텍스트를 포함하려면 **자세히** 견적을 작성할 업데이트 또는 회신 옆에 있는 메뉴 **견적 회신**. 이전 업데이트의 텍스트가 입력 영역에 세로로 회색 선으로 표시됩니다.
1. (선택 사항) 문서의 &quot;Workfront 업데이트에서 리치 텍스트 사용&quot; 섹션에 설명된 대로 서식, 이모지를 사용하고, 링크 또는 이미지를 포함합니다 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 클릭 **답변** 회신을 저장합니다.

## 이메일 알림에서 업데이트에 회신

이메일 알림 구성 방식에 따라 액세스 권한이 있는 특정 오브젝트가 업데이트될 때 이메일 알림을 받을 수 있습니다.

다음과 같은 방법으로 이메일 알림에서 업데이트에 회신할 수 있습니다.

* 받은 이메일에 답장을 보냅니다. 답글 이메일이 원래 의견에 대한 Workfront 답글로 추가됩니다.
* 이메일 내의 댓글 버튼을 사용하여 Workfront으로 다시 이동하고 업데이트 영역에서 업데이트에 회신할 수 있습니다.

다음은 작업의 업데이트 탭에서 업데이트한 결과로서 트리거되는 이메일 알림의 예입니다.

![email.png](assets/email-350x202.png)

자세한 내용은 [이메일 알림에 회신](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






