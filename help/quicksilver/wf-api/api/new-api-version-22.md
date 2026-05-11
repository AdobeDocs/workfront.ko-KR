---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 22의 새로운 기능
description: Adobe Workfront은 2026년 5월 11일에 API 버전 22를 출시했습니다. API 버전 22에는 버전 21의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 1%

---

# API 버전 22의 새로운 기능

Adobe Workfront은 2026년 5월 8일에 API 버전 22를 출시했습니다. API 버전 22에는 버전 21의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

API 버전 22에 대해 다음 리소스가 추가되었습니다.

### ReportShareableFolder(RPSHFD)

공유 가능한 보고서 폴더를 사용하여 보고서를 구성하고 해당 폴더를 다른 사용자와 공유할 수 있습니다. 이 기능은 대량의 보고서를 관리하고 확장 가능하고 일관된 액세스 제어가 필요한 팀을 위해 설계되었습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>ID</li>
          <li>이름</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>ID</li>
          <li>이름</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">기본 필드</td>
      <td>
        <ul>
          <li>이름</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>추가</li>
          <li>수</li>
          <li>DELETE</li>
          <li>편집</li>
          <li>GET</li>
          <li>보고서</li>
          <li>검색</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## 제거된 리소스

다음 리소스가 API 버전 22에서 제거되었습니다.

### UserLocation(USRLOC)

이 개체는 제거되었습니다.

## 수정된 리소스

API 버전 22에 대해 다음 리소스가 수정되었습니다.

### 액세스 수준(ACSLVL)

AccessLevel 개체는 사용자와 연결되어 있으며 사용자가 액세스할 수 있는 항목을 결정하는 AccessLevelPermissions 집합에 대해 설명합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 가능한 값에 대한 변경 사항으로 수정되었습니다. 자세한 내용은 개발자 설명서를 참조하십시오.
        <ul>
          <li><b>필드 액세스 권한</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions(ALVPER)

AccessLevelPermissions 개체는 Workfront 개체에 액세스, 만들기 또는 수정할 수 있는 특정 권한을 나타냅니다. 그런 다음 이러한 권한을 액세스 수준과 연결할 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 가능한 값에 대한 변경 사항으로 수정되었습니다. 자세한 내용은 개발자 설명서를 참조하십시오.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>다음 필드가 가능한 값에 대한 변경 사항으로 수정되었습니다. 자세한 내용은 개발자 설명서를 참조하십시오.
        <ul>
          <li><b>액션</b></li>
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
      <td>다음 필드가 가능한 값에 대한 변경 사항으로 수정되었습니다. 자세한 내용은 개발자 설명서를 참조하십시오.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
        </ul>
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
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 회사(CMPY)

Company 객체는 사람들의 컬렉션으로 구성된 조직을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmProjectID</b></li>
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
      <td>추가됨
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">쿼리</td>
      <td>추가됨
        <ul>
          <li><p><b>assignmentStatus</b></p></li>
          <li><p><b>예약 상태</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### 고객(CUST)

Customer 개체는 Workfront 인스턴스를 사용하는 조직을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 수정되었습니다.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (예약 상태)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (할당 상태)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFile마이그레이션 활성화됨</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomer시스템 파일 마이그레이션 날짜</b></li>
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
      <td>다음 필드가 수정되었습니다.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>엔터프라이즈 스토리지 관리를 지원하기 위해 다음과 같은 값을 추가했습니다.</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
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
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>다음 작업이 수정되었습니다.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder(DOCFDR)

문서를 폴더로 구성할 수 있습니다. 개인 문서 영역에 개인 폴더를 만들 수 있습니다. DocumentFolder 개체는 이러한 폴더 중 하나를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

DocumentVersion 개체는 작성된 자료, 이미지 또는 다른 형태의 정보 등 파일의 특정 버전을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      다음 필드가 수정되었습니다.
        <ul>
          <li><b>version</b><p>유효성 검사기 "필수"를 제거했습니다.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>다음 작업이 추가되었습니다.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">작업</td>
      <td>다음 작업이 추가되었습니다.
        <ul>
          <li><p><b>편집</b></p>
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
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>포트폴리오 ID</b></li>
          <li><b>programID
          </b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 저널 게시물(JRNL)

JournalEntry 개체는 특정 개체 필드에 대한 정보를 해당 필드가 수정될 때마다 기록하도록 설정할 수 있습니다. 필드가 저널 게시물 개체의 일부로 기록되도록 설정되면 해당 필드를 수정할 때마다 해당 저널 게시물이 만들어집니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 수정되었습니다.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>PFM</code>(폴더 이동)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>플래그</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### 저널 필드(JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 수정되었습니다.
        <ul>
          <li>
            <p><b>작업</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>PFM</code>(폴더 이동)</p>
              </li>
              </ul>
         </li>
         </ul>
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
          <li><b>actualWorkRequired</b><p>다음 플래그가 추가되었습니다.
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">필드 검색</td>
      <td>
        <ul>
          <li><b>실제 작업</b><p>유형이 <code>null</code>에서 <code>double</code>(으)로 변경되었습니다.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">작업</td>
      <td>다음 작업이 추가되었습니다.
        <ul>
          <li><p><b>수</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>보고서</b></p>
          <li><p><b>검색</b></p>
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
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>입력자 ID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 매개변수 그룹(PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>입력자 ID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 포털 섹션(PTLSEC)

PortalSection 객체는 Report 입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>reportShareableFolder</b></li>
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
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
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
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      다음 필드가 수정되었습니다.
        <ul>
          <li><b>포트폴리오 ID</b><p>유효성 검사기 "REQUIRED"가 추가되었습니다.</li>
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
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef(QUED)

QueueDef 개체는 Workfront의 요청 큐 정의를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 가능한 값에 대한 변경 사항으로 수정되었습니다. 자세한 내용은 개발자 설명서를 참조하십시오.
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
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
      <td>다음 필드가 가능한 값을 광범위하게 변경하면서 수정되었습니다. 자세한 내용은 개발자 설명서를 참조하십시오.
        <ul>
          <li><b>형식</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 작업(작업)

작업 객체는 최종 목표 달성(프로젝트 완료)의 일환으로 완료해야 하는 작업 항목을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>추가됨</p></li>
          <li><p><b>actualWorkRequired</b></p><p><code>AUTO_LOAD</code> 및 <code>DYNAMIC</code> 플래그를 추가했습니다.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>추가됨</p>
          </li>
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
      <td>엔터프라이즈 스토리지 관리를 지원하기 위해 다음 필드가 추가되었습니다.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>다음 필드가 수정되었습니다.
        <ul>
          <li>
            <p><b>작업</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### 사용자(사용자)

사용자 개체는 로그인하여 시스템과 상호 작용할 수 있는 Workfront의 계정을 가진 사용자를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>다음 필드가 제거되었습니다.
        <ul>
          <li><b>사용자 위치</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





