---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Workfront 내에서 오브젝트를 한 환경에서 다른 환경으로 이동
description: 환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 트랜잭션 개체를 이동하는 기능은 지원하지 않습니다(제한된 예외 사항 포함).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 0cc1ab3a7412b7200ddab1a789ef5e9d86c3949f
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 2%

---

# Workfront 환경 간 객체 이동 개요(환경 프로모션)

환경 홍보 기능을 사용하면 한 Workfront 환경에서 다른 환경으로 개체를 이동할 수 있습니다. 예를 들어, 테스트하는 것이 조직의 실제 데이터에 영향을 주지 않는다는 것을 알고 템플릿을 만들어 샌드박스 환경에서 구성할 수 있습니다. 템플릿을 구성하고 테스트한 후 사용할 수 있도록 프로덕션 환경으로 이동할 수 있습니다.

이 프로세스를 &quot;환경 프로모션&quot;이라고 합니다.

이동할 개체 패키지를 만든 다음 새 환경에 해당 패키지를 설치하여 Workfront에서 이 프로세스를 수행할 수 있습니다.

* Workfront 내에서 이 프로세스를 수행하는 방법에 대한 특정 지침은 다음을 참조하십시오.

   * [환경 프로모션 패키지 만들기 또는 편집](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [환경 프로모션 패키지 설치](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Workfront API를 통해 이 프로세스를 수행하는 방법에 대한 지침은 [API를 사용하여  [!DNL Workfront] 환경 간에 개체 이동](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md)을 참조하십시오. [!DNL Workfront] 

[이 기능의 비디오 데모 보기](https://video.tv.adobe.com/v/3429735/){target=_blank}

## 환경 프로모션을 위해 지원되는 오브젝트

환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 프로젝트, 팀 또는 사용자 정의 양식과 같이 구성할 수 있는 개체입니다.

환경 프로모션은 객체 구성을 다루므로 트랜잭션 객체(자주 변경되거나 사용 사례에 크게 의존하는 객체)는 포함되지 않습니다. 트랜잭션 개체의 예로는 문서, 문제, 요청, 업데이트 및 증명 결정이 있습니다.

* [작업 오브젝트](#work-objects)
* [보고 개체](#reporting-objects)
* [사용자 지정 데이터 개체](#custom-data-objects)
* [조직 개체](#organization-objects)
* [기타 구성 객체](#other-configuration-objects)


### 작업 오브젝트

| 프로모션 가능 개체 | 포함된 프로모션 가능 연결된 오브젝트 |
| --- | --- |
| 프로젝트(프로젝트) | 프로젝트<br>작업<br>할당<br>전임 작업<br>회사<br>재정의 비율<br>그룹<br>역할<br>팀<br>승인 프로세스<br>승인 경로<br>승인 단계<br>단계 승인자<br>일정<br>비근무일<br>대기열 정의<br>대기열 주제 그룹<br>대기열 주제<br>라우팅 규칙<br>마일스톤 경로<br>마일스톤<br>시간 유형<br>리소스 풀<br>범주<br>범주<br>매개변수<br>매개변수 group<br>매개 변수 옵션<br>범주 표시 논리 |
| 템플릿(TMPL) | 템플릿<br>템플릿 작업<br>템플릿 작업 할당<br>템플릿 작업 전임 작업<br>회사<br>재정의 비율<br>그룹<br>역할<br>팀<br>승인 프로세스<br>승인 경로<br>승인 단계<br>단계 승인자<br>일정<br>비근무일<br>대기열 정의<br>대기열 주제 그룹<br>대기열 주제<br>라우팅 규칙<br>마일스톤 경로<br>마일스톤<br>시간 유형<br>리소스 풀<br>범주<br>범주<br>매개변수 매개 변수<br>매개 변수 그룹<br>매개 변수 옵션<br>범주 표시 논리 |

### 보고 개체

| 프로모션 가능 개체 | 포함된 프로모션 가능 연결된 오브젝트 |
| --- | --- |
| 레이아웃 템플릿(UITMPL) | 레이아웃 템플릿<br>대시보드<br>캘린더<br>캘린더 섹션<br>외부 페이지<br>보고서<br>필터<br>그룹화<br>보기<br>매개 변수<br>그룹 |
| 대시보드(PTLTAB) | 대시보드<br>캘린더<br>캘린더 섹션<br>외부 페이지<br>보고서<br>필터<br>그룹화<br>보기<br>매개 변수 |
| 달력(달력) | 달력<br>달력 섹션 |
| 외부 페이지(EXTSEC) | 외부 페이지 |
| 보고서(PTLSEC) | 보고서<br>필터<br>그룹화<br>보기<br>매개 변수 |
| 필터(UIFT) | 필터<br>매개 변수 |
| 그룹화(UIGB) | 그룹화<br>매개 변수 |
| 보기(UIVW) | <br>매개 변수 보기 |

### 사용자 지정 데이터 개체

| 프로모션 가능 개체 | 포함된 프로모션 가능 연결된 오브젝트 |
| --- | --- |
| 범주(CTGY) | 범주<br>범주 매개 변수<br>매개 변수<br>매개 변수 그룹<br>매개 변수 옵션<br>범주 표시 논리<br>그룹 |
| 매개 변수(매개 변수) | Parameter<br>Parameter 옵션 |
| 매개변수 그룹(PGRP) | 매개변수 그룹 |

### 조직 개체

| 프로모션 가능 개체 | 포함된 프로모션 가능 연결된 오브젝트 |
| --- | --- |
| 그룹(그룹) | 그룹 <br>하위 그룹(최대 5개 수준) *<br>범주<br>범주 매개 변수<br>매개 변수<br>매개 변수 그룹<br>매개 변수 옵션<br>범주 표시 논리 |
| 역할(역할) | 역할 |
| 팀(팀) | 팀<br>그룹 |
| 회사(CMPY) | 회사<br>재정의 비율<br>범주<br>범주 매개 변수<br>매개 변수<br>매개 변수 그룹<br>매개 변수 <br>범주 표시 논리<br>그룹 |
| Portfolio(포트) | Portfolio<br>프로그램<br>그룹<br>범주<br>범주 매개변수<br>매개변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |
| 프로그램(PRGM) | 프로그램<br>Portfolio<br>그룹<br>범주<br>범주 매개변수<br>매개변수<br>매개변수 그룹<br>매개변수 옵션<br>범주 표시 논리 |

### 기타 구성 객체

| 프로모션 가능 개체 | 포함된 프로모션 가능 연결된 오브젝트 |
| --- | --- |
| 승인 프로세스(ARVPRC) | 승인 프로세스<br>승인 경로<br>승인 단계<br>단계 승인자<br>역할<br>팀<br>그룹 |
| 일정(일정) | 일정<br>비근무일<br>그룹 |
| 마일스톤 경로(MPATH) | 마일스톤 경로<br>마일스톤 |
| 타임시트 프로필(TSPRO) | 타임시트 프로필<br>시간 유형 |
| 시간 유형(시간) | 시간 유형 |
| 경비 유형(EXPTYP) | 경비 유형 |
| 위험 유형(RSKTYP) | 위험 유형 |
| 리소스 풀(RSPL) | 리소스 풀 |
| 액세스 수준(ACSLVL) | 액세스 수준 |
| 등급 카드(RTCRD) | 요율 카드 |
| 위치/분류자(CLSF) | 위치/분류자 |
| 비즈니스 규칙(BSNRUL) | 비즈니스 규칙 |

\* 현재 사용할 수 없음

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## 환경 프로모션 상태

환경 프로모션 패키지는 환경 간에 이동할 수 있도록 생성되고 준비되는 동안 여러 상태를 통해 진행됩니다. Workfront 내의 패키지 목록 또는 Workfront API를 사용하는 경우 API 응답에서 이러한 상태를 볼 수 있습니다.

이러한 상태는 다음과 같습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>조립되지 않음</td> 
   <td><p>이 상태는 자동으로 지정되며, 저장되었지만 아직 조립되지 않은 패키지를 나타냅니다. </p><p>이 상태는 사용자가 직접 설정할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>어셈블</td> 
   <td><p>이 상태는 객체가 어셈블되는 동안 자동으로 지정됩니다. </p><p>어셈블링은 패키지에 포함할 객체와 하위 객체를 식별하고 해당 객체와 해당 데이터를 패키지에 추가하는 자동화된 프로세스를 말합니다.</p><p>이 상태는 사용자가 직접 설정할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>초안</td> 
   <td><p>이 상태는 어셈블리 프로세스가 끝날 때 또는 빈 프로모션 패키지를 생성할 때 지정됩니다.</p><p>사용자가 프로모션 패키지를 다시 이 상태로 이동할 수 있습니다.</p><p>이 상태에서는 환경 내에서 프로모션 패키지를 설치할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>테스트</td> 
   <td><p>이 상태를 사용하면 프로모션 패키지를 미리보기 또는 사용자 정의 새로 고침 샌드박스에 설치할 수 있습니다. 이 상태에서는 프로덕션에 패키지를 설치할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>활성</td> 
   <td><p>이 상태를 사용하면 프로덕션을 포함한 모든 환경에 프로모션 패키지를 설치할 수 있습니다.</p><p>패키지 상태가 활성으로 설정되면 <code>publishedAt</code> 날짜가 요청의 현재 타임스탬프로 자동 설정됩니다.</p></td> 
  </tr> 
  <tr> 
   <td>비활성화됨</td> 
   <td><p>이 상태는 나중에 환경에 설치되지 않는 이전에 사용한 프로모션 패키지를 숨기는 데 사용됩니다.</p><p>패키지가 이 상태일 때는 환경에 설치할 수 없습니다.</p><p>패키지 상태가 DISABLED로 설정되면 <code>retiredAt</code> 날짜가 요청의 현재 타임스탬프로 자동 설정됩니다.</p><p><code>DELETE /package</code> 끝점은 검색할 수 있고 이 패키지로 만든 배포에 대해 설치 기록이 유지되므로 이 상태를 사용하는 것이 좋습니다.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>ASSEMBLING 단계가 실패할 경우 프로모션 패키지가 자동으로 이 상태로 전환됩니다.</p><p>패키지를 ASSEMBLING 스테이지로 되돌리려면 어셈블 프로세스를 다시 트리거해야 합니다.</p><p>패키지 조립에 대한 자세한 내용은 환경 프로모션 패키지 만들기 또는 편집 문서에서 <a href="https://experienceleague.adobe.com/ko/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">기존 패키지 편집 또는 조립</a> 섹션을 참조하십시오.</td> 
  </tr> 
  </tbody> 
</table>

## 리소스

* 환경 프로모션에 대한 FAQ는 [환경 프로모션 FAQ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)를 참조하십시오.
* 문제 해결 권장 사항은 [환경 프로모션 문제 해결](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)을 참조하십시오.


