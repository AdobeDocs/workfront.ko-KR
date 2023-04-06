---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 16의 새로운 기능
description: Adobe Workfront은 2022년 4월 6일에 API 버전 16을 릴리스했습니다. API 버전 16은 버전 15에서 다음과 같은 변경 사항을 제공합니다.
author: Becky
feature: Workfront API
source-git-commit: 19978aaa2886008afc3c0faa9cfd18bd7c4b2555
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# API 버전 16의 새로운 기능

Adobe Workfront은 2022년 4월 6일에 API 버전 16을 릴리스했습니다. API 버전 16은 버전 15에서 다음과 같은 변경 사항을 제공합니다.

## 리소스를 추가했습니다.

API 버전 16에 대한 리소스가 추가되지 않았습니다.

## 제거된 리소스

API 버전 16에 대해 제거된 리소스가 없습니다

## 수정된 리소스

* <!--[AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [승인(승인)](#approval-approval)
* [고객 기본 설정(CUSTOMER)](#customerpreferences-custpr)
* [외부 섹션(EXTSEC)](#externalsection-extsec)
* [시간(시간)](#hour-hour)
* [레이아웃 템플릿(UITMPL)](#layouttemplate-uitmpl)
* [참고(참고)](#note-note)
* [OpTask/Issue(OPTASK)](#note-note)
* [프로젝트(PROJ)](#project-proj)
* [비율(비율)](#rate-rate)
* [RichTextNote(RHNOTE)](#richtextnote-rhnote)
* [역할/작업 역할(ROLE)](#role--job-role-role)
* [작업(작업)](#task-task)
* [작업표(TSHET)](#timesheet-tshet)
* [UIFilter / 필터(UIFT)](#uifilter--filter-uift)
* [UIGroupBy / 그룹화(UIGB)](#uigroupby--grouping-uigb)
* [UIVview / View (UIVW)](#uiview--view-uivw)
* [사용자(사용자)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

### 승인(승인)

작업, 문서 또는 작업표와 같은 특정 작업 항목에서는 감독자나 다른 사용자가 작업 항목에 대해 로그오프해야 할 수 있습니다. Approval 객체는 작업 항목에 대해 로그오프하는 작업을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>이 필드가 추가되었으며 수행해야 하는 일별 작업 시간(분)이 표시됩니다. 형식은 다음과 같습니다 <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 배정(ASGN)

할당 객체는 작업 항목과 작업 항목에 지정된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>이 필드가 추가되었으며 수행해야 하는 일별 작업 시간(분)이 표시됩니다. 형식은 다음과 같습니다 <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
          <li>
            <p><b>isConcrusevic</b>
            </p>
            <p>이 필드가 추가되었으며 할당이 선택되었는지 여부를 반영하는 부울입니다. 작업 로드 밸런서에서 일별 할당 시간(분)이 편집된 경우, 할당이 중단됩니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum(CSTEM)

CustomEnum 개체는 상태 코드를 사람이 읽을 수 있는 텍스트로 변환하는 데 도움이 됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 고객 기본 설정(CUSTOMER)

CustomerPreferences 개체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>이름</b>
            </p>
            <p>다음 가능한 값을 추가했습니다.</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>이 작업은 고객이 기여자 라이선스 보유자를 자동 업그레이드하는 옵션을 비활성화했는지 여부를 설명하는 부울을 반환합니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 외부 섹션(EXTSEC)

ExternalSection 개체는 Workfront 보고서에 포함된 외부 웹 페이지입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>이 URL이 추가되고 보고서에 포함된 iFrame의 URL을 계산합니다.</p>
         </li>
          <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>이 URL이 추가되고 보고서에 포함된 iFrame의 URL을 계산합니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 시간(시간)

Hour 개체는 사용자가 작업표에 로깅한 시간을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업표HourIdentifier</b>
            </p>
            <p>추가됨. 이 매개 변수는 <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### 참고(참고)

Note 객체는 Workfront 객체에 대한 주석 또는 업데이트입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>이 필드가 추가되었으며 주석에 첨부된 문서 목록을 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Issue(OPTASK)

일반적으로 OpTask 개체를 Issue라고 합니다. 문제는 일반적으로 작업 또는 프로젝트 완료를 방지하는 데 문제가 있음을 나타내는 작업 항목입니다. 헬프데스크 요청도 있습니다. 변경 주문, 요청 및 버그도 문제입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>이 필드가 추가되었으며 수행해야 하는 일별 작업 시간(분)이 표시됩니다. 형식은 다음과 같습니다 <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>이 작업으로 필드가 추가되었습니다 <code>teamIDs</code> 여러 팀을 작업이나 문제에 지정하는 기능을 지원하기 위해</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 프로젝트(PROJ)

프로젝트는 Workfront 내의 작업 항목이며, Workfront이 사람들이 작업을 수행하는 데 도움이 되는 기본 빌딩 블록입니다. 프로젝트 객체는 공통, 특정 목표를 가진 작업 그룹을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerScheduledHours</b>
            </p>
            <p>이 필드가 추가되었으며 프로젝트에 대한 모든 예산책정 시간의 합계를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 비율(비율)

비율 개체는 Workfront의 청구 비율을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>이러한 매개 변수는 역할 개체에서 Rate 개체로 이동되었으므로 역할 및 사용자 개체에 여러 값(별도의 날짜 범위에 대해)이 있을 수 있습니다.</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>이러한 매개 변수는 Rate가 첨부된 개체의 ID 및 개체 코드를 나타냅니다.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>이 작업이 추가되었으며 Rate 객체를 지정된 객체에 첨부합니다. 이 끝점은 모든 연결 가능 개체에 대해 작동합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote(RHNOTE)

RichTextNote 개체는 굵게 또는 기울임꼴 텍스트와 같은 리치 텍스트를 포함하는 Workfront 개체에 작성된 주석 또는 업데이트입니다.

RichTextNote 개체가 플래그를 제거했습니다 `REPORTABLE`.

### 역할/작업 역할(ROLE)

역할 객체(작업 역할)는 사용자가 채울 수 있는 기능 능력 또는 기술 세트(예: 디자이너 또는 제품 관리자)를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
           <li>
            <p><b>요금</b>
            </p>
            <p>이 항목이 추가되었으며 이 역할에 첨부된 Rate 개체를 나타냅니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 작업(작업)

작업 객체는 최종 목표(프로젝트 완료)를 달성하는 단계로 수행되어야 하는 작업 항목을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>이 필드가 추가되었으며 수행해야 하는 일별 작업 시간(분)이 표시됩니다. 형식은 다음과 같습니다 <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>이 작업으로 필드가 추가되었습니다 <code>teamIDs</code> 여러 팀을 작업이나 문제에 지정하는 기능을 지원하기 위해</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 작업표(TSHET)

작업표 개체는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대해 실제 작업 시간을 입력할 수 있도록 하는 가상 타임카드를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>이 매개 변수로 플래그가 제거되었습니다. <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>이 매개 변수로 플래그가 제거되었습니다. <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>이 매개 변수가 추가되었으며 "전체 Workday의 등가 시간"에 대한 변경 사항에 관계없이 작업표 기간을 일 단위로 저장합니다.  예를 들어, 등가 시간이 6으로 설정되고 1일이 기록되면 등가 시간이 8시간으로 변경됩니다. <code>totalDays</code> 에는 값이 1입니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / 필터(UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>이 작업이 추가되었으며 필터 쿼리 맵을 가져와 <code>allowingnull</code> nullable 필드에 조인합니다.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>이러한 작업은 시스템 전체에서 필터, 보기 및 그룹화를 공유하는 기능을 지원합니다.</p><p>자세한 내용은 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / 그룹화(UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>이러한 작업은 시스템 전체에서 필터, 보기 및 그룹화를 공유하는 기능을 지원합니다.</p><p>자세한 내용은 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIVview / View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>다음 가능한 값을 추가했습니다.</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>이러한 작업은 시스템 전체에서 필터, 보기 및 그룹화를 공유하는 기능을 지원합니다.</p><p>자세한 내용은 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 사용자(사용자)

사용자 개체는 로그인하고 시스템과 상호 작용할 수 있는 Workfront에 계정이 있는 사람을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
           <li>
            <p><b>요금</b>
            </p>
            <p>이 항목이 추가되었으며 이 사용자에게 첨부된 Rate 개체를 나타냅니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

UserNote 개체는 알림입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">쿼리</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>다음 가능한 값을 추가했습니다.
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 작업 시간(작업 시간)

작업 개체는 Task 및 OpTask가 모두 상속하고 두 Task 간에 공통 코드를 공유하는 공통 인터페이스입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>이 필드가 추가되었으며 수행해야 하는 일별 작업 시간(분)이 표시됩니다. 형식은 다음과 같습니다 <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
