---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 시스템 작업 상태
description: Workfront에 내장된 시스템 작업 상태 3개가 필요합니다. 즉, 잠금을 해제하고, 이름을 변경하고, 순서를 변경할 수 있지만 숨기거나 삭제할 수는 없습니다. 조직의 요구 사항에 맞게 새 시스템 작업 상태를 추가할 수도 있습니다. 작업 상태를 변경하는 것은 일반적으로 수동 프로세스이지만 시스템에서 발생하는 다른 요소에 따라 작업 상태가 자동으로 변경되는 경우가 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 시스템 작업 상태

Workfront에 내장된 시스템 작업 상태 3개가 필요합니다. 즉, 잠금을 해제하고, 이름을 변경하고, 순서를 변경할 수 있지만 숨기거나 삭제할 수는 없습니다.

조직의 요구 사항에 맞게 새 시스템 작업 상태를 추가할 수도 있습니다.

작업 상태를 변경하는 것은 일반적으로 수동 프로세스입니다. 하지만 시스템에서 발생하는 다른 요소에 따라 작업의 상태가 자동으로 변경되는 경우 다음 목록에 요약된 경우가 있습니다.

다음 작업 상태가 Workfront 인스턴스와 함께 제공됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>시스템 작업 상태</th> 
   <th>이 상태가 발생하는 경우</th> 
   <th>작업이 이 상태에 있을 때 발생하는 작업</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>새로 만들기(필수 상태)</td> 
   <td>새로 만든 모든 작업의 기본 상태입니다.</td> 
   <td>작업이 현재 상태의 프로젝트에 있는 경우 작업에 할당된 사용자의 작업 요청 탭에 작업이 표시됩니다. 이제 사용자가 작업 작업을 시작할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>진행 중(필수 상태)</td> 
   <td>해당 작업에 대한 작업이 시작되었음을 나타내는 작업을 이 상태로 배치할 수 있습니다.</td> 
   <td> <p>작업을 진행 중으로 표시하면 실제 시작 날짜에 대한 값이 표시됩니다.</p> <p>작업의 완료율을 수동으로 업데이트할 때까지 작업 진행 상태가 기록되지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>완료(필수 상태)</td> 
   <td> <p>작업이 완료되면 작업 완료를 수동으로 표시할 수 있습니다.</p> <p>작업의 추적 모드가 자동 완료로 설정되면 작업이 계획된 완료 날짜에 도달하면 자동으로 완료 로 표시됩니다.</p> </td> 
   <td> <p>작업이 완료되면 작업 완료율이 100%로 표시됩니다. 작업이 완료되면 홈 영역의 할당자의 작업 목록에서 작업이 제거됩니다.</p> <p>작업을 완료로 표시하면 작업은 실제 완료 날짜에 대한 값을 표시합니다.</p> <p><b>참고</b>: 작업에 불완전한 문제가 있고 작업 상태를 완료로 변경하면 상태는 자동으로 완료 - 보류 중인 문제로 변경됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
