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
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '2095'
ht-degree: 2%

---

# [!DNL Workfront] 환경 프로모션 API를 사용하여 [!DNL Workfront] 환경 간에 개체 이동

환경 프로모션 기능을 사용하면 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있습니다. 이 문서에 설명된 대로 Workfront API를 사용하여 이러한 개체를 이동할 수 있습니다.

Workfront 애플리케이션을 사용하여 환경 간에 객체를 이동하는 방법에 대한 지침은 다음을 참조하십시오.

* [환경 프로모션 패키지 만들기 또는 편집](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [환경 프로모션 패키지 설치](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 계획</strong>
   </td>
   <td> Prime 또는 Ultimate(신규 계획만 해당)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront]개 라이선스</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td>[!DNL Workfront] 관리자여야 합니다.
   </td>
  </tr>
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 전제 조건

프로모션 패키지 만들기 엔드포인트는 사용자가 이미 소스 환경을 구성했다고 가정합니다. 이 API 호출에는 [!DNL Workfront] objCodes 및 개체 GUID의 개체 맵을 수동으로 만들어야 합니다. 이 지도의 구체적인 구조는 아래에 설명되어 있습니다.

## 환경 프로모션을 위해 지원되는 오브젝트

환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 트랜잭션 개체를 이동하는 기능은 지원하지 않습니다(제한된 예외 사항 포함).

승격 가능한 개체 및 포함된 승격 가능한 하위 개체 목록은 [Workfront 환경 간 개체 이동 개요](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md) 문서의 [환경 승격에 대해 지원되는 개체](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)를 참조하십시오.

## 인증

API는 각 요청을 인증하여 클라이언트가 요청된 개체를 보거나 수정할 수 있는 액세스 권한을 보유하는지 확인합니다.

인증은 다음 방법을 사용하여 제공할 수 있는 세션 ID 또는 API 키를 전달하여 수행됩니다.

### 요청 헤더 인증

기본 인증 방법은 세션 토큰이 포함된 SessionID라는 요청 헤더를 전달하는 것입니다. 이를 통해 [CSRF(크로스 사이트 요청 위조)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) 공격으로부터 안전하며 캐싱을 위해 URI를 방해하지 않는 이점이 있습니다.

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

두 번째 단계에서는 POST 본문에 제공된 `objectCollections` 배열을 사용하여 Workfront에서 요청된 레코드를 조합합니다. 요청한 레코드 수와 Workfront 구성에 따라 이 단계를 완료하는 데 몇 분이 걸릴 수 있습니다. 이 프로세스가 끝나면 빈 프로모션 패키지가 `packageEntities`(으)로 업데이트되고 상태가 자동으로 &quot;초안&quot;으로 설정됩니다.


>[!NOTE]
>
>`objectCollections` 배열의 구조를 확인합니다.
>
>배열의 각 항목에는 Workfront API 탐색기에 문서화된 개체 코드에 해당하는 `objCode` 키가 있습니다.
>
>각 항목에는 `entities` 컬렉션도 포함되어 있습니다. `ID` 필드가 필요합니다. 또한 선택적 `name` 특성을 수락하여 `ID`이(가) 나타내는 내용을 더 쉽게 알 수 있습니다.
>
>`objectCollections` 목록에서 요청할 수 있는 개체 코드 목록을 보려면 이 문서의 [환경 프로모션에 대해 지원되는 개체](#supported-objects-for-environment-promotion) 섹션을 참조하십시오.

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

사용 가능한 상태에 대한 자세한 설명은 문서 [Workfront 환경 간 개체 이동 개요](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md)의 [환경 프로모션 상태](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses)를 참조하십시오.


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

각 프로모션 개체에 대해 다음 `actions` 중 하나가 설정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>만들기</td> 
   <td><p>대상 환경에서 해당 레코드를 찾을 수 없는 경우 작업이 CREATE로 설정됩니다.</p><p>이 작업이 <code>/install</code> 끝점에 제공된 <code>translationmap</code>에서 설정되면 설치 서비스가 레코드를 만듭니다.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>대상 환경에서 해당 레코드가 발견되면 작업이 USEEXISTING으로 설정되고 <code>targetId</code>도 <code>translationmap</code>에서 캡처됩니다.</p><p>이 작업이 <code>/install</code> 끝점에 제공된 <code>translationmap</code>에서 설정되면 설치 서비스가 레코드를 만들지 않습니다. 그러나 이 레코드를 참조할 수 있는 다른 개체에 대해 맵 항목에 포함된 <code>targetId</code>을(를) 사용합니다.</p><p>예를 들어 패키지를 배포하는 대상 환경에서 "기본 그룹"을 찾을 수 있습니다. 두 개의 "기본 그룹" 레코드를 가질 수 없으므로 설치 서비스는 프로젝트, 양식 또는 이 그룹과 관련된 다른 엔티티와 같은 "기본 그룹"에 대한 참조를 포함하는 다른 개체 만들기 작업에서 기존 그룹에 대한 GUID를 사용합니다.</p><p><b>참고:</b> <ul><li><p>USEEXISTING 작업이 지정되면 대상 환경의 기존 레코드는 수정되지 않습니다. </p><p>예를 들어 패키지를 빌드한 샌드박스에서 "기본 그룹"에 대한 설명이 변경되었으며 설명 값이 대상 환경에서 다른 경우 이 <code>translationmap</code>을(를) 사용하여 설치한 후에도 값이 변경되지 않습니다.</li></ul></td> 
  </tr> 
  <tr> 
   <td>덮어쓰기</td> 
   <td><p>이 작업은 자동으로 설정되지 않습니다.</p><p>이 작업은 대상 환경에 있는 개체를 업데이트하는 기능을 제공합니다. <code>/install</code> 호출을 실행하기 전에 할당된 CREATE 또는 USEEXISTING 작업을 수동으로 재정의하는 기능을 제공합니다.<ul><li>사용자는 테스트 환경에서 개체를 업데이트한 다음 덮어쓰기 작업을 사용하여 대상 환경에서 해당 개체를 업데이트할 수 있습니다.</p></li><li><p>사용자가 처음에 프로모션 패키지를 한 개 설치한 다음 차후에 새(또는 업데이트된) 패키지에 초기 패키지의 객체에 대한 변경 사항이 포함된 경우 덮어쓰기 를 사용하여 이전에 설치한 객체를 대체(재정의)할 수 있습니다. </p><p>덮어쓰기에 대한 자세한 내용은 이 문서의 [덮어쓰기](#overwriting) 섹션을 참조하십시오.</li><ul></td> 
  </tr> 
  <tr> 
   <td>무시</td> 
   <td><p>이 작업은 자동으로 설정되지 않습니다.</p><p><code>/install</code> 호출을 실행하기 전에 할당된 CREATE 또는 USEEXISTING 작업을 수동으로 재정의하는 기능을 제공합니다.</p><p><b>참고: </b><ul><li><p>원래 CREATE로 설정되었던 레코드가 IGNORE로 설정된 경우 모든 하위 레코드도 IGNORE로 설정해야 합니다.</p><p>예를 들어 템플릿 레코드가 CREATE 작업과 매핑되었는데 설치 사용자가 이 레코드를 배포에서 제외하려는 경우 템플릿의 작업을 IGNORE로 설정할 수 있습니다.</p><p>이 경우 설치 사용자가 템플릿 작업, 템플릿 작업 할당, 템플릿 작업 전임 작업, 대기열 정의, 대기열 주제, 라우팅 규칙 등도 IGNORE로 설정하지 않으면 배포가 설치 시도에 실패하게 됩니다.</p></li><li><p>원래 USEEXISTING으로 설정된 레코드가 IGNORE로 설정된 경우 설치 과정에서 일부 부작용이 발생할 수 있습니다.</p><p>예를 들어, 그룹 레코드가 USEEXISTING 작업으로 매핑되고 설치 사용자가 작업을 IGNORE로 변경하면 그룹이 필요한 객체(예: 할당된 그룹이 없으면 프로젝트가 존재할 수 없음)에 대해 시스템 기본 그룹이 해당 프로젝트에 할당됩니다.</p></li><li><p>원래 USEEXISTING으로 설정된 레코드가 CREATE로 설정된 경우 많은 Workfront 엔티티에서 고유한 이름 제약 조건이 있으므로 설치 프로세스 중에 몇 가지 부작용이 있을 수 있습니다.</p><p>예를 들어, "기본 그룹" 레코드가 USEEXISTING 작업과 매핑되어 있고, "기본 그룹"이 이미 있으므로 설치 사용자가 작업을 CREATE로 변경하면 설치 시도에서 모든 단계를 완료하지 못합니다. 그룹 이름은 고유해야 합니다.</p><p>일부 엔티티에 고유 이름 제약 조건이 없습니다. 이러한 객체에 대해 이 변경 작업을 수행하면 동일한 이름의 레코드가 두 개 생성됩니다. 예를 들어 템플릿, 프로젝트, 보기, 필터, 그룹화, 보고서 및 대시보드에는 고유한 이름 제약 조건이 필요하지 않습니다. 이러한 레코드에 고유한 이름을 사용하는 것이 가장 좋지만 강제 적용되지는 않습니다.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

현재 이 서비스의 알파 기능에서 UPDATE `action`을(를) 지원하지 않습니다. UPDATE `action`을(를) 허용하는 옵션은 조사 중입니다.

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
>설치를 실행하는 데 필요한 ID는 `id` 필드입니다. 이 예제에서 `id` 필드는 맨 위에서 세 번째이며 `c0bc79bd`(으)로 시작하는 값을 갖습니다.

### 설치 실행

>[!IMPORTANT]
>
>설치를 실행하려면 먼저 사전 실행을 실행해야 합니다. 설치를 실행할 때 사전 실행에서 생성된 ID를 사용합니다.
>
>사전 실행을 실행한 후 대상 환경(패키지를 배포 중인 환경)이 변경된 경우 사전 실행을 다시 실행하는 것이 좋습니다. 사전 실행을 다시 실행하지 않으면 실행이 정확하게 완료되지 않거나 설치에 실패할 수 있습니다.
>
>사전 실행 실행에 대한 지침은 [사전 실행 실행](#execute-a-pre-run)을 참조하십시오.

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

이 호출은 특정 설치를 위해 설치 서비스에서 생성한 최종 `translationMap`을(를) 반환합니다.

각 레코드에는 지정된 `action`이(가) 무엇인지와 해당 작업의 성공 여부가 표시됩니다.

CREATE가 `action`인 레코드의 경우 `targetId` 필드가 대상 시스템에서 새로 만든 레코드의 값으로 설정됩니다. 또한 `installationStatus` 필드가 INSTALLED로 설정됩니다.

USEEXISTING `action`이(가) 있는 레코드의 경우 `targetId` 필드도 설정되고 `installationStatus` 필드는 REGISTERED로 설정됩니다. 이것은 매핑 프로세스가 완료되었으며 설치 서비스가 레코드를 평가했으며 처리할 사항이 없음을 인정함을 의미합니다.

레코드에 CREATE `action`이(가) 있지만 레코드를 성공적으로 만들지 못하면 `installationStatus`이(가) FAILED로 설정되고 실패 이유도 제공됩니다.

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

## 덮어쓰기

3단계 프로세스입니다.

1. 번역 맵 만들기(&quot;설치 준비&quot; 단계와 유사)
1. 생성된 번역 맵을 편집하여 덮어쓸 개체에 대해 `action` 및 `targetId` 필드를 설정합니다. 작업은 `OVERWRITING`이어야 하며 `targetId`은(는) 덮어써야 하는 개체의 UUID여야 합니다
1. 설치를 실행합니다.

* [1단계 - 번역 맵 만들기](#step-1---create-a-translation-map)
* [2단계 - 번역 맵 수정](#step-2---modify-the-translation-map)
* [3단계 - 설치](#step-3---install)

### **1단계 - 번역 맵 만들기**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### 본문

없음

#### 응답

`202 - OK` 상태의 번역 맵

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### 예

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### 2단계 - 번역 맵 수정

이 단계에 대한 끝점이 없습니다.

1. [1단계 - 번역 맵 만들기](#step-1---create-a-translation-map)에서 반환된 번역 맵에서 설치할 개체 목록을 검사하십시오.
1. 각 개체의 작업 필드를 원하는 설치 작업으로 업데이트합니다.
1. 각 개체에서 `targetId`의 유효성을 검사합니다. 설정 작업이 `USEEXISTING` 또는 `OVERWRITING`인 경우 `targetId`을(를) 대상 환경의 대상 개체의 UUID로 설정해야 합니다. 다른 모든 작업의 경우 targetId는 빈 문자열이어야 합니다.

   >[!NOTE]
   >
   >충돌이 감지된 경우 `targetId`이(가) 이미 채워져 있습니다.

### **3단계 - 설치**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### 본문

단일 필드가 `translationMap`인 개체입니다. [2단계 - 번역 맵 수정](#step-2---modify-the-translation-map)에서 수정된 번역 맵과 같아야 합니다.

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### 예

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### 응답

응답에는 `{uuid of the created installation}` 및 `202 - ACCEPTED` 상태가 포함됩니다.

예: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

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
