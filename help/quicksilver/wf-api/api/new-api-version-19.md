---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 19의 새로운 기능
description: Adobe Workfront은 2022년 4월 6일에 API 버전 19를 출시했습니다. API 버전 19에는 버전 18의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 84909dea-7ce1-4ad3-90f5-9dbdb354eaa4
source-git-commit: 1c1f9f46ea25ffa7d01c1a762b0478a5edb3339e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# API 버전 19의 새로운 기능

Adobe Workfront은 2024년 4월 8일에 API 버전 19를 출시했습니다. API 버전 19에는 버전 18의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

API 버전 19에 대한 리소스를 추가하지 않았습니다.

## 제거된 리소스

API 버전 19에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

### 액세스 수준(ACSLVL)

AccessLevel 개체는 사용자와 연결되어 있으며 사용자가 액세스할 수 있는 항목을 결정하는 AccessLevelPermissions 집합에 대해 설명합니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>액세스 제한</b><p>다음과 같은 가능한 값이 추가되었습니다.
            </p>
            <ul>
              <li>
                <p>Workfront AI Assistant(AIOFF) 비활성화
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 할당(할당)

할당 개체는 작업 항목과 작업 항목에 할당된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다.

Assignment 개체가 **DATA_EXTENSIBLE** 플래그를 추가했습니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 직접 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>범주 ID</b><p>범주는 사용자 정의 양식입니다. 이 필드는 사용자 정의 양식을 할당에 추가하는 기능을 지원합니다.
            </p>
          </li>
          <li>
            <p><b>우선 순위</b><p>이 필드에서는 다음 값을 사용할 수 있습니다.
            <ul>
              <li>0(없음)</li>
              <li>1(낮음)</li>
              <li>2(보통)</li>
              <li>3(높음)</li>
              <li>4(긴급)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>다음 참조 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>범주</b><p>범주는 사용자 정의 양식입니다. 이 필드는 사용자 정의 양식을 할당에 추가하는 기능을 지원합니다.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>다음 컬렉션 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>objectCategors</b><p>범주는 사용자 정의 양식입니다. 이 필드는 사용자 정의 양식을 할당에 추가하는 기능을 지원합니다.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### 범주(CTGY)

Category 객체는 사용자 정의 양식입니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>사용자 정의 양식을 할당에 추가하는 기능을 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>catObjCode</b><p>다음과 같은 가능한 값이 추가되었습니다.
            </p>
            <ul>
              <li>
                <p>할당(할당)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objType</b><p>다음과 같은 가능한 값이 추가되었습니다.
            </p>
            <ul>
              <li>
                <p>할당(할당)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 분류기(CLSF)

분류자는 위치입니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">액션</td>
      <td>다음 작업이 추가되었습니다.
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 고객

Customer 개체는 Workfront 인스턴스를 사용하는 조직을 나타냅니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>사용자 정의 열거형 유형</b><p>다음과 같은 가능한 값이 추가되었습니다.
            </p>
            <ul>
              <li>
                <p>할당 우선순위(PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>CustomEnum 개체는 상태 코드를 사람이 읽을 수 있는 텍스트로 변환하는 데 도움이 됩니다.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences (CUSTPR)

CustomerPreferences 객체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>이름</b><p>다음 가능한 값을 제거했습니다.
            </p>
            <ul>
              <li>
                <p>업데이트 스트림에서 확대/축소 통합 활성화(password:zoomIntegrationEnabled)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 문서(DOCU)

Document 객체는 파일(예: 작성된 자료, 이미지 또는 기타 정보 형식)을 나타냅니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>필드 <code>folderID</code>을(를) 추가했습니다.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>추가됨.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### 환율(환율)

ExchangeRate 개체는 Workfront에 설정된 통화 환율을 나타냅니다. Exchange 개체가 동적이지 않습니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
      <ul>
      <li>다음 필드에 유효성 검사기 <code>REQUIRED</code>이(가) 추가되었습니다.
        <ul>
          <li><p><b>통화</b></li>
          <li><p><b>비율</b></li></ul>
      <li>다음 필드가 추가되었습니다.
        <ul>
          <li><p><b>입력자 ID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>마지막 업데이트 날짜</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
      <ul>
        <li>다음 필드가 추가되었습니다.
        <ul>
          <li><p><b>입력한 사람</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 그룹(그룹)

Group 객체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서 구조를 나타냅니다.

Group 개체가 **SHARABLE** 플래그를 추가했습니다.

### 시간(시간)

Hour 개체는 타임시트에 사용자가 기록한 시간을 나타냅니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
      다음 필드가 추가되었습니다.
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>청구됨</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submittedByID</b></li>
          </ul>
          <p><b>시간</b> 필드가 다음과 같이 변경되었습니다.</p>
          <ul> 
          <li> 검사기 <b>GREATER_THAN</b>이(가) 제거되었습니다.</li>
          <li> 검사기 <b>NOT_EQUAL</b>이(가) 추가되었습니다.</li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
      다음 작업이 추가되었습니다.
        <ul>
          <li><p><b>승인</b></li>
          <li><p><b>승인 취소</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### 저널 게시물(JRNL)

JournalEntry 개체는 특정 개체 필드에 대한 정보를 해당 필드가 수정될 때마다 기록하도록 설정할 수 있습니다. 필드가 저널 게시물 개체의 일부로 기록되도록 설정되면 해당 필드를 수정할 때마다 해당 저널 게시물이 만들어집니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>플래그</b><p>다음과 같은 가능한 값이 추가되었습니다.
            </p>
            <ul>
              <li>
                <p>비용 요금(CR)
                </p>
              </li>
              <li>
                <p>청구 요금(BR)
                </p>
              </li>
              <li>
                <p>일반 재무(GF)임
                </p>
              </li>
              <li>
                <p>CF(Combined Finance)
                </p>
              </li>
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
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>다음과 같은 가능한 값이 추가되었습니다.
            <ul>
            <li>기간(DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>보다 사용자 친화적이고 유연한 시스템을 만들기 위해 <b>위젯(WIDGET)</b> 필드 형식은 더 이상 사용되지 않으며 다음 필드 형식으로 분할됩니다.
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>이미지(이미지)</li>
            <li>PDF(PDF)</li>
            <li>비디오(비디오)</li>
            <li>외부 조회(EXTRNL)</li>
            <li>다중 선택 외부 조회(MULTEXTRNL)</li>
            <li>네이티브 필드(WFNATIVE)</li>
            <li>계획 필드(WFPLANNING)</li>
            <li>시간 단계별 KPI(시간대별)</li>
            <li>롤업(롤업)</li>
            <li>문서(문서)</li>
           </ul>
          </li>
          <li>
            <p><b>구성</b><p>추가됨.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 역할(역할)

역할 객체(작업 역할)는 Designer 또는 제품 관리자와 같이 사용자가 채울 수 있는 기능 역량 또는 스킬 세트를 나타냅니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
    다음 필드가 추가되었습니다.
        <ul>
          <li><p><b>마지막 업데이트 날짜</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
        다음 필드가 추가되었습니다.
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### 스코어카드 질문 {#scorecardquestion}

ScoreCardQuestion 객체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자가 결정하며, 관리자는 이에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 파악할 수 있습니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
            <p><b>displayType</b></p><p>보다 사용자 친화적이고 유연한 시스템을 만들기 위해 <b>위젯(WIDGET)</b> 필드 형식은 더 이상 사용되지 않으며 다음 필드 형식으로 분할됩니다.
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>이미지(이미지)</li>
            <li>PDF(PDF)</li>
            <li>비디오(비디오)</li>
            <li>외부 조회(EXTRNL)</li>
            <li>다중 선택 외부 조회(MULTEXTRNL)</li>
            <li>네이티브 필드(WFNATIVE)</li>
            <li>계획 필드(WFPLANNING)</li>
            <li>시간 단계별 KPI(시간대별)</li>
            <li>롤업(롤업)</li>
            <li>문서(문서)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment(작업)

TemplateAssignment 개체는 템플릿 작업과 작업에 할당된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다. 템플릿을 프로젝트에 사용하면 해당 사용자, 팀 또는 그룹이 작업에 할당됩니다.

TemplateAssignment 개체가 **DATA_EXTENSIBLE** 플래그를 추가했습니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 직접 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>범주 ID</b><p>범주는 사용자 정의 양식입니다. 이 필드는 사용자 정의 양식을 할당에 추가하는 기능을 지원합니다.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>다음 참조 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>범주</b><p>범주는 사용자 정의 양식입니다. 이 필드는 사용자 정의 양식을 할당에 추가하는 기능을 지원합니다.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>다음 컬렉션 필드가 추가되었습니다.
        <ul>
          <li>
            <p><b>objectCategors</b><p>범주는 사용자 정의 양식입니다. 이 필드는 사용자 정의 양식을 할당에 추가하는 기능을 지원합니다.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 타임시트(세트)

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

<table>
  <tbody>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>제거됨.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>
