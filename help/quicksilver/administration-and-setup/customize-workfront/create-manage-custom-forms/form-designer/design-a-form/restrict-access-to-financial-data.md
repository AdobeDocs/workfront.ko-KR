---
title: 사용자 정의 필드에서 재무 데이터에 대한 액세스 제한
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 지정 필드를 만들 때 재무 데이터에 대한 액세스를 제한하는 선택적 설정을 정의할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 77be87f54c8745b1cdab219d9d0c5f4ea48d86e4
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 5%
---
# 사용자 정의 필드에서 재무 데이터에 대한 액세스 제한

사용자 지정 필드를 만들 때 재무 데이터에 대한 액세스를 제한하는 선택적 설정을 정의할 수 있습니다. 이렇게 하면 액세스 수준에 설정된 특정 권한이 있는 사용자가 데이터를 볼 수 있으며 액세스 권한이 없어야 하는 재무 데이터를 볼 수 없습니다.

사용자 지정 필드 만들기에 대한 자세한 내용은 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

액세스 수준 및 권한을 통해 재무 데이터에 대한 액세스를 정의하는 방법에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 및 [개체에 대한 재무 권한 공유](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)를 참조하십시오.

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

1. (선택 사항) 계산된 필드에만 **자동 권한** 옵션을 사용하면 수식의 필드에서 재무 권한을 자동으로 만들 수 있습니다.

1. **재무 권한 유형**&#x200B;에 대한 옵션을 선택하십시오.

   이 설정은 사용자가 양식에서 이 사용자 정의 필드를 보거나 편집하기 위해 보유해야 하는 액세스 및 권한 유형을 정의합니다.

   * **권한 필요 없음:** 모든 사용자는 액세스 수준 및 개체 권한에 관계없이 필드를 볼 수 있습니다.
   * **일반:** 사용자가 다음 중 하나를 가지고 있어야 필드를 볼 수 있습니다.

     * 액세스 수준에는 General Finance에 대한 액세스 권한이 활성화된 재무 데이터에 대한 보기 또는 편집 액세스 권한이 포함됩니다.
     * 사용자 정의 양식이 첨부된 객체에 대한 사용 권한에는 일반 재무 보기 또는 편집이 포함됩니다.

   * **청구서:** 사용자가 다음 중 하나를 가지고 있어야 필드를 볼 수 있습니다.

     * 액세스 수준에는 청구 요율에 대한 액세스 권한이 활성화된 재무 데이터에 대한 보기 또는 편집 액세스 권한이 포함됩니다.
     * 사용자 정의 양식이 첨부된 오브젝트에 대한 권한에는 청구 요금 보기 또는 편집이 포함됩니다.

   * **비용:** 사용자가 다음 중 하나를 가지고 있어야 필드를 볼 수 있습니다.

     * 액세스 수준에는 비용 비율에 대한 액세스 권한이 활성화된 재무 데이터에 대한 보기 또는 편집 액세스 권한이 포함됩니다.
     * 사용자 정의 양식이 첨부된 오브젝트에 대한 권한에는 원가율 보기 또는 편집이 포함됩니다.

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
