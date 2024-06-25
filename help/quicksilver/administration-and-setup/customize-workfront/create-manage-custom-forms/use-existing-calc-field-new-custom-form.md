---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 기존 양식 빌더를 사용하여 사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용
description: 다른 오브젝트에 속한 사용자 정의 양식에서 동일한 계산된 사용자 정의 필드를 사용할 수 있습니다. 예를 들어 작업 사용자 정의 양식에서 프로젝트 사용자 정의 양식에 대해 생성한 Profit 계산 필드를 사용할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 기존 양식 빌더를 사용하여 사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용

{{form-designer-default}}

다른 오브젝트에 속한 사용자 정의 양식에서 동일한 계산된 사용자 정의 필드를 사용할 수 있습니다. 예를 들어 작업 사용자 정의 양식에서 프로젝트 사용자 정의 양식에 대해 생성한 Profit 계산 필드를 사용할 수 있습니다.

계산된 사용자 정의 필드를 사용자 정의 양식에 추가하는 방법에 대한 자세한 내용은 [기존 양식 빌더로 계산된 데이터를 사용자 정의 양식에 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

기존의 계산된 사용자 정의 필드를 사용할 때 계산이 새 양식으로 전송되지 않습니다. 새 사용자 정의 양식에 동일한 필드에 계산을 다시 추가해야 합니다.

>[!TIP]
>
>다음에 저장된 계산을 사용할 때입니다 **지침** 사용자 정의 양식의 필드가 도움이 됩니다.

새 양식에서 동일한 필드에 대해 다른 계산을 사용할 수도 있습니다. 계산된 사용자 정의 필드에 대해 동일한 이름을 유지하면 명명 규칙에서 일관성과 일관성이 보장됩니다.

>[!IMPORTANT]
>
>계산된 사용자 정의 필드는 시간이 지남에 따라 오래된 것이 될 수 있습니다. 이러한 필드에서 항상 최신 계산을 보려면 다음 중 하나를 수행합니다.
>
>* 첨부된 사용자 정의 양식에서 데이터를 편집한 개체를 저장한 후 기타 아이콘을 클릭합니다 ![](assets/more-icon.png) 개체의 기본 페이지에서 사용자 정의 표현식을 다시 계산합니다.
>* 개체를 일괄 편집할 때 [사용자 정의 표현식 다시 계산] 옵션을 선택합니다.
>* 사용자 정의 양식에서 계산된 사용자 정의 필드를 편집할 때 이전 계산 업데이트 옵션을 선택합니다.
>
