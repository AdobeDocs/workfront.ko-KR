---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 사용자 정의 양식의 오브젝트 유형 삭제
description: 기존 사용자 정의 양식에서 해당 양식과 연결된 오브젝트 유형을 삭제할 수 있습니다. 이 작업을 수행하면 사용자는 더 이상 해당 유형의 오브젝트에 양식을 첨부할 수 없습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 사용자 정의 양식의 오브젝트 유형 삭제

{{form-designer-default}}

기존 사용자 정의 양식에서 해당 양식과 연결된 오브젝트 유형을 삭제할 수 있습니다. 이 작업을 수행하면 사용자는 더 이상 해당 유형의 오브젝트에 양식을 첨부할 수 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 사용자 정의 양식의 오브젝트 유형 삭제

기존 사용자 정의 양식에서 오브젝트 유형을 삭제할 수 있습니다.

사용자 정의 양식에는 하나 이상의 오브젝트 유형이 있어야 합니다.

>[!CAUTION]
>
>사용자가 삭제하려는 유형의 객체에 사용자 정의 양식을 이미 첨부하고 해당 객체에 데이터를 추가한 경우, 양식에서 해당 객체 유형을 삭제하면 해당 데이터가 영구적으로 삭제됩니다. 여기에는 사용자가 나중에 필요로 하는 이전 정보가 포함될 수 있습니다.
>
>일반적으로 이미 사용 중인 사용자 정의 양식을 편집하는 횟수를 최소화하는 것이 좋습니다. 사용자 정의 양식을 사용하는 사람에게 변경 사항을 알리는 알림 시스템이 없습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 편집할 사용자 정의 양식을 선택한 다음 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
1. 양식에서 삭제할 **개체 형식**&#x200B;의 X를 클릭한 다음 표시되는 경고 메시지에서 **삭제**&#x200B;를 클릭합니다.

   ![](assets/click-x-object-types.jpg)

1. (선택 사항) 양식에서 제거할 다른 객체 유형에 대해 이전 단계를 반복합니다.
1. **완료**&#x200B;를 클릭한 다음 **저장 후 닫기**&#x200B;를 클릭합니다.
