---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명 승인 보고서 사용
description: 증명 승인 보고서를 사용하여 환경에서 증명에 대한 정보를 볼 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 1%

---

# 증명 승인 보고서 사용

증명 승인 보고서를 사용하여 환경에서 증명에 대한 정보를 볼 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront 플랜*</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 라이선스 개요*</p> </td> 
   <td> <p>플랜</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>액세스 수준*</strong> </td> 
   <td> <p>액세스 권한 편집 대상:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 캘린더 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

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

 
