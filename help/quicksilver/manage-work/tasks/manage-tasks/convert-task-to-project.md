---
product-area: projects
navigation-topic: manage-tasks
title: 작업을 프로젝트로 변환
description: 프로젝트의 작업에 원래 계획했던 것보다 많은 작업이 필요한 경우 프로젝트로 변환할 수 있습니다.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 작업을 프로젝트로 변환

프로젝트의 작업에 원래 계획했던 것보다 많은 작업이 필요한 경우 프로젝트로 변환할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>템플릿을 사용하여 프로젝트로 변환할 때 템플릿에 대한 보기 또는 더 높은 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>템플릿을 사용하여 프로젝트로 변환하는 경우 템플릿에 대한 권한 보기</p> <p>프로젝트를 만든 후 프로젝트에 대한 관리 권한이 있습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업을 프로젝트로 변환하는 데 대한 고려 사항

* 원래 작업이 삭제됩니다.
* 작업 승인이 삭제됩니다.
* 모든 하위 작업, 문제 및 참고는 새 프로젝트에 롤업됩니다.
* 문서, 문서 버전 및 증명을 새 프로젝트로 이동합니다.
* 모든 하위 작업 및 문제의 상태 및 완료율이 유지됩니다.
* 작업의 공유 사용자는 프로젝트의 공유 사용자가 됩니다.
* 프로젝트 시작 날짜가 작업의 시작 날짜로 설정됩니다.
* 작업 상태가 &#39;신규&#39;이면 프로젝트 상태가 &#39;계획&#39;으로 설정됩니다.
* 작업 상태가 &#39;진행 중&#39;이면 프로젝트 상태는 &#39;현재&#39;로 설정됩니다.
* 작업 상태가 &#39;완료&#39;이면 프로젝트 상태는 &#39;완료&#39;로 설정됩니다.

## 작업을 프로젝트로 변환

1. 프로젝트로 변환할 작업으로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 아이콘 ![](assets/more-icon.png), 그런 다음 **프로젝트로 변환**.
1. 다음 옵션 중 하나를 선택합니다.

   * **새 프로젝트**
   * 의 템플릿 **템플릿에서 선택** 섹션

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. 클릭 **계속** 표시되는 알림에 표시됩니다.
1. 에서 **프로젝트로 변환** 상자에 다음을 지정합니다.

   * **이름**: 프로젝트에 이름을 지정합니다. 기본 이름은 작업의 이름입니다.
   * (선택 사항) **설명**: 이 프로젝트의 목적을 설명합니다.
   * (선택 사항 및 조건부) 템플릿에서 프로젝트를 만들도록 선택한 경우, 의 사용 가능한 필드를 업데이트합니다 **프로젝트로 변환** 대화 상자

      프로젝트의 필드 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >프로젝트로 변환 상자의 재무 섹션에서 필드를 갱신하려면 액세스 수준에서 재무 데이터에 대한 편집 액세스 권한이 있어야 합니다. 액세스 레벨에서 재무 데이터에 대한 조회 액세스 권한이 있는 경우 템플리트의 모든 재무 정보가 새 프로젝트로 전송되며 문제를 변환하는 동안 편집할 수 없습니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 및 [템플릿 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (선택 사항) 추가 **사용자 지정 Forms** 새 프로젝트에 추가합니다.

      >[!TIP]
      작업에 첨부된 다중 개체 사용자 지정 양식이 작업과 프로젝트에서 모두 사용하도록 구성된 경우 양식에 저장된 모든 정보는 변환될 때 유지됩니다.
      변환에 템플릿을 사용하고 템플릿에 첨부된 사용자 지정 양식에 작업에 첨부된 사용자 지정 필드도 포함되어 있는 경우 작업의 필드 값이 새 프로젝트에 사용됩니다. 그러나 작업에서 사용자 지정 필드가 비어 있으면 템플릿의 값이 사용됩니다.

1. 클릭 **변경 내용 저장**.
