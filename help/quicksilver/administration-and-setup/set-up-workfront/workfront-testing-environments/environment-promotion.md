---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 한 환경에서 다른 환경으로 개체 이동
description: 환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 트랜잭션 개체를 이동하는 기능은 지원하지 않습니다(제한된 예외 사항 포함).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '2304'
ht-degree: 3%

---

# 한 개체에서 개체 이동 [!DNL Workfront] 환경을 다른 환경에

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 플랜</td> 
   <td> <p>Enterprise, Prime 또는 Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 라이센스</p> </td> 
   <td> <p>[!UICONTROL 계획] </p> <p>다음이어야 합니다: [!DNL Workfront] 관리자. 다음에 대한 정보: [!DNL Workfront] 관리자, 참조 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">개체 권한</p> </td> 
   <td> <p>모두</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">지원 패키지</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] 또는 [!UICONTROL Enterprise]</p> <p>표준 지원 패키지는 사용자 정의 새로 고침 샌드박스에 액세스할 수 없지만 미리보기 샌드박스에 액세스할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건

프로모션 패키지 만들기 엔드포인트는 사용자가 이미 소스 환경을 구성했다고 가정합니다. 이 API 호출을 사용하려면 의 개체 맵을 수동으로 만들어야 합니다. [!DNL Workfront] objCodes 및 개체 GUID입니다. 이 지도의 구체적인 구조는 아래에 설명되어 있습니다.

## 환경 프로모션을 위해 지원되는 오브젝트

환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 트랜잭션 개체를 이동하는 기능은 지원하지 않습니다(제한된 예외 사항 포함).

* [작업 오브젝트](#work-objects)
* [보고 개체](#reporting-objects)
* [사용자 지정 데이터 개체](#custom-data-objects)
* [조직 개체](#organization-objects)
* [기타 구성 객체](#other-configuration-objects)


### 작업 오브젝트

| 프로모션 가능 개체 | 포함된 프로모션 가능한 하위 오브젝트 |
| --- | --- |
| 프로젝트(프로젝트) | 프로젝트<br>작업<br>할당<br>전임 작업<br>회사<br>오버라이드 비율<br>그룹<br>역할<br>팀<br>승인 진행<br>승인 경로<br>승인 단계<br>단계 승인자<br>예약<br>비근무일<br>대기열 정의<br>대기열 주제 그룹<br>대기열 주제<br>라우팅 규칙<br>마일스톤 경로<br>마일스톤<br>시간 유형<br>리소스 풀<br>범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |
| 템플릿(TMPL) | 템플릿<br>템플릿 작업<br>템플릿 작업 할당<br>템플릿 작업 전임 작업<br>회사<br>오버라이드 비율<br>그룹<br>역할<br>팀<br>승인 진행<br>승인 경로<br>승인 단계<br>단계 승인자<br>예약<br>비근무일<br>대기열 정의<br>대기열 주제 그룹<br>대기열 주제<br>라우팅 규칙<br>마일스톤 경로<br>마일스톤<br>시간 유형<br>리소스 풀<br>범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |

### 보고 개체

| 프로모션 가능 개체 | 포함된 프로모션 가능한 하위 오브젝트 |
| --- | --- |
| 레이아웃 템플릿(UITMPL) | 레이아웃 템플릿<br>대시보드<br>캘린더<br>달력 섹션<br>외부 페이지<br>보고서<br>필터<br>그룹화<br>보기<br>매개 변수 |
| 대시보드(PTLTAB) | 대시보드<br>캘린더<br>달력 섹션<br>외부 페이지<br>보고서<br>필터<br>그룹화<br>보기<br>매개 변수 |
| 달력(달력) | 캘린더<br>달력 섹션 |
| 외부 페이지(EXTSEC) | 외부 페이지 |
| 보고서(PTLSEC) | 보고서<br>필터<br>그룹화<br>보기<br>매개 변수 |
| 필터(UIFT) | 필터<br>매개 변수 |
| 그룹화(UIGB) | 그룹화<br>매개 변수 |
| 보기(UIVW) | 보기<br>매개 변수 |

### 사용자 지정 데이터 개체

| 프로모션 가능 개체 | 포함된 프로모션 가능한 하위 오브젝트 |
| --- | --- |
| 범주(CTGY) | 범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리<br>그룹 |
| 매개 변수(매개 변수) | 매개 변수<br>매개변수 옵션 |
| 매개변수 그룹(PGRP) | 매개변수 그룹 |

### 조직 개체

| 프로모션 가능 개체 | 포함된 프로모션 가능한 하위 오브젝트 |
| --- | --- |
| 그룹(그룹) | 그룹 <br>하위 그룹(최대 5개 수준) *<br>범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |
| 역할(역할) | 역할 |
| 팀(팀) | 팀<br>그룹 |
| 회사(CMPY) | 회사<br>오버라이드 비율<br>범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개 변수 <br>범주 표시 논리<br>그룹 |
| Portfolio(포트) | Portfolio<br>프로그램<br>그룹<br>범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |
| 프로그램(PRGM) | 프로그램<br>Portfolio<br>그룹<br>범주<br>범주 매개변수<br>매개 변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |

### 기타 구성 객체

| 프로모션 가능 개체 | 포함된 프로모션 가능한 하위 오브젝트 |
| --- | --- |
| 승인 프로세스(ARVPRC) | 승인 진행<br>승인 경로<br>승인 단계<br>단계 승인자<br>역할<br>팀<br>그룹 |
| 일정(일정) | 예약<br>비근무일<br>그룹 |
| 마일스톤 경로(MPATH) | 마일스톤 경로<br>마일스톤 |
| 타임시트 프로필(TSPRO) | 타임시트 프로필<br>시간 유형 |
| 시간 유형(시간) | 시간 유형 |
| 경비 유형(EXPTYP) | 경비 유형 |
| 위험 유형(RSKTYP) | 위험 유형 |
| 리소스 풀(RSPL) | 리소스 풀 |

\* 현재 사용할 수 없음

## 인증

API는 각 요청을 인증하여 클라이언트가 요청된 개체를 보거나 수정할 수 있는 액세스 권한을 보유하는지 확인합니다.

인증은 다음 방법을 사용하여 제공할 수 있는 세션 ID 또는 API 키를 전달하여 수행됩니다.

### 요청 헤더 인증

기본 인증 방법은 세션 토큰이 포함된 SessionID라는 요청 헤더를 전달하는 것입니다. 이는 안전하다는 장점이 있다 [CSRF(크로스 사이트 요청 위조)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) 캐싱을 위해 URI를 공격하고 방해하지 않습니다.

다음은 요청 헤더의 예입니다.

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API 엔드포인트

* [패키지 만들기](#create-a-package)
* [패키지 목록 가져오기](#get-a-list-of-packages)
* [ID로 패키지 가져오기](#get-a-package-by-id)
* [패키지의 특정 속성 업데이트](#update-specific-properties-of-a-package)
* [패키지 삭제](#delete-a-package)
* [사전 실행](#execute-a-pre-run)
* [설치 실행](#execute-an-installation)
* [특정 패키지에 대한 설치 목록 가져오기](#get-a-list-of-installations-for-a-specific-package)
* [설치에 대한 설치 세부 정보 가져오기](#get-the-installation-details-for-an-installation)

### 패키지 만들기

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 여러 단계 프로세스를 실행합니다.

첫 번째 단계는 &quot;ASSEMBLING&quot; 상태의 빈 프로모션 패키지를 만드는 결과를 초래합니다.

두 번째 단계에서는 `objectCollections` Workfront에서 요청된 레코드를 어셈블하기 위해 POST 본문에 제공되는 배열입니다. 요청한 레코드 수와 Workfront 구성에 따라 이 단계를 완료하는 데 몇 분이 걸릴 수 있습니다. 이 프로세스가 끝나면 빈 프로모션 패키지가 `packageEntities` 상태가 자동으로 &quot;초안&quot;으로 설정됩니다.


>[!NOTE]
>
>의 구조를 확인합니다. `objectCollections`  배열입니다.
>
>배열의 각 항목에는 `objCode` Workfront API 탐색기에 문서화된 개체 코드에 해당하는 키입니다.
>
>각 항목에는 `entities` 컬렉션. 이는 다음을 예상합니다. `ID` 필드. 선택 사항도 사용할 수 있습니다 `name` 을(를) 보다 쉽게 알 수 있도록 하는 속성 `ID` 를 나타냅니다.
>
>에서 요청할 수 있는 개체 코드 목록 `objectCollections` list, see the [환경 프로모션을 위해 지원되는 오브젝트](#supported-objects-for-environment-promotion) 이 문서의 섹션.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### 헤더

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

또는

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 본문

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### 응답

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
}
```

### 패키지 목록 가져오기

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 고객에 속한 프로모션 패키지의 필터링되지 않은 목록을 반환합니다.

응답에는 고객의 샌드박스, 미리보기 또는 Workfront의 프로덕션 인스턴스에서 만든 모든 패키지가 포함됩니다.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### 헤더

```json
{
    "apikey": "**********"
}
```

또는

```json
{
    "sessionID": "*****************"
}
```

#### 본문

_비어 있음_

#### 응답

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—위의 &quot;상태&quot;를 확인하십시오. 추가되었습니까?—>

### ID로 패키지 가져오기

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 요청된 프로모션 패키지의 세부 정보를 반환합니다.

프로모션 패키지의 원래 소스와 관계없이 모든 환경을 통해 요청을 수행할 수 있습니다.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 헤더

```json
{
    "apikey": "**********"
}
```

또는

```json
{
    "sessionID": "*****************"
}
```

#### 본문

_비어 있음_

#### 응답

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 패키지의 특정 속성 업데이트

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 PATCH 본문에 제공되는 프로모션 패키지의 콘텐츠를 업데이트합니다.

편집 가능한 속성은 다음과 같습니다.

1. 이름(문자열)
1. 설명(문자열)
1. 상태(값 유효성 검사가 포함된 문자열)

상태 옵션에는 다음이 포함됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>어셈블</td> 
   <td><p>이 상태는 객체가 어셈블되는 동안 자동으로 지정됩니다.</p><p>이 상태는 고객이 직접 설정할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>초안</td> 
   <td><p>이 상태는 어셈블리 프로세스가 끝날 때 또는 빈 프로모션 패키지를 생성할 때 지정됩니다.</p><p>고객이 프로모션 패키지를 다시 이 상태로 이동할 수 있습니다.</p><p>이 상태에서는 프로모션 패키지를 환경에 설치할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>테스트</td> 
   <td><p>이 상태를 사용하면 프로모션 패키지를 미리보기 또는 사용자 정의 새로 고침 샌드박스에 설치할 수 있습니다. 이 상태에서는 프로덕션에 패키지를 설치할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>활성</td> 
   <td><p>이 상태를 사용하면 프로덕션을 포함한 모든 환경에 프로모션 패키지를 설치할 수 있습니다.</p><p>패키지 상태를 활성으로 설정하면 <code>publishedAt</code> 날짜는 요청의 현재 타임스탬프로 자동 설정됩니다.</p></td> 
  </tr> 
  <tr> 
   <td>비활성화됨</td> 
   <td><p>이 상태는 나중에 환경에 설치되지 않는 이전에 사용한 프로모션 패키지를 숨기는 데 사용됩니다.</p><p>패키지가 이 상태일 때는 환경에 설치할 수 없습니다.</p><p>패키지 상태를 사용 안 함으로 설정하면 <code>retiredAt</code> 날짜는 요청의 현재 타임스탬프로 자동 설정됩니다.</p><p>이 상태를 사용하는 것이 을(를) 사용하는 것보다 좋습니다.<code>DELETE /package</code> 끝점은 검색할 수 있고 설치 기록이 이 패키지로 만든 배포에 대해 보존되기 때문입니다.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>ASSEMBLING 단계가 실패할 경우 프로모션 패키지가 자동으로 이 상태로 전환됩니다.</p><p>패키지를 ASSEMBLING 단계로 되돌리려면 추출 프로세스를 다시 트리거해야 합니다.</p></td> 
  </tr> 
  </tbody> 
</table>


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### 헤더

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

또는

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 본문

```json
{
    "status": "ACTIVE"
}
```

#### 응답

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 패키지 삭제

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 프로모션 패키지 레코드를 삭제합니다. 이 작업은 취소할 수 없습니다.

>[!NOTE]
>
>프로모션 패키지를 삭제하는 대신 패키지의 상태를 DISABLED로 변경하는 것이 좋습니다. 이렇게 하면 패키지를 검색할 수 있고 패키지가 배포된 위치의 설치 기록을 유지할 수 있습니다.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 헤더

```json
{
    "apikey": "**********"
}
```

또는

```json
{
    "sessionID": "*****************"
}
```

#### 본문

_비어 있음_

#### 응답

```
200
```

```
Deleted
```

### 사전 실행

>[!IMPORTANT]
>
>설치를 실행하려면 먼저 이 사전 실행을 실행해야 합니다. 설치를 실행할 때 이 호출에서 생성된 ID를 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 패키지 정의와 URL에서 식별된 대상 환경 간의 비교를 수행합니다.

결과는 프로모션 개체가 대상 환경에서 발견되었는지 여부를 식별하는 JSON 본문입니다.

각 프로모션 개체에 대해 다음 중 하나를 수행합니다 `actions`  이(가) 설정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>만들기</td> 
   <td><p>대상 환경에서 해당 레코드를 찾을 수 없는 경우 작업이 CREATE로 설정됩니다.</p><p>이 작업을 다음에서 설정하면 <code>translationmap</code> 에 제공됩니다. <code>/install</code> 끝점은 설치 서비스가 레코드를 만듭니다.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>대상 환경에서 해당 레코드를 찾으면 작업은 USEEXISTING으로 설정되고 <code>targetId</code> 에도 캡처됩니다. <code>translationmap</code>.</p><p>이 작업을 다음에서 설정하면 <code>translationmap</code> 에 제공됩니다. <code>/install</code> 끝점입니다. 설치 서비스가 레코드를 만들지 않습니다. 그러나 는 <code>targetId</code> 이 레코드에 대한 참조가 있을 수 있는 다른 객체에 대한 맵 항목에 포함됩니다.</p><p>예를 들어 패키지를 배포하는 대상 환경에서 "기본 그룹"을 찾을 수 있습니다. 두 개의 "기본 그룹" 레코드를 가질 수 없으므로 설치 서비스는 프로젝트, 양식 또는 이 그룹과 관련된 다른 엔티티와 같은 "기본 그룹"에 대한 참조를 포함하는 다른 개체 만들기 작업에서 기존 그룹에 대한 GUID를 사용합니다.</p><p><b>참고:</b> <ul><li><p>USEEXISTING 작업이 지정되면 대상 환경의 기존 레코드는 수정되지 않습니다. </p><p>예를 들어 패키지를 빌드한 샌드박스에서 "기본 그룹"에 대한 설명이 변경되고 설명 값이 타겟 환경에서 다른 경우 이 값은 설치 후에도 변경되지 않습니다 <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>무시</td> 
   <td><p>이 작업은 자동으로 설정되지 않습니다.</p><p>CREATE 또는 USEEXISTING 작업을 실행하기 전에 수동으로 재정의하는 기능을 제공합니다. <code>/install</code> 호출합니다.</p><p><b>메모: </b><ul><li><p>원래 CREATE로 설정되었던 레코드가 IGNORE로 설정된 경우 모든 하위 레코드도 IGNORE로 설정해야 합니다.</p><p>예를 들어 템플릿 레코드가 CREATE 작업과 매핑되었는데 설치 사용자가 이 레코드를 배포에서 제외하려는 경우 템플릿의 작업을 IGNORE로 설정할 수 있습니다.</p><p>이 경우 설치 사용자가 템플릿 작업, 템플릿 작업 할당, 템플릿 작업 전임 작업, 대기열 정의, 대기열 주제, 라우팅 규칙 등도 IGNORE로 설정하지 않으면 배포가 설치 시도에 실패하게 됩니다.</p></li><li><p>원래 USEEXISTING으로 설정된 레코드가 IGNORE로 설정된 경우 설치 과정에서 일부 부작용이 발생할 수 있습니다.</p><p>예를 들어, 그룹 레코드가 USEEXISTING 작업으로 매핑되고 설치 사용자가 작업을 IGNORE로 변경하면 그룹이 필요한 객체(예: 할당된 그룹이 없으면 프로젝트가 존재할 수 없음)에 대해 시스템 기본 그룹이 해당 프로젝트에 할당됩니다.</p></li><li><p>원래 USEEXISTING으로 설정된 레코드가 CREATE로 설정된 경우 많은 Workfront 엔티티에서 고유한 이름 제약 조건이 있으므로 설치 프로세스 중에 몇 가지 부작용이 있을 수 있습니다.</p><p>예를 들어, "기본 그룹" 레코드가 USEEXISTING 작업과 매핑되어 있고, "기본 그룹"이 이미 있으므로 설치 사용자가 작업을 CREATE로 변경하면 설치 시도에서 모든 단계를 완료하지 못합니다. 그룹 이름은 고유해야 합니다.</p><p>일부 엔티티에 고유 이름 제약 조건이 없습니다. 이러한 객체에 대해 이 변경 작업을 수행하면 동일한 이름의 레코드가 두 개 생성됩니다. 예를 들어 템플릿, 프로젝트, 보기, 필터, 그룹화, 보고서 및 대시보드에는 고유한 이름 제약 조건이 필요하지 않습니다. 이러한 레코드에 고유한 이름을 사용하는 것이 가장 좋지만 강제 적용되지는 않습니다.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

현재 업데이트를 지원하지 않습니다. `action` 을 참조하십시오. 업데이트를 허용하는 옵션 `action` 우리가 연구하고 있는 거야.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### 헤더

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

또는

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 본문

```json
{}
```

#### 응답

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>설치를 실행하는 데 필요한 ID는 `id` 필드. 이 예에서는 `id` 필드는 맨 위에서 세 번째이며 다음 값으로 시작하는 값이 있습니다. `c0bc79bd`.

### 설치 실행

>[!IMPORTANT]
>
>설치를 실행하려면 먼저 사전 실행을 실행해야 합니다. 설치를 실행할 때 사전 실행에서 생성된 ID를 사용합니다.
>
>사전 실행을 실행한 후 대상 환경(패키지를 배포 중인 환경)이 변경된 경우 사전 실행을 다시 실행하는 것이 좋습니다. 사전 실행을 다시 실행하지 않으면 실행이 정확하게 완료되지 않거나 설치에 실패할 수 있습니다.
>
>사전 실행 실행에 대한 지침은 다음을 참조하십시오. [사전 실행](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 POST URL에서 식별된 대상 환경에 프로모션 패키지의 설치 시도를 시작합니다.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### 헤더

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

또는

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 본문

```json
{
}
```

#### 응답

```
202
```


```json
{}
```

### 특정 패키지에 대한 설치 목록 가져오기

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

결과에는 패키지가 배포된 모든 환경의 설치 이벤트가 포함됩니다. 이는 요청이 수행되는 환경에 대한 설치로 제한되지 않습니다. 이를 통해 이 패키지를 수신한 환경을 식별할 수 있습니다.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### 헤더

```json
{
    "apikey": "**********"
}
```

또는

```json
{
    "sessionID": "*****************"
}
```

#### 본문

_비어 있음_

#### 응답

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### 설치에 대한 설치 세부 정보 가져오기

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

이 호출은 최종 값을 반환합니다. `translationMap` 특정 설치를 위해 설치 서비스에서 생성합니다.

각 기록에는 처방된 내용이 명시됩니다 `action` 이(가) 및 해당 작업의 성공 여부를 나타냅니다.

CREATE가 있는 레코드 `action` 다음 `targetId` 필드는 대상 시스템에서 새로 만든 레코드의 값으로 설정됩니다. 또한 `installationStatus` 필드가 설치됨으로 설정됩니다.

USEEXISTING이 있는 레코드 `action` 다음 `targetId` 필드도 설정되고 `installationStatus` 필드가 등록됨으로 설정됩니다. 이것은 매핑 프로세스가 완료되었으며 설치 서비스가 레코드를 평가했으며 처리할 사항이 없음을 인정함을 의미합니다.

레코드에 CREATE가 있는 경우 `action` 그러나 레코드를 성공적으로 만들지 못한 다음 `installationStatus` 이 실패로 설정되고 실패 이유도 제공됩니다.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### 헤더

```json
{
    "apikey": "**********"
}
```

또는

```json
{
    "sessionID": "*****************"
}
```

#### 본문

_비어 있음_

#### 응답

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
