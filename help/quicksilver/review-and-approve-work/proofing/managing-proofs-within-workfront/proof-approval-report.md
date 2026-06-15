---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명 승인 보고서 사용
description: 증명 승인 보고서를 사용하여 환경에서 증명에 대한 정보를 볼 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
TQID: https://experienceleague.adobe.com/ZU6Ej5QhI7v9zoAxurBz1YsFVIuVIh2a8tR2h6vYL18
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a2241fa21f51f8146c1f3725d2ba2235f8458ab4
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 6%

---

# 증명 승인 보고서 사용

증명 승인 보고서를 사용하여 환경에서 증명에 대한 정보를 볼 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront 패키지</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 라이선스</p> </td> 
   <td> 
   <p>표준</p>
   <p>플랜</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>액세스 수준 구성</strong> </td> 
   <td> <p>액세스 권한 편집 대상:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 캘린더 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 증명 승인 보고서 사용

{{step1-to-reports}}

1. **새 보고서**&#x200B;를 클릭한 다음 스크롤하여 **증명 승인**&#x200B;을 선택합니다.

   ![증명 승인 보고서](assets/proof-approval-report.png)

1. (선택 사항) 추가 필드를 추가합니다.
1. **저장 및 닫기**&#x200B;를 클릭합니다.

## 추가 필드

증명 승인 보고서에 다음 필드를 추가할 수 있습니다.

* **결정 날짜**: 증명에 대한 승인자의 결정 날짜를 표시합니다. 증명의 인쇄 요약에서도 이 날짜를 확인할 수 있습니다.
* **승인자 단계**: 현재 단계 정보를 표시합니다.
* **워크플로 템플릿**: 증명에 첨부된 모든 워크플로 템플릿을 표시합니다. 첨부된 템플릿이 없으면 열이 비어 있습니다.
* **결정 대기 중**: 다음 조건이 참일 때 최신 버전에서 결정이 충족되지 않았음을 나타내기 위해 true를 표시합니다.

   * 증명이 보관되지 않음
   * 승인자가 진행 중인 단계가 활성 상태입니다.
   * 증명이 승인 보류 중입니다.

* **증명 기한**: 증명 기한을 표시합니다. 이 필드를 채우려면 모든 단계에 기한이 할당되어야 합니다. 필드에는 가장 최근에 활성화된 단계의 기한이 표시됩니다.

## 승인자 결정 필드 정보

승인자 결정 필드에는 증명에 대한 수신자의 결정이 표시됩니다. 경우에 따라 이 필드에 결정 값 대신 하이픈(-)이 표시되는데, 이는 수신자가 증명에서 더 이상 결정 역할에 있지 않음을 나타냅니다. 자세한 내용은 증명 승인 보고서에서 [승인자 결정에 하이픈이 표시됨](../tips-tricks-and-troubleshooting/approver-decision-shows-hyphen.md)을 참조하세요.

 
