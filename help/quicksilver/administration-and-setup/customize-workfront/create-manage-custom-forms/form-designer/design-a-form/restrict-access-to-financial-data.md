---
title: 사용자 정의 필드에서 재무 데이터에 대한 액세스 제한
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 지정 필드를 만들 때 재무 데이터에 대한 액세스를 제한하는 선택적 설정을 정의할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 5cdaccd9381b02f183b837208eaac4389b0b7a24
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 6%

---


# 사용자 정의 필드에서 재무 데이터에 대한 액세스 제한

{{highlighted-preview-article-level}}

사용자 지정 필드를 만들 때 재무 데이터에 대한 액세스를 제한하는 선택적 설정을 정의할 수 있습니다. 이렇게 하면 액세스 수준에 설정된 특정 권한이 있는 사용자가 데이터를 볼 수 있으며 액세스 권한이 없어야 하는 재무 데이터를 볼 수 없습니다.

사용자 지정 필드 만들기에 대한 자세한 내용은 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

액세스 수준에 대한 자세한 내용은 [액세스 수준 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)를 참조하세요. 공유 및 사용 권한에 대한 자세한 내용은 [개체에 대한 공유 사용 권한 개요](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td>Any</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>사용자 정의 양식에 대한 관리 액세스</td> 
  </tr>  
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 필드의 재무 데이터에 대한 액세스 제한

1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다.

   자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. 양식에 사용자 정의 필드를 추가하거나 기존 필드를 선택합니다.

   다음 필드 유형은 재무 데이터 액세스에 따라 제한될 수 있습니다.

   * 한 줄 텍스트
   * 단락
   * 단일 선택 드롭다운
   * 다중 선택 드롭다운
   * 확인란 그룹
   * 라디오 버튼
   * 외부 조회
   * 다중 선택 외부 조회
   * 계산됨

1. **형식** 필드에서 **통화**&#x200B;를 선택합니다.

   >[!NOTE]
   >
   >계산된 필드의 경우 모든 형식이 허용됩니다. 다른 모든 필드 형식은 **통화** 형식을 사용해야 합니다. 그렇지 않으면 **재무 권한 형식** 필드를 사용할 수 없습니다.

1. (선택 사항) 계산된 필드에만 **자동 권한** 옵션을 켜면 수식의 필드에서 재무 권한이 자동으로 부여됩니다.

1. **재무 권한 유형**&#x200B;에 대한 옵션을 선택하십시오.

   양식에서 이 사용자 정의 필드를 보거나 편집하려면 먼저 사용자에게 이 재무 권한 유형이 있어야 합니다.

   * **권한 필요 없음:** 모든 사용자가 이 필드를 볼 수 있음
   * **일반:** 사용자는 일반 금융을 편집하거나 볼 수 있는 권한이 있어야 합니다.
   * **청구:** 사용자에게 청구 요율을 편집하거나 볼 수 있는 권한이 있어야 합니다.
   * **비용:** 사용자가 비용 비율을 편집하거나 볼 수 있는 권한이 있어야 합니다.

   계산된 필드의 경우:

   * **자동 권한** 필드가 켜져 있는 경우 **재무 권한 유형** 필드를 사용 권한의 수동 설정에 사용할 수 없습니다.
   * 수식에 사용되는 필드는 권한 필드의 활성 여부를 결정합니다. 권한 필드가 비어 있고(자동 권한이 설정되지 않은 경우) 공식의 필드가 재무 권한을 지원하지 않습니다.
   * 수식의 모든 필드에 대한 액세스 권한이 필요합니다. 예를 들어 계산된 필드에서 두 개의 필드가 사용되고 그 중 하나에 청구 권한이 적용되고 두 번째에 비용 권한이 적용되는 경우 계산된 값을 보려면 사용자에게 청구 및 비용 요금을 모두 볼 수 있는 권한이 있어야 합니다.

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 양식을 계속 빌드하세요.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

## 예

두 개의 프로젝트가 사용자와 공유됩니다.

* 사용자는 첫 번째 프로젝트에서 모든 재무 옵션을 편집할 수 있습니다.
* 사용자는 두 번째 프로젝트에 대한 청구 요금 및 일반 재무 정보를 볼 수 있는 권한이 있습니다

사용자가 첫 번째 프로젝트를 편집하면 사용자 정의 양식의 모든 재무 필드를 편집할 수 있습니다. 사용자가 두 번째 프로젝트를 편집할 때 **청구** 또는 **일반**(으)로 설정된 필드는 보기 전용이며 **비용**(으)로 설정된 필드는 표시되지 않습니다.

사용자가 목록 또는 보고서에서 프로젝트를 볼 때:

* 재무 필드는 권한 및 보고서 설정에 따라 보거나 편집할 수 있습니다.
* 사용자에게 재무 필드를 볼 수 있는 권한이 없는 경우 재무 필드가 비어 있음

프로젝트 세부 정보를 내보내면 목록과 동일한 재무 필드 값(또는 빈 필드)이 표시됩니다.

두 프로젝트를 모두 벌크 편집할 때 청구 및 일반 재무 필드는 읽기 전용으로 표시되고 비용 필드에는 해당 없음이 표시됩니다.

