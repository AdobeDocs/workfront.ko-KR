---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 17의 새로운 기능
description: Adobe Workfront은 2022년 4월 6일에 API 버전 17을 출시했습니다. API 버전 17에는 버전 15의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 1%

---

# API 버전 17의 새로운 기능

Adobe Workfront은 2023년 10월 12일에 API 버전 17을 출시했습니다. API 버전 17에는 버전 16의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

<!--

### Booking (BOOKNG)

-->

### ExternalDocument(EXTDOC)

ExternalDocument 객체는 Workfront 외부의 문서 스토리지 공급자에 있는 문서 또는 기타 디지털 에셋입니다. 이러한 에셋은 Workfront에서 또는 와 연결할 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li><p><b>날짜 수정</b></p></li>
          <li><p><b>설명</b></p></li>
          <li><p><b>문서 공급자 ID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>이름</b></p></li>
          <li><p><b>경로</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>읽기 전용</b></p></li>
          <li><p><b>크기</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li><p><b>날짜 수정</b></p></li>
          <li><p><b>설명</b></p></li>
          <li><p><b>문서 공급자 ID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>이름</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>경로</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>읽기 전용</b></p></li>
          <li><p><b>크기</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>값</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">기본 필드</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>이름</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMeta</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">쿼리</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocument</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li><p><b>검색</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation(USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li><p><b>분류자 ID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
        <ul>
          <li><p><b>고객</b></p></li>
          <li><p><b>사용자</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## 제거된 리소스

API 버전 17에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

API 버전 17에 대해 다음 리소스가 수정되었습니다.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### 기준선(BLIN)

기준선은 특정 시점의 프로젝트 성능에 대한 스냅샷입니다. 여기에는 주요 날짜, 진행 상황, 비용 및 수익 값과 같은 프로젝트에 대한 주요 정보가 저장됩니다.

기준 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

### BillingRecord(BILL)

BillingRecord 개체는 청구할 수 있는 수익, 시간 또는 비용을 기록합니다. 이 정보는 외부 회계 시스템에서 송장을 생성하는 데 사용할 수 있습니다.

BillingRecord 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### 회사(CMPY)

Company 객체는 사람들의 컬렉션으로 구성된 조직을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>제거됨</p>
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
            <p>가능한 값 "config.defaultToNewHomeDescription"(customer:config.defaultToNewHome)&gt;/p를 추가했습니까?<p>이를 통해 조직에서는 새 홈 환경을 사용자의 기본값으로 설정할 수 있습니다.</p>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>가능한 값 "Frame.io"(FRAMEIO)가 추가되었습니다.</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>가능한 값 "enum.filetype.site"(site)가 추가되었습니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 환율(환율)

ExchangeRate 개체는 Workfront에서 설정된 통화 환율을 나타냅니다. Exchange 개체가 동적이지 않습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>다음 필드가 추가되었습니다.
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>추가됨.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### 경비(EXPNS)

경비는 프로젝트 수명 동안 발생할 수 있는 비인적 비용을 나타냅니다.

경비 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

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
            <p><b>defaultInterface</b>
            </p>
            <p>제거됨</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 시간(시간)

Hour 개체는 타임시트에 사용자가 기록한 시간을 나타냅니다.

Hour 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

### 반복(ITRN)

Iteration 객체는 단일 애자일 반복을 나타냅니다. 반복은 애자일 스토리를 계획하고 완료하는 데 사용되는 이산 기간입니다.

반복 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.


### 저널 게시물(JRNL)

JournalEntry 개체는 특정 개체 필드에 대한 정보를 해당 필드가 수정될 때마다 기록하도록 설정할 수 있습니다. 필드가 저널 게시물 개체의 일부로 기록되도록 설정되면 해당 필드를 수정할 때마다 해당 저널 게시물이 만들어집니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>승인자 추가됨(AAA)</li>
              <li>추가된 검토자(AAR)</li>
              <li>제거된 검토자(ARR)</li>
              <li>승인자 제거됨(ARA)</li>
              <li>승인된 결정 (ADA)</li>
              <li>변경 사항과 함께 승인된 결정(ADC)</li>
              <li>의사 결정에는 (AND) 작업이 필요합니다.</li>
              <li>취소된 결정(ADR)</li>
              <li>승인자 변경됨(AAC)</li>
              <li>검토자 변경됨(ARC)</li>
              <li>검토 완료(RDC)</li>
              <li>리뷰가 취소되었습니다(RDR).</li>
              <li>Publish (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 칸반 보드(KNBNBD)

Kanban 보드는 애자일 환경에서 작업을 추적하는 데 사용됩니다.

Kanban 보드 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.


### LinkedFolder(LNKFDR)

LinkedFolder 개체는 Google 드라이브 또는 Dropbox과 같은 외부 문서 공급자로부터 연결된 폴더를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>가능한 값 "Frame.io(FRAMEIO)"가 추가되었습니다.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / 문제 (OPTASK)

OpTask 객체를 일반적으로 문제라고 합니다. 문제는 일반적으로 작업 또는 프로젝트의 완료를 방해하는 문제가 있음을 나타내는 작업 항목입니다. 문제는 헬프 데스크 요청일 수도 있습니다. 변경 주문, 요청 및 버그도 문제가 됩니다.

Issue 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

### 프로젝트(프로젝트)

프로젝트는 Workfront 내의 작업 항목이며 Workfront이 작업을 수행하는 데 도움을 주는 방식의 주요 빌딩 블록입니다. Project 개체는 일반적인 특정 목표를 가진 작업 그룹을 나타냅니다.

프로젝트 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

### 프로젝트 사용자(PRTU)

ProjectUser 개체는 특정 프로젝트와 관련된 사용자를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### 비율(비율)

요금 오브젝트는 Workfront에서의 청구 요금을 나타냅니다.

Rate 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">액션</td>
      <td>비율 카드 기능을 지원하기 위해 다음 작업이 추가되었습니다.
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p><b>setRatesForRole</b> 작업이 다음 필드를 추가하도록 수정되었습니다.
        <ul>
        <li>분류자 ID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 위험(위험)

위험 개체는 프로젝트가 정시 또는 예산 내에서 완료되지 않을 수 있는 가능한 이벤트를 나타냅니다. 작업 승인 전에 잠재적인 장애 요소를 식별하기 위해 계획 단계에서 프로젝트에 위험이 추가됩니다.

위험 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

### 역할/작업 역할(역할)

역할 객체(작업 역할)는 Designer 또는 제품 관리자와 같이 사용자가 채울 수 있는 기능 역량 또는 스킬 세트를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>제거됨</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 작업(작업)

작업 객체는 최종 목표 달성(프로젝트 완료)을 위한 단계로 수행해야 하는 작업 항목을 나타냅니다.

작업 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

### 팀(TEAOB)

팀 개체는 작업 항목에 할당할 수 있는 사용자 컬렉션입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>제거됨</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 팀원(TEAMMB)

TeamMember 개체는 특정 팀과 연결된 사용자입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 템플릿 사용자(TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
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
      <td role="rowheader">직접 필드</td>
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
            <p><b>changeType</b>
            </p>
            <p>다음 값이 추가되었습니다.</p>
            <ul>
              <li>추가된 승인자(assetapprovalAddApprover)</li>
              <li>추가된 검토자(assetapprovalAddReviewer)</li>
              <li>제거된 승인자(assetapprovalRemoveApprover)</li>
              <li>제거된 검토자(assetapprovalRemoveReviewer)</li>
              <li>결정 승인됨(assetapprovalDecisionApproved)</li>
              <li>의사 결정에 필요한 작업(assetapprovalDecisionNeedsWork)</li>
              <li>변경 사항과 함께 승인된 결정(assetapprovalDecisionApprovedChanges)</li>
              <li>취소된 결정(assetapprovalDecisionRevoced)</li>
              <li>승인자 변경됨(assetapprovalApproverChanged)</li>
              <li>검토자 변경됨(assetapprovalReviewerChanged)</li>
              <li>검토 완료(assetapprovalReviewerDecisionComplete)</li>
              <li>리뷰가 취소됨(assetapprovalReviewerDecisionRevocated)</li>
              <li>외부 문서 전송 오류(externalDocumentSendError)</li>
              <li>문서 버전이 게시됨(documentVersionPublish)</li>
              <li>연결된 폴더 워크플로(linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### 사용자(사용자)

사용자 개체는 로그인하여 시스템과 상호 작용할 수 있는 Workfront의 계정을 가진 사용자를 나타냅니다.

사용자 개체가 **INLINE_EDITABLE** 플래그를 제거했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>작업 시간</b>
            </p>
            <p>이 필드가 추가되었으며, 0에서 1 사이의 숫자로, 사용자가 매일 프로젝트 작업(오버헤드가 아닌 작업)에 소비할 수 있는 시간의 백분율을 나타냅니다. 값 1은 사용자가 프로젝트 작업에 시간을 100% 사용할 수 있음을 의미합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 사용자 그룹(USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote(USRNOT)

UserNote 객체는 알림입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>다음 값이 추가되었습니다.</p>
            <ul>
              <li>문서에 귀하의 승인이 필요합니다(AAA)</li>
              <li>문서에 검토 필요(AAR)</li>
              <li>문서에 더 이상 귀하의 승인이 필요하지 않습니다(ARA).</li>
              <li>문서에 더 이상 귀하의 검토(ARR)가 필요하지 않습니다.</li>
              <li>문서에 (사용자의) 승인 필요(ATA)</li>
              <li>문서 요구(사용자) 검토(ATR)</li>
              <li>문서에 더 이상 (사용자)의 승인(RTA)이 필요하지 않음</li>
              <li>문서에 더 이상 (사용자)의 검토(RTR)가 필요하지 않음</li>
              <li>문서 승인됨(ADA)</li>
              <li>변경 사항과 함께 승인된 문서(ADC)</li>
              <li>문서에 작업(AND) 필요</li>
              <li>(사용자)가 (문서)를 승인됨으로 표시했습니다. 더 이상 승인이 필요하지 않습니다. (AAN)</li>
              <li>(사용자)가 (문서)를 변경 사항과 함께 승인됨으로 표시했습니다. 더 이상 승인이 필요하지 않습니다. (ACN)</li>
              <li>(사용자)이(문서가) 필요한 작업이라고 표시했습니다. 더 이상 승인이 필요하지 않습니다. (AWN)</li>
              <li>문서에 승인이 아닌 검토가 필요합니다(AAC).</li>
              <li>문서에 검토(AND)가 아닌 지금 사용자의 승인이 필요합니다.</li>
              <li>검토된 문서(RDC)</li>
              <li>검토된 문서(TRC)</li>
              <li>(사용자)가 (문서)를 완료된 것으로 검토했습니다. 더 이상 검토할 필요가 없습니다. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole(USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
