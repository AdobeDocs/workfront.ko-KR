---
title: 작업 공간 템플릿 목록
description: 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에는 작업 영역을 구축할 때 기본 레코드 유형 및 필드를 시작하기 위한 템플릿 세트가 포함되어 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c4758b87-45dc-4ffd-b086-5e2e907bdf34
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fo6vWjL0XWOPzrBDUC02ES9kgnzmlTGsi050JUfz3zk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 958
ht-degree: 6%

---

# 작업 공간 템플릿 목록

{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다.

Workfront Planning에는 작업 영역을 구축할 때 기본 레코드 유형 및 필드를 시작하기 위한 템플릿 세트가 포함되어 있습니다. 작업 영역 만들기에 대한 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

이 문서에서는 Adobe Workfront Planning에서 사용할 수 있는 작업 공간 템플릿에 대해 설명합니다.

## Adobe Workfront Planning 템플릿에 대한 고려 사항

* Planning 작업 공간 템플릿을 사용할 때 만드는 작업 공간의 수에 따라 다음 유형의 템플릿을 사용할 수 있습니다.

   * 단일 템플릿: 하나의 템플릿이 하나의 작업 공간을 만듭니다.
   * 다중 작업 영역 템플릿 번들: 템플릿 번들은 서로 연결된 6개의 작업 영역을 만듭니다.
* 각 템플릿에는 레코드 유형 세트가 있습니다.

  자세한 내용은 [레코드 종류 개요](/help/quicksilver/planning/architecture/overview-of-record-types.md)를 참조하세요.
* 각 템플릿의 레코드 유형은 구성된 섹션으로 구성되어 있습니다.
* 각 레코드 종류에는 필드 집합이 포함되어 있습니다. 이러한 필드 중 일부는 다른 Workfront Planning 레코드 유형에 대한 연결입니다.
* 템플릿을 사용하여 작업 공간을 만들 수 있으며, 작업 공간이 만들어지면 이를 사용자 정의하고 레코드 유형, 필드, 레코드 및 보기를 추가한 다음 다른 사용자와 공유할 수 있습니다.
* 각 템플릿의 레코드 유형에는 예제 레코드가 포함되어 있습니다. 템플릿에서 작업 공간을 작성한 후 삭제할 수 있습니다.
* 템플릿에서 작업 영역이 생성되면 작업 영역 관리자는 레코드 유형, 필드, 보기 및 레코드를 삭제할 수 있습니다.


<!--
 I modeled this article by the "List of available Blueprints" and that articles does not have an Access area

## Access requirements

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--
the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="././administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Planning area in your layout template. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

-->

## 단일 Workfront Planning 작업 공간 템플릿

다음은 Workfront Planning의 작업 공간 템플릿과 여기에 포함된 레코드 유형입니다.

* **Operations Initiative Studio**: 통합 이니셔티브(Workfront의 자동화된 SOL 연결)를 계획하고 제공하는 방법을 보여 주는 완벽하고 탐색할 준비가 된 운영 이니셔티브 모델입니다. 이니셔티브에서 워크스트림으로의 분류, 연결된 위험, 문제 및 결정, 지원 참조 목록(팀, 시스템), 타임라인, 테이블 및 달력 보기, 간단한 작업 공식이 포함되어 있어 팀이 Planning 기능을 빠르게 학습할 수 있습니다.

  Operations Initiative Studio 템플릿에는 다음 레코드 종류 및 해당 필드가 포함되어 있습니다.

   * 이니셔티브
   * 워크스트림
   * 위험 및 문제
   * 결정
   * 시스템
   * 팀
* **Communications Planning Studio**: 통신 계획 허브를 빠르게 설정하는 것이 좋습니다. 긴 통신 계획 또는 짧은 통신 계획 템플릿 레코드를 복제한 다음 전술을 추가하고 승인 체크포인트를 추적하여 롤아웃을 작성합니다. 일관된 보고, 필터링 및 재사용을 위해 대상, 시장 및 채널을 참조하십시오. 샘플 레코드와 즉시 사용할 수 있는 테이블, 타임라인 및 달력 보기를 포함하여 팀이 Planning 기능을 즉시 탐색할 수 있습니다.

  Communications Planning Studio 템플릿에는 다음 레코드 유형과 해당 필드가 포함되어 있습니다.

   * 커뮤니케이션
   * 대상자
   * 전술
   * 승인 체크포인트
   * 채널
   * 시장
   * 관련자 역할

* **기본: 마케팅 관리**: 기본 마케팅 시스템의 기반을 구축하는 조직에 이상적입니다. 템플릿에는 다음 레코드 종류 및 다른 레코드 종류에 연결된 필드를 포함한 필드 수가 포함됩니다.

   * 캠페인
   * 페르소나
   * 브랜드
   * 제품

* **고급: 마케팅 관리**: 더 세밀한 마케팅 전략을 탐색할 준비가 된 팀에 적합합니다. 템플릿에는 다음 레코드 종류 및 다른 레코드 종류에 연결된 필드를 포함한 필드 수가 포함됩니다.

   * 캠페인
   * 프로그램
   * 지역
   * 고객 여정 단계
   * 대상자
   * 결과물
   * 브랜드

* **엔터프라이즈: 마케팅 관리**: 마케팅 시스템이 복잡한 대규모 조직 또는 성숙 조직을 위해 설계되었습니다. 템플릿에는 다음 레코드 종류 및 다른 레코드 종류에 연결된 필드를 포함한 필드 수가 포함됩니다.

   * 캠페인
   * 프로그램
   * 전술
   * 활동
   * 제품
   * 결과물
   * Target 대상
   * 지역
   * 하위 영역
   * 파트너
   * 사용 사례
   * 고객 여정 단계

* 판매 관리: 판매 프로세스를 간소화하고 효율성을 향상시키는 포괄적인 판매 시스템을 만들 수 있습니다. 템플릿에는 다음 레코드 종류 및 다른 레코드 종류에 연결된 필드를 포함한 필드 수가 포함됩니다.

   * 기회
   * 활동
   * 캠페인
   * 계정
   * 리드
   * 연락처
   * 지역
   * 업계
   * 구매 센터
   * 제품/서비스
   * 경쟁


* 제품 관리: 이 템플릿을 사용하여 효율적이고 구조화된 제품 관리 프로세스를 만들 수 있습니다. 템플릿에는 다음 레코드 종류 및 다른 레코드 종류에 연결된 필드를 포함한 필드 수가 포함됩니다.

   * 테마
   * 이니셔티브
   * Epic
   * 사용자 스토리
   * 고객
   * Sprint
   * 제품 팀
   * 기능 요청
   * 업계

## 다중 작업 공간 Workfront Planning 작업 공간 템플릿

모범 사례 다중 작업 영역 템플릿 번들을 사용하여 6개의 작업 영역을 동시에 만들 수 있습니다.

다음 사항을 고려하십시오.

* 이 번들에서 템플릿을 하나만 선택할 수는 없습니다.
* 6개의 작업 공간을 모두 한 번에 만들어야 하며, 이때 사용하지 않을 수 있는 작업 공간은 삭제할 수 있습니다.

다중 작업 영역 템플릿 번들에는 해당 레코드 유형과 함께 다음 템플릿이 들어 있습니다.

* 1.**전역 분류 및 분류**: Fréscopa의 핵심 공유 레코드 및 분류의 기업 거버넌스를 위한 허브입니다. 모든 시스템과 팀 간의 일관성, 정렬 및 표준화를 보장합니다.

  >[!NOTE]
  >
  >우리는 기업의 일반적인 예로 &quot;Fréscopa&quot;라는 이름을 사용합니다.


   * 고객 여정
   * 국가
   * 채널
   * 지역
   * 주, 시/도 또는 현
   * 언어
   * 플랫폼
   * 경험 유형
   * 년
   * 분기
   * 메시징 전략
   * Target 대상
   * 페르소나
   * 제품
   * 브랜드
   * 제품 범주
   * 값
   * 비전과 사명
   * 기둥
   * 주요 성과 지표

* **2.Fréscopa 글로벌 마케팅**: Fréscopa의 엔터프라이즈 마케팅 전략 및 실행을 관리하기 위한 중앙 집중식 작업 영역입니다. 캠페인, 콘텐츠 및 지표를 종합하여 브랜드 효과를 높입니다.

   * 캠페인
   * 채널 전술
   * 경험
   * 이벤트

* **3.Fréscopa 소셜 마케팅**: Fréscopa의 소셜 미디어 상태 및 캠페인을 관리하기 위한 전용 작업 영역입니다. 모든 소셜 플랫폼에서 계획, 게시 및 성능 추적을 중앙 집중화합니다.

   * 인플루언서

* **4.Fréscopa Media &amp; PR**: 미디어 및 PR 팀이 글로벌 마케팅 목표를 지원하기 위해 활동을 조정하는 곳입니다.

   * 리포터
   * 미디어 아울렛
   * 미디어 참여

* **5.Fréscopa 글로벌 이벤트**: 모든 지역, 국가 및 사업부에서 Fréscopa 이벤트를 계획하고 추적할 수 있는 중앙 위치입니다.

   * 이벤트 유형
   * 작업 스트림 유형
   * 스피커
   * 이벤트 위치
   * 이벤트 대상 유형

* **6.Fréscopa Executive Company Leadership**: 전략적 리더가 엔터프라이즈 목표 및 목표와 같은 실행 가능한 데이터와 인터페이스할 수 있는 중앙 집중식 작업 영역입니다.

   * 엔터프라이즈 목표
   * 부서 목표
   * 팀 목표
   * 핵심 결과

