---
navigation-topic: get-started-with-workfront
title: 우선 순위를 사용하여 작업 필터링 및 그룹화
description: 필터를 사용하여 원하는 작업을 찾은 다음 그룹화를 적용하여 체계적으로 관리할 수 있습니다.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 75396c3f066abc6070ae2a89c2ded0255dbc0751
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 6%

---


# 우선 순위를 사용하여 작업 필터링 및 그룹화

필터를 사용하여 원하는 작업을 찾은 다음 그룹화를 적용하여 체계적으로 관리할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> 
   <p>현재: 요청 이상</p>
   <p>새로운 기능: 기여자 이상</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>업데이트가 있는 오브젝트에 대한 보기 또는 편집 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>오브젝트에 대한 액세스 보기</p></td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 필터링

자신에게 할당된 작업 및 문제를 필터링할 수 있습니다.

{{step1-to-priorities}}

1. 작업 목록 오른쪽 상단의 **필터**&#x200B;를 클릭합니다.
1. 하나 이상의 필터를 선택하여 작업 항목 범위를 좁힙니다.
   ![](assets/filters.png)

+++을 확장하여 사용 가능한 필터에 대한 자세한 정보 확인
<table>
  <tbody>
   <tr>
   <th>필터</th>
   <th>설명</th>
   </tr>
    <tr>
      <td>처리 중</td>
      <td>현재 작업 중인 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>시작 준비 완료</td>
      <td>항목이 있는 항목 표시 
      <ul>
      <li>완료되지 않은 전임 작업 또는 작업 제한 없음</li>
      <p>및</p>
      <li>계획된 시작 일자가 과거 또는 최대 2주 미래입니다.</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>준비 안 됨</td>
      <td>다음과 같은 항목이 있는 항목 표시
       <ul>
      <li>항목이 작업되지 않도록 하는 불완전한 전임 작업 또는 작업 제한</li>
      <p>또는</p>
      <li>2주 이상 후의 계획된 시작 일자</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>요청됨</td>
      <td>작업을 시작하지 않은 문제를 표시합니다.</td>
    </tr>
      <td>완료</td>
      <td>지난 2주 이내에 완료된 작업을 표시합니다. 이 필터 옵션에는 승인이 포함되지 않습니다.</td>
    </tr>
    <tr>
    <td>프로젝트</td>
    <td>할당된 작업 또는 문제가 포함된 프로젝트를 표시합니다.</td>
    </tr>
    <tr>
    <td>기한</td>
    <td>계획된 완료 일자별 작업 표시</td>
    </tr>
    <tr>
    <td>상태</td>
    <td>작업 또는 문제를 신규, 진행 중 및 완료 상태로 표시</td>
    </tr>
    <tr>
    <td>내 포커스</td>
    <td>포커스 수준이 할당된 의 작업 또는 문제를 표시합니다. 포커스 수준은 개별 사용자가 할당 및 관리합니다.</td>
    </tr>
  </tbody>
</table>

+++

1. (선택 사항) 선택을 재설정하려면 **기본값으로 돌아가기**&#x200B;를 클릭합니다.

## 내 작업 그룹화

{{step1-to-priorities}}

1. 작업 목록 오른쪽 상단의 **그룹**&#x200B;을 클릭합니다.
1. 작업 목록을 구성할 그룹 선택
   ![](assets/groups.png)

+++을 확장하여 사용 가능한 그룹에 대한 자세한 정보 보기

| 그룹 | 설명 |
|-----------|-------------|
| 없음 | 그러면 작업 목록에서 그룹화가 제거됩니다. |
| 내 포커스 | 할당된 포커스 수준에 따라 항목을 그룹화합니다. |
| 주 마감일 | 기한이 있는 주를 기준으로 항목을 그룹화합니다. 계획된 완료 일자에 의해 납기 일자가 결정됩니다. |
| 상태 | 신규, 진행 중, 완료 상태로 항목을 그룹화합니다. <br>참고: 지금은 우선 순위에서 사용자 지정 상태를 사용할 수 없습니다. |
| 프로젝트 | 프로젝트별로 항목을 그룹화합니다. |

+++

## 작업 정렬

작업을 정렬하려면 **그룹**&#x200B;을 열고 **오름차순 정렬** 또는 **내림차순 정렬**&#x200B;을 클릭하세요.

![](assets/expand-sort-groups.png)

>[!IMPORTANT]
>
>그룹을 적용한 경우에는 정렬 옵션을 일시적으로 사용할 수 없습니다.



## 모든 섹션 확장 또는 축소

모든 섹션을 확장하거나 축소하려면 **그룹**&#x200B;을 열고 **모두 확장** 또는 **모두 축소**&#x200B;를 클릭합니다.

![](assets/expand-sort-groups.png)


