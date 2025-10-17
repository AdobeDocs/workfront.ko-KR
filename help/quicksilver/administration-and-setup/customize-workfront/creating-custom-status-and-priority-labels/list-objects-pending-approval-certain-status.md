---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 특정 상태를 사용하여 승인 보류 중인 객체 나열
description: 상태를 삭제하려고 하면 시스템의 오브젝트에서 승인 보류 중인 프로세스에서 사용되고 있으므로 삭제할 수 없다는 오류 메시지가 표시될 수 있습니다. 이러한 객체를 찾아 검토하여 수행할 작업을 결정하려는 경우 해당 객체를 나열하는 보고서를 실행할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 특정 상태를 사용하여 승인 보류 중인 오브젝트 나열

상태를 삭제하려고 하면 시스템에서 하나 이상의 보류 중인 승인 프로세스에 있기 때문에 삭제할 수 없다는 오류 메시지가 표시될 수 있습니다. 보고서를 실행하여 승인 보류 프로세스에 있는 객체를 나열한 다음 각 객체에 대해 수행해야 할 작업을 결정할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
     <p>표준</p>
     <p>플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p><p>필터, 보기, 그룹화에 대한 액세스 편집</p></td>
  </tr>
  <tr> 
   <td>개체 권한</td> 
   <td>작성한 보고서에 대한 관리 권한을 받습니다.</td>
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 표준 모드에서

{{step1-to-reports}}

1. **새 보고서**&#x200B;를 클릭한 다음 **프로젝트 보고서**, **작업 보고서** 또는 **문제 보고서**&#x200B;를 선택하십시오.
1. **필터** 탭을 엽니다.
1. **필터 규칙 추가**&#x200B;를 클릭한 후 다음을 수행하여 규칙을 설정합니다.
   1. `status`을(를) 입력한 다음 표시될 때 **상태**&#x200B;을(를) 선택하십시오.
   1. 두 번째 필드에 **Equal**&#x200B;을(를) 둡니다.
   1. 세 번째 필드에서 상태의 이름을 선택합니다.
1. **필터 규칙 추가**&#x200B;를 다시 클릭한 후 다음을 수행하여 규칙을 설정합니다
   1. `pending status`을(를) 입력한 다음 찾는 개체 형식(**프로젝트**, **작업** 또는 **문제**) 아래에 표시되는 항목을 선택하십시오.
   1. 두 번째 필드에 **Equal**&#x200B;을(를) 둡니다.
   1. 세 번째 필드에 `in`을(를) 입력합니다.
1. **필터 규칙 추가**&#x200B;를 다시 클릭한 후 다음을 수행하여 규칙을 설정합니다
   1. 승인 프로세스를 입력한 다음 **승인 프로세스**&#x200B;에 표시될 때 **그룹 ID**&#x200B;을(를) 선택하십시오.
   1. 두 번째 필드에서 **비어 있음**&#x200B;을 선택합니다.
1. 보고서를 실행하고 지정한 상태(**프로젝트**, **작업** 또는 **문제**)에 따라 승인 프로세스와 함께 지정한 유형의 개체를 보류 중 상태로 나열하려면 **저장 + 닫기**&#x200B;를 클릭하십시오.
1. 이 단계를 반복하여 다른 두 객체 유형에 대해 동일한 정보를 찾습니다.


## 텍스트 모드

{{step1-to-reports}}

1. **새 보고서**&#x200B;를 클릭한 다음 **프로젝트 보고서**, **작업 보고서** 또는 **문제 보고서**&#x200B;를 선택하십시오.
1. **필터** 탭을 엽니다.
1. **텍스트 모드로 전환**&#x200B;을 선택합니다.
1. 다음 내용을 복사하여 편집 창에 붙여넣고 XXX를 상태의 3자리 키로 바꿉니다.

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   다음 문서에 표시된 대로 상태 목록에서 키를 볼 수 있습니다.
   * [시스템 프로젝트 상태 목록 액세스](project-statuses.md)
   * [시스템 작업 상태 목록 액세스](task-statuses.md)
   * [시스템 문제 상태 목록 액세스](issue-statuses.md)

1. 보고서를 실행하고 지정한 상태(**프로젝트**, **작업** 또는 **문제**)에 따라 승인 프로세스와 함께 지정한 유형의 개체를 보류 중 상태로 나열하려면 **저장 + 닫기**&#x200B;를 클릭하십시오.
1. 이 단계를 반복하여 다른 두 객체 유형에 대해 동일한 정보를 찾습니다.
