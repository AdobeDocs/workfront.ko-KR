---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 삭제
description: 시간이 지남에 따라 프로젝트에 대한 기록 정보를 유지할 수 있도록 템플릿을 삭제하는 대신 더 이상 사용하지 않는 템플릿을 비활성화하는 것이 좋습니다.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 프로젝트 템플릿 삭제

시간이 지남에 따라 프로젝트에 대한 기록 정보를 유지할 수 있도록 템플릿을 삭제하는 대신 더 이상 사용하지 않는 템플릿을 비활성화하는 것이 좋습니다. 템플릿 비활성화에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>템플릿을 삭제할 때 해당 템플릿을 사용하는 프로젝트는 어떤 식으로든 수정되지 않습니다. 그러나 프로젝트의 템플릿 필드에는 원본 템플릿의 이름이 더 이상 표시되지 않습니다. 또한 작업 보기에서 프로젝트의 작업에 대한 템플릿 작업 이름을 더 이상 볼 수 없습니다. 원래 프로젝트와 연관된 템플릿이 삭제된 후에는 프로젝트의 템플릿 필드와 작업의 템플릿 작업 필드가 비어 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>삭제에 대한 액세스 권한이 포함된 템플릿에 대한 액세스 편집</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>템플릿 삭제 권한이 포함된 템플릿에 대한 권한 관리</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 템플릿 삭제 시 고려 사항

* 템플릿을 첨부할 때 프로젝트에 추가된 작업은 프로젝트에 유지됩니다. 단, 작업과 연관된 템플릿 작업 정보는 삭제됩니다.
* 템플릿 이름이에 더 이상 나열되지 않음 **템플릿** 의 필드 **개요** 프로젝트의 하위 탭.

* 최근에 삭제된 템플릿을 휴지통에서 복구할 수 있습니다. 휴지통에서 항목을 복구하는 방법에 대한 자세한 내용은 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 템플릿 삭제

{{step1-to-templates}}

템플릿 목록이 열립니다.

1. 템플릿 이름의 왼쪽에 있는 확인란을 클릭하여 삭제할 템플릿을 선택한 다음 를 클릭합니다 **삭제 > 예, 삭제합니다.** 삭제 확인.

   또는

   템플릿 이름을 클릭하여 액세스한 다음 **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) , 그런 다음 **템플릿 삭제 > 예, 삭제합니다.**.

   템플릿을 더 이상 프로젝트와 연결할 수 없습니다.
