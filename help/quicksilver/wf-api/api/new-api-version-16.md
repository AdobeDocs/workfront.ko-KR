---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 16의 새로운 기능
description: Adobe Workfront은 2022년 4월 6일에 API 버전 16을 출시했습니다. API 버전 16에는 버전 15의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# API 버전 16의 새로운 기능

Adobe Workfront은 2023년 4월 6일에 API 버전 16을 출시했습니다. API 버전 16에는 버전 15의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

API 버전 16에 대해 추가된 리소스가 없습니다.

## 제거된 리소스

API 버전 16에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [승인(승인)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [외부 섹션(EXTSEC)](#externalsection-extsec)
* [시간(시간)](#hour-hour)
* [레이아웃 템플릿(UITMPL)](#layouttemplate-uitmpl)
* [참고(참고)](#note-note)
* [OpTask / 문제 (OPTASK)](#note-note)
* [프로젝트(프로젝트)](#project-proj)
* [비율(비율)](#rate-rate)
* [리치 텍스트 메모(RHNOTE)](#richtextnote-rhnote)
* [역할/작업 역할(역할)](#role--job-role-role)
* [작업(작업)](#task-task)
* [타임시트(세트)](#timesheet-tshet)
* [UIFilter / 필터 (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / 그룹화(UIGB)](#uigroupby--grouping-uigb)
* [UIView / 보기 (UIVW)](#uiview--view-uivw)
* [사용자(사용자)](#user-user)
* [UserNote(USRNOT)](#usernote-usrnot)

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

작업, 문서 또는 타임시트와 같은 특정 작업 항목에서는 감독자 또는 다른 사용자가 해당 작업 항목을 승인해야 할 수 있습니다. 승인 오브젝트는 작업 항목에 대한 사인오프 작업을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업 날짜</b>
            </p>
            <p>이 필드가 추가되었으며, 필요한 하루 작업 시간(분)을 표시합니다. 형식은 다음과 같습니다. <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 할당(할당)

할당 개체는 작업 항목과 작업 항목에 할당된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업 날짜</b>
            </p>
            <p>이 필드가 추가되었으며, 필요한 하루 작업 시간(분)을 표시합니다. 형식은 다음과 같습니다. <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
          <li>
            <p><b>isContofed</b>
            </p>
            <p>이 필드가 추가되었으며, 은 할당의 윤곽선 표시 여부를 반영하는 부울입니다. 일별 할당 시간이 업무 균형자에서 편집된 경우 할당이 윤곽선으로 표시됩니다.</p>
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

### CustomerPreferences (CUSTPR)

CustomerPreferences 객체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

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
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
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
            <p>이 작업은 고객이 기여자 라이선스 소유자를 자동 업그레이드하는 옵션을 비활성화했는지 여부를 설명하는 부울을 반환합니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 외부 섹션(EXTSEC)

ExternalSection 객체는 Workfront 보고서에 포함된 외부 웹 페이지입니다.

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
            <p>이 항목이 추가되었으며, 보고서에 포함된 iFrame의 URL이 계산됩니다.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>이 항목이 추가되어 보고서에 포함된 iFrame의 URL이 계산됩니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 시간(시간)

Hour 개체는 타임시트에 사용자가 기록한 시간을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>추가됨. 이 매개 변수는 다음을 사용하여 만든 시간을 식별하는 데 사용됩니다. <code>batchSave</code>. </p>
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

Note 객체는 Workfront 객체에 대한 댓글 또는 업데이트입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>첨부된 문서</b>
            </p>
            <p>이 필드가 추가되었으며 주석에 첨부된 문서 목록을 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / 문제 (OPTASK)

OpTask 객체를 일반적으로 문제라고 합니다. 문제는 일반적으로 작업 또는 프로젝트의 완료를 방해하는 문제가 있음을 나타내는 작업 항목입니다. 문제는 헬프 데스크 요청일 수도 있습니다. 변경 주문, 요청 및 버그도 문제가 됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업 날짜</b>
            </p>
            <p>이 필드가 추가되었으며, 필요한 하루 작업 시간(분)을 표시합니다. 형식은 다음과 같습니다. <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
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
            <p>이 작업은 필드를 추가했습니다. <code>teamIDs</code> 작업 또는 문제에 여러 팀을 할당하는 기능을 지원합니다.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 프로젝트(프로젝트)

프로젝트는 Workfront 내의 작업 항목이며 Workfront이 작업을 수행하는 데 도움을 주는 방식의 주요 빌딩 블록입니다. Project 개체는 일반적인 특정 목표를 가진 작업 그룹을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetHours</b>
            </p>
            <p>이 필드가 추가되었으며 프로젝트에 대한 모든 예산 시간의 합계를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 비율(비율)

요금 오브젝트는 Workfront에서의 청구 요금을 나타냅니다.

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
           <p>이러한 매개 변수는 Role 개체에서 Rate 개체로 이동되었으므로 Role 및 User 개체는 별도의 날짜 범위에 대해 여러 값을 가질 수 있습니다.</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>이러한 매개 변수는 Rate가 첨부된 개체의 ID와 개체 코드를 나타냅니다.
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
           <p>이 작업이 추가되었으며 Rate 개체를 지정된 개체에 연결합니다. 이 끝점은 모든 Rate Attachable 개체에 대해 작동합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 리치 텍스트 메모(RHNOTE)

RichTextNote 객체는 굵게 또는 기울임꼴 텍스트와 같은 서식 있는 텍스트를 포함하는 Workfront 객체에 대한 댓글 또는 업데이트입니다.

RichTextNote 개체에서 플래그를 제거했습니다. `REPORTABLE`.

### 역할/작업 역할(역할)

역할 객체(작업 역할)는 사용자가 채울 수 있는 기능 역량 또는 기술 세트(예: 디자이너 또는 제품 관리자)를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
           <li>
            <p><b>비율</b>
            </p>
            <p>이 항목이 추가되었으며 이 역할에 첨부된 비율 개체를 나타냅니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 작업(작업)

작업 객체는 최종 목표 달성(프로젝트 완료)을 위한 단계로 수행해야 하는 작업 항목을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업 날짜</b>
            </p>
            <p>이 필드가 추가되었으며, 필요한 하루 작업 시간(분)을 표시합니다. 형식은 다음과 같습니다. <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
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
            <p>이 작업은 필드를 추가했습니다. <code>teamIDs</code> 작업 또는 문제에 여러 팀을 할당하는 기능을 지원합니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 타임시트(세트)

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

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
            <p>이 매개 변수는 플래그를 제거했습니다. <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEdit</b>
            </p>
            <p>이 매개 변수는 플래그를 제거했습니다. <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>이 매개 변수가 추가되었으며 "전체 Workday에 해당하는 시간"의 변경과 관계없이 타임시트 지속 시간을 일 단위로 저장합니다.  예를 들어, 등가 시간이 6으로 설정되어 있고 1일이 기록된 경우, 등가 시간은 8시간으로 변경됩니다. <code>totalDays</code> 에는 여전히 1의 값이 있습니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / 필터 (UIFT)



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
            <p>이 작업이 추가되었으며 필터 쿼리 맵을 가져오고 다음을 추가합니다. <code>allowingnull</code> nullable 필드에 대한 조인.</p>
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


### UIView / 보기 (UIVW)

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
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
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

사용자 개체는 로그인하여 시스템과 상호 작용할 수 있는 Workfront의 계정을 가진 사용자를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
           <li>
            <p><b>비율</b>
            </p>
            <p>이 항목이 추가되었으며 이 사용자에게 첨부된 비율 개체를 나타냅니다.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote(USRNOT)

UserNote 객체는 알림입니다.

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
            <p>다음과 같은 가능한 값이 추가되었습니다.
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

### 작업(작업)

Work 개체는 Task와 OpTask가 모두 상속하는 공통 인터페이스이며 두 개체 간에 공통 코드를 공유합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업 날짜</b>
            </p>
            <p>이 필드가 추가되었으며, 필요한 하루 작업 시간(분)을 표시합니다. 형식은 다음과 같습니다. <code>YYYY-MM-DD: (number of minutes)</code>, 및 은 시간대를 고려합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
