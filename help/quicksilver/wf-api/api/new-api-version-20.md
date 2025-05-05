---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 20의 새로운 기능
description: Adobe Workfront은 2022년 4월 6일에 API 버전 20을 출시했습니다. API 버전 20에는 버전 19의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# API 버전 20의 새로운 기능

Adobe Workfront은 2025년 5월 4일에 API 버전 20을 출시했습니다. API 버전 20에는 버전 19의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

API 버전 20에 대한 리소스를 추가하지 않았습니다.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## 제거된 리소스

API 버전 20에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

### AccessLevelPermissions(ALVPER)

AccessLevelPermissions 개체는 Workfront 개체에 액세스, 만들기 또는 수정할 수 있는 특정 권한을 나타냅니다. 그런 다음 이러한 권한을 액세스 수준과 연결할 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest(ACSREQ)

사용자에게 Workfront의 필요한 오브젝트에 대한 액세스 권한이 없는 경우 해당 오브젝트에 대한 액세스를 요청할 수 있습니다. AccessRequest 개체는 이 요청을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업</b>
            </p>
             <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule(ACSRUL)

AccessRule 개체는 사용자가 만드는 프로젝트를 공유할 수 있는 방법을 결정하는 사용자 지정 액세스 수준에 설정된 규칙을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AnnouncementAttachment(ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>파일 확장명</b>
            </p>
             <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>actualBenefits</li>
              <li>실제 청구 가능 경비</li>
              <li>실제 비용</li>
              <li>실제 경비</li>
              <li>실제 인건비</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>실제 값</li>
              <li>청구된 수익</li>
              <li>예산</li>
              <li>예산 비용</li>
              <li>budgetHours</li>
              <li>예산 인건비</li>
              <li>비용 금액</li>
              <li>costType</li>
              <li>고정 비용</li>
              <li>fixedRevenue</li>
              <li>plannedBenefits</li>
              <li>계획된 청구 가능 경비</li>
              <li>계획된 비용</li>
              <li>plannedExpenseCost</li>
              <li>계획된 인건비</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>실제 비용</li>
          <li>actualRevenue</li>
          <li>계획된 비용</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p><code>DYNAMIC</code>, <code>LAZY_READ</code> 플래그를 추가했습니다. <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetHours</b></p> <p>플래그가 추가됨 <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>가능한 값 <code>URH</code>을(를) 추가했습니다(시간별 사용자 및 역할). </li>
          <li><p><b>revenueType</b></p> <p>가능한 값 <code>URH</code>(시간별 사용자 및 역할), <code>URC</code>(시간별 사용자 및 역할) 및 <code>URF</code>(시간별 사용자 및 역할 + 고정)을 추가했습니다.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
          <p>다음 필드가 추가되었습니다.</p>
             <ul>
              <li><b>청구 요금</b></li>
              <li><b>원가율</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### 할당(할당)

할당 개체는 작업 항목과 작업 항목에 할당된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다.

할당 개체에서 플래그 `ATTRIBUTE_ATTACHABLE` 및 `DOMAIN_EXTENDABLE`을(를) 추가했습니다.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### 아바타

아바타 개체는 사용자 사진입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>추가됨</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>추가됨</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>복사</b>
            </p>
             <p>추가됨</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### 기준선(BLIN)

기준선은 특정 시점의 프로젝트 성능에 대한 스냅샷입니다. 여기에는 주요 날짜, 진행 상황, 비용 및 수익 값과 같은 프로젝트에 대한 주요 정보가 저장됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 청구 가능 경비</li>
              <li>실제 비용</li>
              <li>actualNonBillableExpenseCost</li>
              <li>예산</li>
              <li>eac</li>
              <li>계획된 청구 가능 경비</li>
              <li>계획된 비용</li>
              <li>계획된 비용 청구 불가 비용</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>실제 비용</li>
          <li>계획된 비용</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>플래그가 추가됨 <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 초기 계획 작업(BSTSK)

기준선은 특정 시점의 프로젝트 성능에 대한 스냅샷입니다. 여기에는 주요 날짜, 진행 상황, 비용 및 수익 값과 같은 프로젝트에 대한 주요 정보가 저장됩니다. 베이스라인을 생성하면 작업 정보가 해당 베이스라인의 베이스라인 작업에도 캡처됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 청구 가능 경비</li>
              <li>실제 비용</li>
              <li>actualNonBillableExpenseCost</li>
              <li>계획된 청구 가능 경비</li>
              <li>계획된 비용</li>
              <li>계획된 비용 청구 불가 비용</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>실제 비용</li>
          <li>계획된 비용</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>플래그가 추가됨 <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BillingRecord(BILL)

BillingRecord 개체는 청구할 수 있는 수익, 시간 또는 비용을 기록합니다. 이 정보는 외부 회계 시스템에서 송장을 생성하는 데 사용할 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>금액</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>추가됨</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

### CategoryParameter(CTGAA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>구성</b>
            </p>
             <p>추가됨</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 회사(CMPY)

Company 객체는 사람들의 컬렉션으로 구성된 조직을 나타냅니다.

Company 개체가 `SHARABLE` 플래그를 추가했습니다.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissumove)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 환율(환율)

ExchangeRate 개체는 Workfront에 설정된 통화 환율을 나타냅니다. Exchange 개체가 동적이지 않습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
           <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>비율</li>
      </td>
    </tr>
  </tbody>
</table>


### 재무 데이터(FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 청구 가능 경비</li>
              <li>실제 경비</li>
              <li>actualFixedRevenue</li>
              <li>실제 인건비</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>고정 비용</li>
              <li>계획된 청구 가능 경비</li>
              <li>plannedExpenseCost</li>
              <li>계획된 고정 수입</li>
              <li>계획된 인건비</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>totalRealCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceWorkbenchHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 그룹(그룹)

Group 객체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서 구조를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>통화</b>
            </p>
             <p>추가됨</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 비용</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
              <li>실제 비용</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>환율 원본</b></p> <p>추가됨</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask(OPTASK)

OpTask 객체를 일반적으로 문제라고 합니다. 문제는 일반적으로 작업 또는 프로젝트의 완료를 방해하는 문제가 있음을 나타내는 작업 항목입니다. 문제는 헬프 데스크 요청일 수도 있습니다. 변경 주문, 요청 및 버그도 문제가 됩니다.

OpTask 개체가 DOMAIN_EXTENSIBLE 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 비용</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
              <li>실제 비용</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 매개 변수(매개 변수)

Parameter 개체는 사용자 지정 필드입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (내부 조회)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (다중 선택 내부 조회)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio(포트)

Portfolio 객체는 동일한 리소스(일반적으로 돈 또는 완료하는 사람)에 대해 경쟁하는 프로젝트의 컬렉션입니다.

Portfolio 개체가 `DOMAIN_EXTENDABLE` 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>정렬됨</li>
              <li>예산</li>
              <li>통화</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 프로그램(PRGM)

프로그램 객체는 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 프로젝트 하위 집합입니다.

Program 개체가 `DOMAIN_EXTENDABLE` 플래그를 추가했습니다.

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
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>actualBenefits</li>
              <li>실제 청구 가능 경비</li>
              <li>실제 비용</li>
              <li>실제 경비</li>
              <li>실제 인건비</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>실제 값</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>청구된 수익</li>
              <li>예산</li>
              <li>예산 비용</li>
              <li>budgetHours</li>
              <li>예산 인건비</li>
              <li>eac</li>
              <li>고정 비용</li>
              <li>fixedRevenue</li>
              <li>plannedBenefits</li>
              <li>계획된 청구 가능 경비</li>
              <li>계획된 비용</li>
              <li>plannedExpenseCost</li>
              <li>계획된 인건비</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>실제 비용</li>
          <li>actualRevenue</li>
          <li>계획된 비용</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetHours</b></p> <p>플래그가 추가됨 <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef(QUED)

QueueDef 개체는 사용자가 문제를 제출할 수 있도록 헬프 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (사용자 지정 데이터에서 제거)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (하위 프로젝트 추가)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 비율(비율)

요금 오브젝트는 Workfront에서의 청구 요금을 나타냅니다.

Rate 개체가 `ATTRIBUTE_ATTACHABLE` 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>다음 필드가 추가되었습니다.
          <ul>
          <li>통화</li>
          <li>잠김</li>
          <li>유형</li>
          <li>값</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 역할(역할)

역할 객체(작업 역할)는 Designer 또는 제품 관리자와 같이 사용자가 채울 수 있는 기능 역량 또는 스킬 세트를 나타냅니다.

Role 개체가 `DOMAIN_EXTENDABLE` 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
          <p>다음 필드가 추가되었습니다.
          <ul>
          <li>청구 요금</li>
          <li>원가율</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 예약된 보고서(SCHREP)

ScheduledReport 개체는 전송을 위해 예약되도록 구성된 보고서를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>형식</b>
            </p>
             <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion(SCORREQ)

ScoreCardQuestion 객체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자가 결정하며, 관리자는 이에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 파악할 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
             <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li><p><code>INTRNL</code> (내부 조회)</p></li>
              <li><p><code>MULTINTRNL</code> (다중 선택 내부 조회)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 작업(작업)

작업 객체는 최종 목표 달성(프로젝트 완료)을 위한 단계로 수행해야 하는 작업 항목을 나타냅니다.

작업 개체가 `DOMAIN_EXTENDABLE` 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 청구 가능 경비</li>
              <li>실제 비용</li>
              <li>실제 경비</li>
              <li>실제 인건비</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>비용 금액</li>
              <li>costType</li>
              <li>계획된 청구 가능 경비</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>계획된 인건비</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>실제 비용</li>
          <li>actualRevenue</li>
          <li>계획된 비용</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>다음과 같은 가능한 값이 추가되었습니다.<ul><li><code>URH</code> (시간별 사용자 및 역할)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>다음과 같은 가능한 값이 추가되었습니다.<ul><li><code>URH</code> (시간별 사용자 및 역할)</li><li><code>URC</code> (시간별 사용자 및 역할(상한 포함))</li><li><code>URF</code> (시간별 사용자 및 역할 + 고정)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 템플릿(TMPL)

Template 객체는 프로젝트의 패턴을 나타냅니다. 템플릿에서 프로젝트를 생성하여 시간을 절약할 수 있습니다. 템플릿에는 팀과 작업이 포함되어 있으며, 이 작업은 템플릿에서 만든 프로젝트에 복사됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>예산</li>
              <li>고정 비용</li>
              <li>fixedRevenue</li>
              <li>plannedBenefits</li>
              <li>계획된 청구 가능 경비</li>
              <li>계획된 비용</li>
              <li>plannedExpenseCost</li>
              <li>계획된 인건비</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>작업 필요</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>계획된 비용</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
          <p>다음 필드가 추가되었습니다.</p>
             <ul>
              <li><b>청구 요금</b></li>
              <li><b>원가율</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### 템플릿 작업(TTSK)

TemplateTask 개체는 Template의 일부인 작업을 나타냅니다. 템플릿 작업은 템플릿이 사용되는 프로젝트의 작업이 됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>billingAmount</li>
              <li>비용 금액</li>
              <li>costType</li>
              <li>계획된 청구 가능 경비</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>계획된 인건비</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>plannedRevenue</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>계획된 비용</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>다음과 같은 가능한 값이 추가되었습니다.<ul><li><code>URH</code> (시간별 사용자 및 역할)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>다음과 같은 가능한 값이 추가되었습니다.<ul><li><code>URH</code> (시간별 사용자 및 역할)</li><li><code>URC</code> (시간별 사용자 및 역할(상한 포함))</li><li><code>URF</code> (시간별 사용자 및 역할 + 고정)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 타임시트(세트)

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>제거됨</p>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 업데이트(업데이트)

Workfront의 작업 항목을 업데이트하여 사용자에게 현재 상태를 알릴 수 있습니다. Update 개체는 이러한 업데이트 중 하나를 나타냅니다. 업데이트는 사용자가 입력하거나 Workfront 시스템에서 만들 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
             <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 사용자(사용자)

사용자 개체는 로그인하여 시스템과 상호 작용할 수 있는 Workfront의 계정을 가진 사용자를 나타냅니다.

사용자 개체가 필드 `ATTRIBUTE_ATTACHABLE` 및 `DOMAIN_EXTENDABLE`을(를) 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
          <p>다음 필드가 추가되었습니다.</p>
             <ul>
              <li><b>청구 요금</b></li>
              <li><b>원가율</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
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
            <p>다음 필드에서 플래그 <code>RESTRICTABLE</code>을(를) 추가했습니다.
            </p>
             <ul>
              <li>실제 청구 가능 경비</li>
              <li>실제 비용</li>
              <li>실제 경비</li>
              <li>실제 인건비</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>비용 금액</li>
              <li>costType</li>
              <li>계획된 청구 가능 경비</li>
              <li>계획된 비용</li>
              <li>plannedExpenseCost</li>
              <li>계획된 인건비</li>
              <li>계획된 비용 청구 불가 비용</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>다음 필드의 형식이 <code>double</code>에서 <code>class java.math.BigDecimal</code>(으)로 변경되었습니다.
          <ul>
          <li>실제 비용</li>
          <li>actualRevenue</li>
          <li>계획된 비용</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p><code>DYNAMIC</code>, <code>LAZY_READ</code> 플래그를 추가했습니다. <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetHours</b></p> <p>플래그가 추가됨 <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>가능한 값 <code>URH</code>을(를) 추가했습니다(시간별 사용자 및 역할). </li>
          <li><p><b>revenueType</b></p> <p>가능한 값 <code>URH</code>(시간별 사용자 및 역할), <code>URC</code>(시간별 사용자 및 역할) 및 <code>URF</code>(시간별 사용자 및 역할 + 고정)을 추가했습니다.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



