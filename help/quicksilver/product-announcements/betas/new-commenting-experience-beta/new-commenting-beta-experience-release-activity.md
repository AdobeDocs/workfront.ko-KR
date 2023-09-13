---
product-area: betas
navigation-topic: new-commenting-exprience-beta
title: 새로운 댓글 달기 경험 릴리스 활동
description: Adobe Workfront의 새로운 댓글 달기 환경에 대한 주간 릴리스 활동을 검토합니다.
author: Alina
feature: Product Announcements
role: User, Admin
exl-id: 1c0cb547-ac99-4cdf-8a74-2c47ad5a10ad
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '2047'
ht-degree: 2%

---

# 새로운 댓글 달기 경험 릴리스 활동

<!--take the badge out when it comes to production GA for everyone-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
* <span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> -->


이 페이지에는 현재 Adobe Workfront에서 진행 중인 새 댓글 달기 환경의 릴리스 타임라인에 대한 정보가 포함되어 있습니다.

현재 사용할 수 있거나 연구 중인 기능 목록을 포함하여 새 댓글 달기 환경에 대한 일반 정보는 다음을 참조하십시오. [새 댓글 달기 환경](../new-commenting-experience-beta/unified-commenting-experience.md).


>[!IMPORTANT]
>
>새로운 댓글 달기 환경은 23.2 릴리스와 함께 Beta로 출시되었습니다. 원본 릴리스에 대한 자세한 내용은 [23.2 릴리스 개요](../../product-releases/23.2-release-activity/23-2-release-overview.md).
>
>Beta 댓글 달기 경험을 지원하는 Workfront 개체에 릴리스된 기능은 유일한 댓글 달기 경험으로 다음 개체의 업데이트 섹션에도 릴리스됩니다.
>* 목표
>* 보드 영역의 카드.

## 릴리스 타임라인

새로운 댓글 달기 경험을 반복적으로 출시할 예정입니다. 각 릴리스의 일부 오브젝트에 영향을 줍니다. 처음에는 작은 기능 세트가 릴리스될 수 있으며 시간이 지남에 따라 더 많은 기능이 나머지 개체에 추가됩니다.

업데이트 섹션이 표시되는 Workfront 개체에 대한 자세한 내용은   [업데이트 섹션 개요](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

다음은 프로덕션 환경에 대한 새로운 댓글 달기 환경의 릴리스에 대한 주요 이정표가 포함된 계획된 타임라인입니다. 아래 이정표 외에도, 더 작은 개선 사항으로 주석 달기 환경을 계속 개선해 나갈 것입니다. 릴리스된 모든 기능에 대한 자세한 내용은 [릴리스된 기능](#released-features) 이 문서의 섹션.

* 23.2 릴리스(2023년 4월 6일):
   * 문제에 대한 Experience Beta 주석 달기
   * 목표에 대한 새로운 댓글 달기 경험(유일한 경험으로)
* 23.3 릴리스(2023년 7월 20일):
   * 프로젝트, 작업 및 문서에 대한 Experience Beta에 댓글을 남깁니다.
   * 보드 영역의 카드에 대한 새로운 댓글 달기 경험(유일한 경험으로)
* 2023년 4분기 릴리스(제한된 릴리스, 빠른 릴리스를 선택하는 고객만 사용 가능) 중:
   * 템플릿, 템플릿 작업, 프로그램, 포트폴리오, 팀, 사용자 및 타임시트에 대한 새로운 댓글 달기 경험(유일한 경험임)
   * 프로젝트, 작업, 문제 및 문서에 대한 Experience Beta 댓글을 달 수 있는 것이 기본 옵션이 됩니다. Beta 레이블이 제거됩니다.
* 2023년 4분기(23.10) 릴리스 포함(2023년 10월)
   * 템플릿, 템플릿 작업, 프로그램, 포트폴리오, 팀, 사용자 및 타임시트에 대한 새로운 댓글 달기 경험(유일한 경험임)
   * 프로젝트, 작업, 문제 및 문서에 대한 새로운 댓글 달기 환경이 기본 옵션이 됩니다. 이렇게 하면 새 댓글 달기 환경의 베타 단계가 종료됩니다.
* 2023년 말:
   * 기존 댓글 달기 경험은 프로젝트, 작업, 문제 및 문서 개체에 대한 보조 옵션으로 유지됩니다.

  >[!NOTE]
  >
  >    반복에는 기존 댓글 달기 환경이 계속 유지됩니다. 새 주석 달기 경험을 반복할 수 없습니다.

## 릴리스된 기능

다음 섹션에는 원래 23.2 릴리스 이후 가장 최근에 릴리스된 기능부터 추가된 기능 목록이 포함되어 있습니다.

다음 정보는 새 댓글 달기 Beta 경험에 포함된 기능을 기반으로 매주 릴리스 활동을 참조합니다. 이 문서에는 새로운 댓글 달기 환경에 대해 추가된 새로운 기능과 해결된 문제가 나열되어 있습니다.

### 2023년 9월 11일 주

#### 새로운 댓글 달기 환경은 2019년 1월 1일부터 정보를 캡처합니다

현재 프로젝트, 작업, 문제 및 문서에는 2019년 1월 1일부터 업데이트가 표시됩니다. 이 개선 이전에는 새로운 댓글 달기 환경에서 2022년 6월 이러한 오브젝트에 대한 업데이트만 캡처했습니다.

자세한 내용은 [새 댓글 달기 환경](../new-commenting-experience-beta/unified-commenting-experience.md).

모든 고객을 위한 미리 보기 및 프로덕션: 2023년 9월 11일.

### 2023년 8월 21일 주

#### 댓글 탭에서 타임스탬프 형식 변경

새 댓글 스트림의 댓글 탭에서 사용자 댓글의 타임스탬프 형식을 업데이트했습니다. 이 변경 사항의 일부로, 현재 연도의 주석은 더 이상 타임스탬프에 연도를 표시하지 않습니다. 타임스탬프를 마우스로 가리키면 연도를 포함한 전체 날짜가 표시됩니다.

시스템 활동 탭의 시스템 업데이트에는 변경 사항이 적용되지 않습니다.

모든 고객을 위한 미리보기 및 프로덕션: 2023년 8월 24일

### 2023년 8월 14일 주

[2023년 8월 14일이 있는 주에 릴리스된 모든 기능에 대한 비디오 데모를 확인하십시오](https://video.tv.adobe.com/v/3422912/){target=_blank}

#### 추가 오브젝트에 대한 새로운 댓글 달기 환경

[!BADGE Fast Release를 위한 프로덕션]{type=Positive}

새로운 주석 달기 환경은 23.3 프로덕션 릴리스 직후 다음 오브젝트(템플릿 작업, 템플릿, 타임시트, 팀, 사용자, 프로그램, 포트폴리오)에 대해 사용할 수 있습니다.

이러한 오브젝트에 액세스할 때 기존 댓글 달기 경험이 제거되므로 이 환경은 유일한 댓글 달기 경험이 됩니다.

자세한 내용은 [새 댓글 달기 환경](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

미리보기 릴리스: 2023년 8월 17일

빠른 릴리스를 위한 프로덕션 릴리스: 23.8 릴리스 포함(2023년 8월 31일)

모든 고객을 위한 프로덕션 릴리스: 23.10 릴리스 포함(2023년 10월)

#### 새 댓글 스트림에 대한 새 디자인 업데이트

[!BADGE Fast Release를 위한 프로덕션]{type=Positive}

새로운 주석 처리 스트림을 재설계하여 보다 업데이트된 디자인을 제공했습니다. 몇 가지 개선 사항은 다음과 같습니다.

* 주석 스트림의 콘텐츠는 페이지의 전체 너비를 차지하지 않고 페이지 중앙에 있습니다.

* 기타 메뉴 아이콘은 좋아요 단추 옆에 있지 않고 댓글의 오른쪽 상단 모서리에 재배치됩니다.

* 이제 [좋아요] 및 [회신] 단추가 서로 옆에 있습니다.

* 로그 시간 단추가 댓글 달기 영역의 오른쪽 위 모서리에 재배치되었습니다.

* 기존 회신에 회신을 추가할 것인지 묻는 메시지를 표시하기 위해 회신 추가 프롬프트가 추가되었습니다.

* 각 주석 스레드 사이에는 분리 선이 있습니다

자세한 내용은 [업데이트 탭 개요](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

미리보기 릴리스: 2023년 8월 17일

빠른 릴리스를 위한 프로덕션: 23.8 릴리스 포함(2023년 8월 31일)

분기별 릴리스 프로덕션: 23.10 릴리스 포함(2023년 10월)

#### 새 댓글 달기 환경은 프로젝트, 작업, 문제 및 문서에 대한 기본 경험입니다

[!BADGE Fast Release를 위한 프로덕션]{type=Positive}

새 댓글 달기 경험을 프로젝트, 작업, 문제 및 문서 개체에 대한 기본 경험으로 만들고 있습니다.  이러한 오브젝트에 액세스할 때 기존 댓글 달기 경험이 대체 옵션으로 유지됩니다.

이 변경 사항을 지원하기 위해 &quot;댓글 달기 Beta&quot; 토글을 &quot;새 댓글 달기&quot;로 변경했습니다.

자세한 내용은 [새 댓글 달기 환경](../new-commenting-experience-beta/unified-commenting-experience.md).

미리보기 릴리스: 2023년 8월 17일

빠른 릴리스를 위한 프로덕션: 23.8 릴리스 포함(2023년 8월 31일)

분기별 릴리스 프로덕션: 23.10 릴리스 포함(2023년 10월)

#### 업데이트에서 사용자를 태그 지정할 때 아바타 개선

업데이트에서 태그가 지정된 사용자를 더 잘 보이도록 하기 위해, 이제 업데이트에서 태그가 지정된 사용자(최대 2명의 사용자)의 이름이 표시됩니다. 자세한 내용은 [업데이트의 다른 사용자에게 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

미리보기 릴리스: 2023년 8월 17일

빠른 릴리스를 위한 프로덕션: 23.8 릴리스 포함(2023년 8월 31일)

모든 고객을 위한 프로덕션: 23.10 릴리스 포함(2023년 10월)

### 2023년 8월 7일 주

#### 업데이트에 이모지 추가

이제 새 댓글 달기 환경에서 서식 있는 텍스트 도구 모음 옵션을 사용하여 댓글에 이모지를 추가할 수 있습니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 설명서는 릴리스 시점에 업데이트됩니다.

미리보기 및 프로덕션: 2023년 8월 10일

### 2023년 7월 10일 주

#### 모든 스레드 참가자에 자동으로 태그 지정

이제 댓글 소유자에 스레드에서 자동으로 태그가 지정됩니다. 이 업데이트 이전에는 &quot;@name&quot; 태그를 사용하거나 태그가 지정된 사용자 목록에 표시되는 &quot;사람 또는 팀 태그 지정&quot; 섹션에 추가하여 태그가 지정된 사용자만 볼 수 있었습니다. 이제 필요한 경우 이전에 수동으로 태그가 지정되지 않은 경우에도 스레드에서 주석 소유자를 제거할 수 있습니다.

미리보기 릴리스: 2023년 7월 12일

프로덕션 릴리스: 2023년 7월 13일

### 2023년 7월 3일 주

#### 시간 기록을 위한 새로운 인터페이스

새 댓글 달기 환경의 업데이트 영역에서 시간을 기록하기 위한 인터페이스를 다시 설계했습니다.

자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md).

미리보기 릴리스: 2023년 7월 5일

프로덕션 릴리스: 23.3 릴리스 포함(2023년 7월)

### 2023년 6월 26일 주

#### 새 회신에서 댓글 내용 인용

이제 새로운 댓글 달기 경험을 사용할 때 동일한 스레드에서 댓글 콘텐츠를 복사하고 회신에 새 인용구로 추가할 수 있습니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

미리 보기: 2023년 6월 28일

프로덕션 릴리스: 2023년 6월 29일

### 2023년 6월 12일 주

#### 보드 영역의 카드에 대한 새로운 댓글 달기 경험

이제 보드 영역의 카드에 새 댓글 달기 환경을 사용할 수 있습니다. 이 경험은 카드에 사용할 수 있는 유일한 경험입니다. 자세한 내용은 [23.3 릴리스 개요](../../product-releases/23.3-release-activity/23-3-release-overview.md).

미리 보기: 2023년 6월 15일

조기 옵트인을 위한 프로덕션 릴리스: 2023년 6월 22일

모든 고객을 위한 프로덕션: 23.3 릴리스 포함(2023년 7월)

#### 댓글에 블록 따옴표 추가

이제 새로운 댓글 달기 Beta 경험에서 서식 있는 텍스트 도구 모음 옵션을 사용하여 댓글에 블록 따옴표를 추가할 수 있습니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

미리 보기: 2023년 6월 14일

프로덕션: 2023년 6월 15일

#### 댓글 편집 시 향상된 경험

이제 주석을 편집할 때 다음 단축키를 사용할 수 있습니다.

* CTRL+Z (Mac의 경우 CMD+Z) 를 클릭하여 변경 내용을 실행 취소합니다

* CTRL+Y(Mac의 경우 CMD+Y) 를 눌러 변경 사항을 재실행합니다

이러한 개선 사항 이전에는 주석을 편집하는 동안 변경 사항을 실행 취소하거나 다시 실행할 수 없었습니다. 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

미리 보기: 2023년 6월 13일

프로덕션: 2023년 6월 13일

<!--I used the date when I found them in Prod. Not sure when these released, but it could have been before this date-->

### 2023년 5월 29일 주

#### 프로젝트, 작업 및 문서에 대한 새로운 댓글 달기 Beta 경험

이제 프로젝트, 작업 및 문서에 새 댓글 달기 Beta 환경을 사용할 수 있습니다. 이 업데이트 이전에는 댓글 달기 Beta 경험을 문제 및 목표에 대해서만 사용할 수 있었습니다.

미리 보기: 2023년 6월 1일

프로덕션: 23.3 릴리스(2023년 7월) 포함

>[!NOTE]
>
>2023년 6월 1일부터 새로운 댓글 달기 Beta 경험에 릴리스된 모든 기능은 프로덕션 23.3 릴리스 이후 프로젝트, 작업 및 문서에 대한 프로덕션에서 사용할 수 있습니다. 자세한 내용은 [23.3 릴리스 개요](../../../product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

#### 댓글을 편집한 후 &quot;편집된&quot; 태그의 새로운 모양과 느낌

새 댓글 달기 Beta 경험에서 댓글을 편집할 때 &quot;편집됨&quot; 태그가 댓글에 추가됩니다. 이제 이 태그는 원래 릴리스된 태그와 다른 새로운 모양과 느낌을 갖게 되었습니다. 주석의 날짜 및 타임스탬프는 원래 주석의 타임스탬프 및 타임스탬프입니다. 편집이 이루어진 날짜와 타임스탬프가 아닙니다.  자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

미리 보기: 2023년 5월 31일

프로덕션: 2023년 6월 1일

#### 하위 객체의 주석이 상위 객체로 롤업됩니다.

댓글 달기 Beta 경험을 활성화하면 이제 하위 객체와 연관된 댓글이 상위 객체로 롤업됩니다. 예를 들어 이제 문서의 주석이 문서가 첨부된 문제에 표시됩니다. 자세한 내용은 [업데이트 섹션 개요](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

미리 보기: 2023년 6월 1일

프로덕션: 2023년 6월 1일

#### 새 댓글 달기 Beta 경험에 시간 기록

새로운 댓글 달기 Beta 환경을 사용할 때 업데이트 영역에서 문제, 작업 및 프로젝트에 대한 시간을 기록할 수 있습니다. 자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md).

미리 보기: 2023년 6월 1일

프로덕션: 23.3 릴리스(2023년 7월) 포함

### 2023년 5월 15일 주

#### 댓글에 하이퍼링크를 추가할 때의 경험 개선

이제 다음 바로 가기 키를 사용하여 댓글에 하이퍼링크를 추가할 수 있습니다.

* CTRL+V(Mac의 경우 CMD+V)를 누르면 링크가 선택한 텍스트 위에 붙여넣습니다.
* CTRL + K (Mac의 경우 CMD + K)를 누르면 링크 추가 상자가 열립니다.

이러한 개선 사항 이전에는 리치 텍스트 도구 모음에서 링크 아이콘을 클릭해야만 하이퍼링크를 추가할 수 있었습니다. 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

미리 보기: 2023년 5월 17일

프로덕션: 2023년 5월 18일

### 2023년 5월 1일 주

#### 첨부 파일을 주석에서 제거하거나 첨부 파일이 포함된 주석을 제거하면 문서 영역에서 이미지가 제거됩니다

첨부 파일이 포함된 주석을 제거하거나 편집할 때 첨부 파일이 작동하는 방식을 변경하고 있습니다. 이제 주석을 편집하고 첨부 파일을 제거할 때 또는 첨부 파일이 포함된 주석을 삭제할 때 문서 영역에서도 첨부 파일이 제거됩니다. 이 변경 이전에는 이전 댓글 달기 환경에서 첨부 파일이 문서 영역에 남아 있었습니다. 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Beta 경험에 대한 댓글을 달거나 다음 날짜에 기본적으로 Workfront 목표에 사용할 수 있습니다.

* 미리보기 및 프로덕션: 2023년 5월 4일


### 2023년 4월 27일

베타 문제를 댓글로 달고 목표에 대해 다음 유지 보수 업데이트가 릴리스되었습니다.

댓글 수정 시 첨부된 이미지 수정. 자세한 내용은 이 문서의 &quot;4월 27일 유지 보수 업데이트&quot; 섹션을 참조하십시오 <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">2023년 4월 업데이트</a>.

### 2023년 4월 20일

베타 문제를 댓글로 달고 목표에 대해 다음 유지 보수 업데이트가 릴리스되었습니다.

댓글 달기 Beta 경험의 목표 및 문제에 대한 업데이트에서 이동할 때 이미지를 초안으로 유지. 자세한 내용은 이 문서의 &quot;4월 20일 유지 보수 업데이트&quot; 섹션을 참조하십시오 <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">2023년 4월 업데이트</a>.

### 2023년 4월 17일

베타 문제를 댓글로 달고 목표에 대해 다음 유지 보수 업데이트가 릴리스되었습니다.

문제의 업데이트 섹션(새로운 댓글 달기 Beta 경험)과 목표에서 보이는 화면 영역 외부에 새 댓글이 표시됨. 자세한 내용은 이 문서의 &quot;4월 17일 유지 보수 업데이트&quot; 섹션을 참조하십시오  <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">2023년 4월 업데이트</a>.


### 2023년 4월 6일 주

문제에 대한 새 댓글 달기 Beta 경험이 시작되었습니다.
Workfront 개체의 댓글 달기 베타에 대해 릴리스된 동일한 기능은 Workfront 목표에 액세스할 수 있는 모든 사용자의 목표에 대해 동시에 릴리스됩니다. 자세한 내용은 [23.2 릴리스 개요](../../product-releases/23.2-release-activity/23-2-release-overview.md).
