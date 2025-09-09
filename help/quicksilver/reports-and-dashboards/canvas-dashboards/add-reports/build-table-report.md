---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 캔버스 대시보드에서 표 보고서 작성
description: 테이블 형식으로 데이터를 시각화하기 위해 캔버스 대시보드에 테이블 보고서를 추가할 수 있습니다.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 1%

---

# 캔버스 대시보드에서 표 보고서 작성

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>>가능한 버그 또는 기술 문제에 대한 피드백이 있는 경우 Workfront 지원에 티켓을 제출하십시오. 자세한 내용은 [고객 지원 센터에 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)<br>를 참조하세요.
>>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

테이블 형식으로 데이터를 시각화하기 위해 캔버스 대시보드에 테이블 보고서를 추가할 수 있습니다.

![테이블 보고서 예제](assets/table-example-main.png)

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td> 
   <td> 
<p>임의 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td> 
<p>현재: 플랜 </p> 
<p>새로운 기능: 표준</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td><p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p>
  </td> 
  </tr>  
</tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 전제 조건

테이블 보고서를 작성하려면 먼저 대시보드를 만들어야 합니다.


## 캔버스 대시보드에서 표 보고서 작성

테이블 보고서를 작성하는 데 사용할 수 있는 구성 옵션은 여러 가지가 있습니다. 이 섹션에서는 하나를 만드는 일반적인 프로세스를 안내합니다.

{{step1-to-dashboards}}

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. 오른쪽 상단의 **새 대시보드**&#x200B;를 클릭합니다.

1. **대시보드 만들기** 상자에 대시보드의 **이름** 및 **설명**&#x200B;을 입력하십시오.

1. Click **Create**.

1. **보고서 추가** 상자에서 **보고서 만들기**&#x200B;를 선택합니다.

1. 왼쪽에서 **테이블**&#x200B;을 선택합니다.

1. 오른쪽 상단 모서리에서 **보고서 만들기**&#x200B;를 클릭합니다.

1. (선택 사항) 아래 단계에 따라 **세부 정보** 섹션을 구성하십시오.

   1. 보고서 **이름**&#x200B;을(를) 입력하십시오.

   1. **설명** 보고서를 입력하십시오.

1. 아래 단계에 따라 **테이블 빌드** 섹션을 구성하십시오.

   1. 왼쪽 패널에서 **테이블 열** ![테이블 작성 아이콘](assets/drilldown-column.png) 아이콘을 클릭합니다.

   1. **열 추가**&#x200B;를 클릭한 다음 테이블에 열로 표시할 필드를 선택합니다. 오른쪽 미리보기 섹션에 열이 나타납니다.



   1. 추가할 각 열에 대해 위 단계를 반복합니다.

1. **필터** 섹션을 구성하려면 아래 단계를 따르십시오.

   1. 왼쪽 패널에서 **필터** ![필터 아이콘](assets/filter-icon.png) 아이콘을 클릭합니다.

   1. **필터 편집**&#x200B;을 선택합니다.

   1. **조건 추가**&#x200B;를 클릭한 다음 필터링할 필드와 필드가 충족해야 하는 조건 종류를 정의하는 수정자를 지정합니다. 오른쪽 미리보기 섹션에 열이 나타납니다.

1. (선택 사항) 다른 필터링 기준 집합을 추가하려면 **필터 그룹 추가**&#x200B;를 클릭합니다. 세트 사이의 기본 연산자는 AND입니다. 연산자를 클릭하여 OR로 변경합니다.

1. **드릴다운 그룹 설정** 섹션을 구성하려면 아래 단계를 따르십시오.

   1. 왼쪽 패널에서 **그룹 설정** ![그룹 설정 아이콘](assets/drilldown-group-icon.png) 아이콘을 클릭합니다.

   1. **그룹화 추가** 단추를 클릭한 다음 그룹화로 만들 필드를 선택합니다. 그룹화 열이 오른쪽의 미리보기 섹션에 나타납니다.

1. 보고서를 만들고 대시보드에 추가하려면 **저장**&#x200B;을 클릭하세요.

## 테이블 보고서 예제 작성

이 섹션에서는 보류 중인 문서 승인을 표시하는 테이블 보고서를 생성하는 단계를 살펴봅니다.

표 보고서 예에 대한 자세한 내용은 [검토 및 승인을 위한 보고서 대시보드 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)를 참조하십시오.

{{step1-to-dashboards}}

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. 오른쪽 상단의 **새 대시보드**&#x200B;를 클릭합니다.

1. **대시보드 만들기** 상자에 대시보드의 **이름** 및 **설명**&#x200B;을 입력하십시오.

1. Click **Create**.

1. **보고서 추가** 상자에서 **보고서 만들기**&#x200B;를 선택합니다.

1. 왼쪽에서 **테이블**&#x200B;을 선택합니다.

1. 오른쪽 상단 모서리에서 **보고서 만들기**&#x200B;를 클릭합니다.

1. **세부 정보** 섹션을 구성하려면 아래 단계를 따르십시오.

   1. _이름_ 필드에 **승인 보류 중**&#x200B;을(를) 입력하십시오.
   1. **설명** 필드에 설명을 입력하십시오. 이 텍스트는 차트 이름 옆에 툴팁으로 표시됩니다.

1. 아래 단계에 따라 **테이블 빌드** 섹션을 구성하십시오.

   1. 왼쪽 패널에서 **테이블 열** ![테이블 열 아이콘](assets/drilldown-column.png) 아이콘을 클릭합니다.
   1. **열 추가**&#x200B;를 클릭합니다.
   1. 아래로 스크롤하여 **문서 승인** > **상태**&#x200B;를 선택합니다.
   1. 다음 열을 추가합니다.

   <table>
    <tr>
    <td><strong>프로젝트 이름</strong></td>
    <td>문서 버전 &gt; 문서 &gt; 프로젝트 &gt; 이름</td>
    </tr>
    <tr>
    <td><strong>문서 이름</strong></td>
    <td>문서 버전 &gt; 문서 &gt; 검색 상자에 <em>이름</em>을(를) 입력하십시오.</td>
    </tr>
    <tr>
    <td><strong>문서 버전</strong></td>
    <td>문서 버전 &gt; 문서 &gt; 버전</td>
    </tr>
    <tr>
    <td><strong>마감</strong></td>
    <td>문서 승인 &gt; 승인 단계 &gt; 기한</td>
    </tr>
    <tr>
    <td><strong>요청한 사람</strong></td>
    <td>문서 승인 &gt; 승인 단계 &gt; 승인 단계 참가자* &gt; 요청자 &gt; 검색 상자에 <em>이름</em>을(를) 입력합니다.</td>
    </tr>
    <tr>
    <td><strong>요청한 날짜</strong></td>
    <td>문서 승인 &gt; 승인 단계 &gt; 승인 단계 참가자* &gt; 생성일</td>
    </tr>
    <tr>
    <td><strong>승인자</strong></td>
    <td>문서 승인 &gt; 승인 단계 &gt; 승인 단계 참가자* &gt; 참가자 사용자 &gt; 검색 상자에 <em>이름</em>을(를) 입력합니다.</td>
    </tr>
    </table>


   *승인 단계 참가자는 _승인 단계 Pa.._(으)로 잘립니다.


1. **필터** 섹션을 구성하려면 아래 단계를 따르십시오.
   1. 왼쪽 패널에서 **필터** ![필터 탭 아이콘](assets/filter-tab.png) 아이콘을 클릭합니다.
   1. **필터 편집**&#x200B;을 클릭한 다음 **조건 추가**&#x200B;를 클릭합니다.
   1. 빈 조건 필터를 클릭한 다음 **필드 선택**&#x200B;을 클릭합니다.
   1. **상태**&#x200B;를 선택하십시오.
   1. 연산자를 **Equal**(으)로 변경한 다음 텍스트 상자에 _승인 보류 중_을(를) 입력하십시오.
      ![보류 중인 승인 테이블 필터 예](assets/pending-approval-table-filter.png)
   1. (선택 사항) 아래의 **선택 필터** 섹션에 설명된 대로 필터를 더 추가합니다.
1. 화면 오른쪽 상단에서 **저장**&#x200B;을 클릭합니다.

## 테이블 보고서 작성 시 고려 사항

### 필드 선택기 활용

**테이블 작성** 섹션의 **섹션** 드롭다운은 테이블 보고서를 작성할 때 개체를 더 쉽게 찾을 수 있도록 필드 선택기에서 선택 항목의 범위를 좁히도록 설계되었습니다. 시작하려면 기본 엔티티 객체를 선택합니다.

* **모든 섹션**: Workfront Workflow 및 Workfront Planning의 모든 개체 유형.
* **Workfront 개체**: 기본 Workfront 워크플로 개체.
* **계획 레코드 종류**: Workfront Planning에 정의된 사용자 지정 레코드 종류.

![섹션 드롭다운](assets/sections-dropdown.png)

기본 엔터티 개체를 선택하면 **섹션** 드롭다운이 업데이트되며 선택할 수 있는 필드 형식 옵션이 제공됩니다.

* **모든 섹션**: 네이티브 필드, 사용자 지정 필드 및 관련 개체.
* **모든 필드**: 기본 필드와 사용자 지정 필드 모두(관계 제외).
* **사용자 정의 필드**: 사용자 정의 양식 또는 Planning 레코드의 고객 정의 필드.
* **Workfront 필드**: 기본 필드만.
* **관계**: 연결된 레코드입니다.

![보고 가능한 개체 선택](assets/reportable-objects-selection.png)

### 자식 개체 참조

추가 열, 필터 옵션 및 그룹화 속성에 대해 사용할 수 있는 관계는 일반적으로 Workfront 개체 계층 구조의 상위 개체로 제한되거나 보고서의 기본 엔티티 개체를 한 번만 선택합니다. 여기에는 다음과 같은 몇 가지 예외가 있습니다.

* 프로젝트 > 작업
* 문서 승인 > 문서 승인 단계
* 문서 승인 단계 > 문서 승인 단계 참가자

위에 나열된 상위-하위 관계를 활용하는 경우 상위 객체에 연결된 각 하위 레코드에 대한 행이 테이블에 표시됩니다.
