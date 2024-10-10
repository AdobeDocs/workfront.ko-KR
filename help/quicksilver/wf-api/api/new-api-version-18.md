---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 18의 새로운 기능
description: Adobe Workfront은 2022년 4월 6일에 API 버전 18을 출시했습니다. API 버전 18에는 버전 17의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# API 버전 18의 새로운 기능

Adobe Workfront은 2024년 4월 8일에 API 버전 18을 출시했습니다. API 버전 18에는 버전 17의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

API 버전 18에 대한 리소스를 추가하지 않았습니다.

## 제거된 리소스

API 버전 18에 대해 제거된 리소스가 없습니다.

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
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
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
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
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
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 승인 대기 중(AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p>다음 작업이 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>추가</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>:
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.
            <ul>
              <li>
                <p><code>NLBRCY</code> (비인적 자원 범주)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (시간)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (등급 카드)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.
            <ul>
              <li>
                <p><code>NLBRCY</code> (비인적 자원 범주)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (시간)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (등급 카드)
                </p>
              </li>
             </ul>
             </p>
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
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>다음 매개 변수가 추가되었습니다.
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>폴더로 이동</b>:
            </p>
            <p>추가됨. 이 새 작업은 다음 매개 변수를 사용합니다.
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
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
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>프로젝트 변환</b>:
            </p>
            <p>다음 필드가 추가되었습니다.
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>변환 작업</b>:
            </p>
            <p>다음 필드가 추가되었습니다.
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>추가됨.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole(PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
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
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (원가율 보기)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (청구 요금 보기)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (일반 재무 보기)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (원가율 편집)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (청구 요금 편집)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (일반 재무 편집)</p>
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
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>다음 플래그가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>동적
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>추가됨.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>프로젝트로 전환</b>
            </p>
             <p>다음 필드가 추가되었습니다.
             <ul><li><code>copyCategories</code></li></ul>
            </p>
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
      <td>
        <ul>
          <li>
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 템플릿 작업(TTSK)

TemplateTask 개체는 Template의 일부인 작업을 나타냅니다. 템플릿 작업은 템플릿이 사용되는 프로젝트의 작업이 됩니다.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole(TTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>다음 필드를 제거했습니다.
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
              </li>
             </ul>
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
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjID</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue(USERPF)

UserPrefValue 객체는 사용자 기본 설정을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>값</b>
            </p>
            <p>검사기를 추가했습니다. <code>MAX_LENGTH</code></p>
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
            <p>다음 필드가 추가되었습니다.
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>실제 청구 불가능한 경비</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

