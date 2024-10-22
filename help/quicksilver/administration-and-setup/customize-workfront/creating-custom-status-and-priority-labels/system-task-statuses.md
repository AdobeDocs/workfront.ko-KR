---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 시스템 작업 상태
description: Workfront에 내장된 세 가지 시스템 작업 상태가 필요합니다. 즉, 잠금을 해제하고 이름을 바꾸고 순서를 변경할 수 있지만 숨기거나 삭제할 수는 없습니다. 조직의 요구 사항에 맞게 새 시스템 작업 상태를 추가할 수도 있습니다. 작업 상태 변경은 일반적으로 수동 프로세스이지만 시스템에서 발생하는 다른 요인에 따라 작업 상태가 자동으로 변경되는 경우가 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 시스템 작업 상태

Workfront에 내장된 세 가지 시스템 작업 상태가 필요합니다. 즉, 잠금을 해제하고 이름을 바꾸고 순서를 변경할 수 있지만 숨기거나 삭제할 수는 없습니다.

조직의 요구 사항에 맞게 새 시스템 작업 상태를 추가할 수도 있습니다.

작업 상태를 변경하는 것은 일반적으로 수동 프로세스입니다. 그러나 시스템에서 발생하는 다른 요인에 따라 작업 상태가 자동으로 변경되는 경우 다음 목록에 요약된 경우가 있습니다.

Workfront 인스턴스에는 다음 작업 상태가 제공됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>시스템 작업 상태</th> 
   <th>이 상태가 발생하는 경우</th> 
   <th>작업이 이 상태일 때 발생하는 작업</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>신규(필수 상태)</td> 
   <td>새로 생성된 모든 작업의 기본 상태입니다.</td> 
   <td>작업이 현재 상태의 프로젝트에 있는 경우 작업에 할당된 사용자의 작업 요청 탭에 작업이 표시됩니다. 이제 사용자는 작업 작업을 시작할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>진행 중(필수 상태)</td> 
   <td>이 상태에서 작업을 배치하여 해당 작업에 대한 작업이 시작되었음을 나타낼 수 있습니다.</td> 
   <td> <p>작업을 진행 중으로 표시하면 작업에 실제 시작 일자 값이 표시됩니다.</p> <p>작업의 완료율을 수동으로 업데이트할 때까지 작업 진행률이 기록되지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>완료(필수 상태)</td> 
   <td> <p>작업이 완료되면 작업이 완료되었음을 수동으로 표시할 수 있습니다.</p> <p>작업의 추적 모드가 자동 완료로 설정된 경우 계획된 완료 일자에 도달하면 작업이 자동으로 완료로 표시됩니다.</p> </td> 
   <td> <p>작업이 완료되면 작업의 완료율이 100%로 표시됩니다. 작업이 완료되면 홈 영역에 있는 할당자의 내 작업 목록에서 제거됩니다.</p> <p>작업을 완료로 표시하면 작업에 실제 완료 일자 값이 표시됩니다.</p> <p><b>참고</b>: 작업에 불완전한 문제가 있고 작업 상태를 완료로 변경하면 상태가 자동으로 완료 - 보류 중인 문제로 변경됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
