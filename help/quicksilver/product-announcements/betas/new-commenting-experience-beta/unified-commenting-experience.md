---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: 새 댓글 달기 환경
description: Adobe Workfront의 댓글 달기 환경에 대한 업데이트가 현재 개발 중입니다. 이 업데이트에는 선택한 객체의 업데이트 섹션에 새로운 인터페이스, 새로운 기능 및 향상된 성능이 포함되어 있습니다.
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 2%

---

# 새 댓글 달기 환경

<!--take out legacy, preview, prod references from below-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.  </span>  

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>이 문서의 정보는 새로운 댓글 달기 환경에 릴리스된 기능을 참조합니다.
>
>새로운 댓글 달기 경험을 위한 베타 프로그램은 2023년 4월에 시작하여 2023년 10월에 종료되었습니다. 새로운 댓글 달기 경험을 위한 베타 프로그램은 2023년 10월 릴리스로 종료되었습니다.
>
>2023년 10월부터 새로운 댓글 달기 경험을 위한 모든 새로운 기능이 모든 고객에게 릴리스됩니다. 자세한 내용은 각 릴리스의 현재 릴리스 개요 페이지를 참조하십시오.

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## 기능

새 댓글 달기 경험에는 Adobe Workfront 개체의 업데이트 섹션에 대한 개선 사항 및 변경 사항이 포함되어 있습니다.

새 댓글 달기 환경에 포함된 개선 사항 중 하나는 다음과 같습니다.

* 향상된 성능 및 사용자 경험
* 시스템 활동 업데이트에서 사용자 주석 분리
* 오브젝트에 새 댓글이 추가될 때 실시간 표시기
* 의견 제출 후 편집

다음 기능은 제거되었거나 새 경험에서 더 이상 사용되지 않습니다.

* 시스템 업데이트에 대한 주석 달기
* 작업 및 문제에 대해 댓글을 작성하는 동안 상태, 조건, 커밋 일자 및 완료율을 편집할 수 있습니다.
* 사용자 정의 양식 편집
* Workfront 또는 그룹 관리자가 다른 사용자로 로그인하고 대신 주석을 추가할 때의 &quot;대신하여 &lt; 사용자 이름 >&quot; 정보는 원래 제거되었습니다. 2023년 10월 19일에 복원되었습니다.
* 문서에 주석을 추가하는 동안 다른 사용자에게 태그를 지정할 때 &quot;승인 요청&quot; 옵션이 표시됩니다.
* 사용자의 프로필 상자를 편집할 때 &quot;업데이트 상태에서 완료율 표시&quot; 설정이 제거됩니다. 작업 또는 문제의 완료율을 업데이트하는 기능이 제거되었습니다.
* 작업 또는 문제의 할당자가 커밋 일자를 편집했다는 업데이트 영역의 프로젝트 소유자에 대한 알림입니다. <!--ensure this is correct when re remove the legacy and leave only new commenting-->

<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

다음 표는 새 댓글 달기 환경에서 사용할 수 있는 기능과 지원되는 영역에서 사용할 수 있는 기능을 보여 줍니다.

<table>
  <tr>
   <td><strong>기능 </strong>
   </td>
   <td><strong>이전 댓글 환경에 있음 </strong>
   </td>
   <td><strong>새 댓글 달기 환경에 있음 </strong>
   </td>
   <td><strong>새로운 댓글 달기 환경에 도입될 예정입니다. </strong>
   </td>
   <td><strong>새로운 댓글 달기 환경에 도입될 시기 </strong>
   </td>
   <td><strong>연구 중 </strong>
   </td>
  </tr>
  <tr>
   <td>댓글 만들기/읽기/회신/삭제 
   </td>
   <td>✓ 덧신 
  </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>리치 텍스트(인용 및 이모지 제외)
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>리치 텍스트(이모티콘)
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>리치 텍스트(블록 인용)
   </td>
   <td>✓ 덧신 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td> 2023년 2분기
   </td>
   <td> 
   </td>
  </tr>
  <tr>
<tr>
   <td> 견적 주석
   </td>
   <td>✓ 덧신 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td> 2023년 2분기
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>댓글에 반응(예: 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>댓글에 이미지 첨부 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>댓글에 직원 태그 지정 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>스레드 참가자 제거
   </td>
   <td> 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>


<tr>
   <td>모든 스레드 참가자에 자동으로 태그 지정
   </td>
   <td> 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>회사에 비공개인 댓글 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>댓글 게시 취소 
   </td>
   <td>✓ 덧신 
   </td>
   <td>댓글 편집으로 대체됨 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>시스템 업데이트 끄기 
   </td>
   <td>✓ 덧신 
   </td>
   <td>활동 탭으로 대체됨 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>댓글 편집 
   </td>
   <td> 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>페이지에서 이동할 때 주석 초안 저장 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>새 댓글을 실시간으로 확인(댓글 삭제 시 확인 포함)
   </td>
   <td> 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>로그 시간 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>스레드 링크 복사 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 복사 링크로 대체됨
   </td>
   <td> 
   </td>
   <td>2023년 2분기 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>주석 링크 복사 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 복사 링크로 대체됨
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>견적 주석 텍스트 
   </td>
   <td>✓ 덧신 
   </td>
   <td>✓ 덧신
   </td>
   <td> 
   </td>
   <td>2023년 2분기 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>본문 복사 
   </td>
   <td>✓ 덧신 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>댓글에서 검색 
   </td>
   <td> 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td>2024년 1분기 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>댓글에 이미지 복사 및 붙여넣기
   </td>
   <td> 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td>2024년 1분기 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>댓글에 이미지 드래그 앤 드롭
   </td>
   <td> ✓ 덧신
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td>2024년 1분기 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>사용자 정의 양식 편집 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>댓글을 달면서 상태, 조건, 커밋 일자를 편집할 수 있는 기능 
   </td>
   <td>✓ 덧신 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>시스템 업데이트에 대한 회신 
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>다른 사용자로 로그인한 댓글을 추가할 때 "대신" 표시
   </td>
   <td> ✓ 덧신
   </td>
   <td> ✓ 덧신
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
</table>

## 릴리스 타임라인

>[!IMPORTANT]
>
>Beta 기간 동안 새로운 댓글 달기 경험에 릴리스된 기능에 대한 자세한 내용은 [새로운 댓글 달기 Beta 경험 릴리스 활동](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Workfront 개체의 업데이트 관리에 대한 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


다음은 프로덕션 환경에 대한 새로운 댓글 달기 환경의 릴리스에 대한 주요 이정표가 포함된 계획된 타임라인입니다. 아래 이정표 외에도, 더 작은 개선 사항으로 주석 달기 환경을 계속 개선해 나갈 것입니다.

Beta 기간이 종료된 후 새 주석 달기 경험을 위해 릴리스된 기능에 대한 자세한 내용은 현재 릴리스 개요 페이지를 참조하십시오.

다음은 새로운 댓글 달기 환경의 릴리스에 대해 계획된 타임라인입니다.

* 23.2 릴리스(2023년 4월 6일):
   * 문제에 대한 댓글 달기 경험 베타 시작
   * 목표에 대한 새 댓글 달기 경험 릴리스(유일한 경험으로)
* 23.3 릴리스(2023년 7월 20일):
   * 프로젝트, 작업 및 문서에 대한 댓글 달기 경험 Beta를 시작합니다.
   * 보드 영역에서 카드에 대한 새 댓글 달기 경험을 해제합니다(유일한 경험으로).
* 2023년 4분기 릴리스(제한된 릴리스, 빠른 릴리스를 선택하는 고객만 사용 가능) 중:
   * 템플릿, 템플릿 작업, 프로그램, 포트폴리오, 팀, 사용자 및 타임시트에 대한 새로운 댓글 달기 환경(유일한 경험으로) 릴리스
   * 프로젝트, 작업, 문제 및 문서에 대한 댓글 달기 경험 Beta를 업데이트하여 기본 옵션으로 설정합니다. Beta 레이블이 제거됩니다.
* 2023년 4분기(23.10) 릴리스 포함(2023년 10월 26일)
   * 모든 고객에게 템플릿, 템플릿 작업, 프로그램, 포트폴리오, 팀, 사용자 및 타임시트에 대한 새로운 댓글 달기 환경(유일한 경험으로)을 릴리스합니다.
   * 프로젝트, 작업, 문제 및 문서에 대한 새로운 댓글 달기 환경을 기본 옵션으로 설정합니다.

  >[!IMPORTANT]
  >
  >    이렇게 하면 새 댓글 달기 환경의 베타 단계가 종료됩니다.

   * 현재 정기 월별 및 분기별 릴리스의 이 날짜 부분부터 새로운 댓글 달기 경험을 위해 릴리스된 모든 기능을 사용할 수 있습니다.
* 2023년 말:
   * 프로젝트, 작업, 문제 및 문서 개체에 대한 보조 옵션으로 기존 주석 달기 환경을 유지합니다. 새 댓글 달기 환경은 이러한 오브젝트의 모든 사용자에 대한 기본 옵션입니다.
   * 새 댓글 달기 경험을 다른 모든 오브젝트에 대한 유일한 경험으로 만듭니다.

  >[!NOTE]
  >
  >    반복에는 기존 댓글 달기 환경이 계속 유지됩니다. 새 주석 달기 경험을 반복할 수 없습니다.

* 2024년 2분기(2024년 4월):

   * 기존 댓글 달기 스트림으로 다시 전환하고 새 댓글 달기 스트림을 반복을 제외하고 모든 개체에 대한 유일한 경험으로 만드는 옵션을 제거합니다.

## 새 댓글 달기 환경 찾기

&lt;!—중요: 기존 경험을 제거할 때 이 의 버전을 업데이트 작업 문서 또는 업데이트 섹션 개요로 이동하여 경험이 반복을 제외한 모든 작업에 대해 다르다고 설명하십시오—>

새로운 댓글 달기 환경은 현재 모든 고객 및 모든 환경에서 사용할 수 있습니다.

댓글 달기 경험에 액세스하는 객체에 따라 업데이트 섹션에 다음과 같은 기능이 표시될 수 있습니다.

* 다음 개체에 대한 새 댓글 및 이전 댓글 사용 환경:

   * 프로젝트
   * 작업(스토리 포함)
   * 문제
   * 문서

  >[!TIP]
  >
  >새 주석 달기 옵션을 사용하여 이 섹션에 설명된 대로 새 주석 달기 경험(활성화할 경우) 또는 기존 주석 달기 경험(비활성화할 경우)을 표시합니다. 새 댓글 달기 환경이 기본값입니다.

   * 아래 나열된 객체에 대한 새 댓글 달기 경험만 해당됩니다. 다음 객체에 대한 기존 댓글 달기 환경을 활성화하는 옵션은 없습니다.

      * 목표

     >[!NOTE]
     >
     >이 Workfront 영역에 액세스하려면 Adobe Workfront 목표에 대한 추가 라이선스가 있어야 합니다. 자세한 내용은 [Workfront 목표 사용 요구 사항](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
      * 보드에 있는 카드
      * 팀
      * 템플릿
      * 템플릿 작업
      * 타임시트
      * 프로그램
      * 포트폴리오
      * 사용자

* 다음 개체에 대한 레거시 댓글 달기 환경만 해당:

   * 반복

     반복에 대한 새 주석 달기 경험을 활성화하는 옵션은 없습니다. 반복에는 기존 주석 달기 경험만 사용할 수 있습니다.


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

프로젝트, 작업, 문제 및 문서에 대해 주석 달기 경험 옵션을 활성화하려면 다음을 수행하십시오.

1. 새 댓글 달기 경험을 활성화할 개체로 이동한 다음, **업데이트** 왼쪽 패널에서
1. (조건부) 비활성화되어 있다면 **새 댓글 달기** 업데이트 영역의 오른쪽 위 모서리에 있는 옵션을 활성화하십시오. 이 기능은 기본적으로 활성화되어 있어야 합니다.

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. 에서 업데이트를 입력하십시오. **댓글** 탭. 새 경험이 열릴 때 주석 탭이 기본 탭입니다

   또는

   다음을 클릭합니다.  **시스템 활동** 탭으로 이동하여 Workfront에서 생성한 활동 업데이트를 봅니다.

1. (선택 사항) 새 댓글 달기 경험을 비활성화하고 기존 댓글 달기로 돌아가려면 **새 댓글 달기** 옵션을 선택합니다.

