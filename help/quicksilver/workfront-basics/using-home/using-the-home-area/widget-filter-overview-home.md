---
product-area: home
navigation-topic: new-home
title: 홈 위젯 필터 개요
description: 다양한 위젯 중에서 선택하여 홈 페이지에 표시되는 콘텐츠를 맞춤화할 수 있습니다. 홈 페이지에서 이러한 위젯의 크기를 조정하고 정렬할 수 있습니다.
author: Courtney
feature: Get Started with Workfront
exl-id: 58f79e81-df6b-456f-9e91-4e00a1c2a8a2
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 11%

---

# 홈 위젯 필터 개요

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>을 참조하세요.

다음 위젯에서 필터를 사용하여 작업을 찾고 구성할 수 있습니다.

* [내 프로젝트](#my-projects)
* [내 작업](#my-tasks)
* [내 문제](#my-issues)
* [내 요청](#my-requests)
* [내 작업](#my-work)
* [내 승인](#my-approvals)

>[!IMPORTANT]
>
>* 홈 위젯에서 작업 및 문제를 표시하려면 상위 프로젝트가 현재 상태 또는 현재 상태와 동등한 상태여야 합니다.
>* 프로젝트가 또한 현재 상태 또는 현재 상태와 동등한 상태여야 표시합니다.

## 내 프로젝트

내 프로젝트 위젯에서 다음 필터를 사용할 수 있습니다.

<table>
  <tr>
    <td>활성</td>
    <td>프로젝트를 현재, 계획 및 승인됨 상태로 표시합니다. </td>
  </tr>
  <tr>
    <td>위험 상태</td>
    <td>위험 상태의 프로젝트 표시 </td>
  </tr>
  <tr>
    <td>지연됨</td>
    <td>프로젝트가 지연된 상태로 표시됩니다.</td>
  </tr>
  <tr>
    <td>현재</td>
    <td>현재 상태의 프로젝트 표시 </td>
  </tr>
  <tr>
    <td>기한: 이번 달</td>
    <td>현재 달력에 계획된 완료 일자가 있는 프로젝트를 표시합니다.</td>
  </tr>
  <tr>
    <td>지연</td>
    <td>프로젝트가 지연 상태로 표시됨</td>
  </tr>
  <tr>
    <td>내 프로젝트</td>
    <td>나 또는 내 프로젝트 팀에 할당된 프로젝트를 현재 상태로 표시합니다.</td>
  </tr>
  <tr>
    <td>정시</td>
    <td>정시 상태로 프로젝트 표시</td>
  </tr>
  <tr>
    <td>비용 예산 초과</td>
    <td>실제 비용 값이 계획된 비용 값보다 큰 프로젝트를 표시합니다.</td>
  </tr>
  <tr>
    <td>작업 예산 초과</td>
    <td>실제 작업 필요 값이 작업 필요 값보다 큰 프로젝트를 표시합니다.</td>
  </tr>
  <tr>
    <td>대기열만</td>
    <td>요청 대기열로 지정된 프로젝트를 표시합니다.</td>
  </tr>
  <tr>
    <td>요청됨</td>
    <td>요청된 상태의 프로젝트 표시</td>
  </tr>
  <tr>
    <td>시나리오 플래너 프로젝트</td>
    <td>시나리오 플래너를 통해 이니셔티브 ID가 설정된 프로젝트를 표시합니다.</td>
  </tr>
</table>

## 내 작업

내 작업 위젯에서 다음 필터를 사용할 수 있습니다.

<table>
  <tr>
    <td>활성 작업</td>
    <td><p>전달 일자 또는 전달 일자가 오늘이거나 이전인 작업을 표시합니다.</p>
<ul>
  <li>완료율이 100%보다 작음</li>
  <li>시작 가능 값이 True로 설정되어 있습니다.</li>
</ul>
</td>
  </tr>
   <!-- <tr>
    <td>All Unassigned Tasks</td>
    <td></td>
  </tr> -->
  <tr>
    <td>승인 작업</td>
    <td>승인 보류 중 상태의 작업 표시</td>
  </tr>
  <tr>
    <td>시작 가능</td>
    <td><p>나에게 할당된 작업 표시</p>
<ul>
  <li>완료 상태가 아닙니다.</li>
  <li>true인 시작 가능 값이 있어야 합니다.</li>
</ul>
</td>
  </tr>
  <tr>
    <td>중요 경로</td>
    <td>위험 작업으로 지정된 작업 표시</td>
  </tr>
  <tr>
    <td>미완료 작업</td>
    <td>상태가 완료를 제외한 다른 항목으로 설정된 작업을 표시합니다.</td>
  </tr>
  <tr>
    <td>마일스톤 작업</td>
    <td>이정표와 연관된 작업을 표시합니다. 자세한 내용은 <a href="/help/quicksilver/manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">작업과 마일스톤 연결</a>을 참조하세요.
</td>
  </tr>
  <tr>
    <td>내 프로젝트 작업</td>
    <td>내가 프로젝트 팀의 멤버인 현재 상태의 작업을 표시합니다 </td>
  </tr>
    <tr>
    <td>내 작업</td>
    <td>나에게 할당된 작업 표시</td>
  </tr>
  <tr>
    <td>반복에 할당되지 않음</td>
    <td>반복에 할당되지 않은 작업 표시</td>
  </tr>
  <tr>
    <td>최근에 관심을 가진 항목</td>
    <td><p>최근 업데이트가 지난 2주 이내에 있었던 작업과</p>
<ul>
  <li>커밋 일자는 계획된 완료 일자보다 이후입니다.</li>
  또는
  <li>프로젝트 기간이 계획된 기간보다 큽니다.</li>
  또는
  <li>상태는 순조롭게 진행되고 있거나 약간의 우려가 있습니다</li>
  또는
  <li>기본 작업 할당자가 작업 작업을 시작했습니다.</li>
</ul>
</td>
  </tr>
  <tr>
    <td>내 역할의 할당 해제된 작업</td>
    <td><p>다음 작업을 표시합니다.</p>
<ul>
  <li>내 역할에 할당됨</li>
  <li>완료 안 됨</li>
</ul>
</td>
  </tr>
  <tr>
    <td>예정된 작업</td>
    <td><p>다음 작업을 표시합니다.</p>
<ul>
  <li>완료되지 않음</li>
  <li>현재 상태의 프로젝트에 속함</li>
  <li>오늘 날짜로부터 2주 이내에 계획된 시작 일자가 있어야 합니다.</li>
</ul>
</td>
  </tr>
</table>

## 내 문제

내 문제 위젯에서 다음 필터를 사용할 수 있습니다.

<table>
<tr>
    <td>모두 할당 해제됨</td>
    <td>미할당되고 해결 오브젝트가 첨부되지 않은 모든 문제를 표시합니다. </td>
  </tr>
  <tr>
    <td>나에게 할당됨</td>
    <td>내가 기본 피할당자인 문제를 표시합니다.</td>
  </tr>
  <tr>
    <td>완료</td>
    <td>완료 일자 관련 문제 표시 </td>
  </tr>
  <tr>
    <td>내가 입력한 항목</td>
    <td>내가 입력한 문제 표시</td>
  </tr>
  <tr>
    <td>내 프로젝트 문제</td>
    <td><p>다음의 문제를 표시합니다.</p>
<ul>
  <li>내가 기본 피할당자입니다.</li>
  <li>상태가 완료되지 않았습니다.</li>
  <li>연결된 해결 개체가 없습니다.</li>
</ul>
</td>
  </tr>
    <tr>
    <td>최근에 제출된 문제</td>
    <td><p>다음과 같은 문제 표시</p>
<ul>
  <li>제출함</li>
  <li>연결된 해결 개체가 없습니다.</li>
  <li>상태가 완료됨이 아니고 완료 일자가 없습니다.</li>
  <li>이(가) 오늘 날짜로부터 3개월 이내에 제출되었습니다.</li>
</ul>
</td>
  </tr>
    </tr>
    <tr>
    <td>내가 제출한 문제</td>
    <td>내가 소유한 문제 표시</td>
  </tr>
  <tr>
    <td>열기</td>
    <td>완료 일자가 없는 문제를 표시합니다.</td>
  </tr>
  <tr>
    <td>해결 가능</td>
    <td>해결 중인 오브젝트가 첨부된 문제를 표시합니다.</td>
  </tr>
  <tr>
    <td>내 역할에 할당되지 않음</td>
    <td>할당된 기본 사용자가 없지만 할당된 역할이 있는 모든 문제를 표시합니다. </td>
  </tr>
</table>

## 내 요청

프로덕션 환경에서:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두</td> 
      <td>상태 또는 요청 제출자에 관계없이 제출된 모든 요청을 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">열기</td> 
      <td> <p>제출된 모든 요청 표시 
      <ul>
      <li>누가 제출했는지에 상관없이 현재 열려 있습니다. 직접 제출하지 않은 경우 적어도 볼 수 있는 권한이 있는 요청만 여기에 표시됩니다.</li>
      <li>실제 완료 일자가 없거나 해결 객체에 실제 완료 일자가 없는 경우 열기 하위 탭에 나열됩니다.</li> 
      </ul>
      <p><b>참고</b> 
      Closed와 동일하지 않은 모든 상태에 있는 요청은 Open으로 간주됩니다.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 요청</td> 
      <td>상태에 관계없이 제출한 요청을 표시합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 진행 중 요청</td> 
      <td> <p>요청 표시 
      <ul>
      <li>을(를) 제출했으며 아직 열려 있습니다. </li> 
      <li>실제 완료 일자가 없거나 해결 객체에 실제 완료 일자가 없는 경우 [내 진행 요청] 하위 탭에 나열됩니다.  </li> 
      </ul>
      <p><b>참고</b> 
      Closed와 동등한 상태가 아닌 요청은 Open으로 간주됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<div class="preview">

미리보기 환경에서:

내 요청 위젯에는 사용자 정의 가능한 필터가 있어 위젯에 표시되는 요청을 제어할 수 있습니다. 다양한 필드 및 값에 대해 이 필터를 구성하고 AND 및 OR를 사용하여 조건을 스택할 수 있습니다.

내 요청 위젯에서 필터를 구성하는 방법에 대한 지침은 내 요청 위젯 사용 문서에서 [필터 요청](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md#filter-requests)을 참조하십시오.

</div>

## 내 작업

내 작업 위젯에서 다음 필터를 사용할 수 있습니다.

<table>
  <tbody>
    <tr>
      <td>작업 중</td>
      <td>현재 작업 중인 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>시작 준비 완료</td>
      <td>항목이 있는 항목 표시 
      <ul>
      <li>완료되지 않은 전임 작업 또는 작업 제한 없음</li>
      <li>계획된 시작 일자가 과거 또는 최대 2주 미래입니다.</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>준비 안 됨</td>
      <td>다음과 같은 항목이 있는 항목 표시
       <ul>
      <li>항목이 작업되지 않도록 하는 불완전한 전임 작업 또는 작업 제한</li>
      또는
      <li>2주 이상 후의 계획된 시작 일자</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>요청됨</td>
      <td>작업을 시작하지 않은 문제를 표시합니다.</td>
    </tr>
    <tr>
      <td>내가 위임함</td>
      <td>다른 사용자에게 위임한 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>내게 위임함</td>
      <td>사용자가 귀하에게 위임한 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>완료됨</td>
      <td>지난 2주 이내에 완료된 작업을 표시합니다. 이 필터 옵션에는 승인이 포함되지 않습니다.</td>
    </tr>
  </tbody>
</table>

## 내 승인

내 승인 위젯에서 다음 필터를 사용할 수 있습니다.

<table>
  <tbody>
    <tr>
      <td>위임된 승인</td>
      <td>내게 위임된 승인을 표시합니다.</td>
    </tr>
    <tr>
      <td>내 승인</td>
      <td>승인이 필요한 항목을 표시합니다.
      </td>
    </tr>
    <tr>
      <td>내가 제출한 승인</td>
      <td>승인을 위해 제출한 항목을 표시합니다.
       </td>
    </tr>
  </tbody>
</table>
