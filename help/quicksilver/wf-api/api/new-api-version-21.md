---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 21의 새로운 기능
description: Adobe Workfront은 2025년 10월 23일에 API 버전 21을 출시했습니다. API 버전 21에는 버전 20의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 155323314712e020a638619d9bf10d678078645e
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 3%

---

# API 버전 21의 새로운 기능

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

Adobe Workfront은 2025년 10월 23일에 API 버전 21을 출시했습니다. API 버전 21에는 버전 20의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

## 제거된 리소스

### AssignmentBillingRole(ASBLRL)

AssignmentBillingRole 개체 및 해당 필드를 모두 제거했습니다.

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
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
            </ul>
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
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
         </li>
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
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
            </ul>
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
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>팀 할당</b>
            </p>
            <p>추가됨</p>
          </li>
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
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>제거됨</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 범주(CTGY)

Category 객체는 사용자 정의 양식입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (팀)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (팀)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 고객(CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (타임라인 계산을 위한 Java 애플릿 사용 비활성화)
            </p>
            <p>추가됨</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 문서(DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>추가됨</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 문서 폴더

DocumentFolder 개체가 `RESTORABLE` 플래그를 추가했습니다.

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
            <p><b>getTerejectionCommentporaryCloudURL</b>
            </p>
            <p>검사기를 추가했습니다. <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### OpTask(OPTASK)

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>추가됨</p>
              </li>
            </ul>
         </li>
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
            <p><b>dataType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (어휘 서식 있는 텍스트)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (단일 라인 롤업)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>추가됨</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">기본 필드</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>추가됨</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio(포트)

Portfolio 객체는 동일한 리소스(일반적으로 돈 또는 완료하는 사람)에 대해 경쟁하는 프로젝트의 컬렉션입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>추가됨</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 프로그램(PRGM)

프로그램 객체는 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 프로젝트 하위 집합입니다.

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
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>추가됨</p>
              </li>
            </ul>
         </li>
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
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (연락처 정보 편집)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>추가됨</p>
            </li>
            </ul>
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
            <p><b>localBillingPerHour</b>
            </p>
            <p>제거됨</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>제거됨</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 역할(역할)

역할 객체(작업 역할)는 Designer 또는 제품 관리자와 같이 사용자가 채울 수 있는 기능 역량 또는 스킬 세트를 나타냅니다.

<div class="preview">

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>통화 재정의</b>
            </p>
            <p>제거됨</p>
              </li>
          <li>
            <p><b>비용 비율 재정의</b>
            </p>
            <p>제거됨</p>
              </li>
          <li>
            <p><b>청구 요금 재정의</b>
            </p>
            <p>제거됨</p>
              </li>
      </td>
    </tr>
  </tbody>
</table>

</div>

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
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion(SCORREQ)

ScoreCardQuestion 객체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자가 결정하며, 관리자는 이에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 파악할 수 있습니다.<table>
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
                <p><code>SNGLROLLUP</code> (단일 라인 롤업)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>팀 할당</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### 팀

Team 개체가 `DATA_EXTENDIBLE` 및 `SHARABLE` 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
        <ul>
          <li>
            <p><b>범주</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>개체 범주</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### 템플릿 할당

TemplateAssignment 개체가 `ATTRIBUTE_ATTACHABLE` 플래그를 추가했습니다.

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>팀 할당</b>
            </p>
            <p>추가됨</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


