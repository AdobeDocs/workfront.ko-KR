---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 시간 및 날짜 차이 계산'
description: 다음의 차이를 계산할 수 있습니다. - EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 보기: 시간 및 날짜 차이 계산

>[!IMPORTANT]
>
>Adobe Workfront에서 같은 종류의 서로 다른 두 개체 간의 시간 및 날짜 차이를 계산할 수 없습니다. 예를 들어 서로 다른 두 프로젝트, 작업 또는 문제에 대한 두 날짜 간의 시간 및 날짜 차이를 계산할 수 없습니다.

다음 항목 간의 차이를 계산할 수 있습니다.

* 동일한 오브젝트에 있는 두 날짜 필드 간의 시간 및 날짜 차이
* 개체의 필드와 부모 개체의 다른 필드 사이의 시간 및 날짜 차이입니다

>[!TIP]
>
>이 계산에는 두 날짜 사이의 일 수가 표시됩니다. 결과는 일 단위로 표시됩니다. 날짜 필드의 타임스탬프도 고려되며, 타임스탬프가 일치하지 않으면 일 수 뒤에 소수가 올 수 있습니다. 작업이 늦게 완료된 경우 일 수가 음수 값으로 표시됩니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>보기 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 동일한 오브젝트에 있는 두 날짜 필드 간의 시간 및 날짜 차이 계산

예를 들어 작업의 계획된 완료 일자와 실제 완료 일자 간의 차이를 계산할 수 있습니다.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. 작업 목록으로 이동합니다.
1. 다음에서 **보기** 드롭다운 메뉴, 클릭 **새 보기**.

1. 클릭 **열 추가** 및 을(를) 시작하고 &quot;계획된 완료 일자&quot;를 **이 열에 표시** 필드에 입력한 후 목록에 표시되면 선택합니다.

1. 클릭 **열 추가** 및 을(를) 시작하고 &quot;실제 완료 일자&quot;를 **이 열에 표시** 필드에 입력한 후 목록에 표시되면 선택합니다.

1. 클릭 **열 추가**&#x200B;을 클릭한 다음 을 클릭합니다 **텍스트 모드로 전환**.

1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 에서 찾은 텍스트 제거 **텍스트 모드** 확인란을 선택하고 다음 코드로 바꿉니다.

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. 클릭 **저장**, 그런 다음 **보기 저장**.

## 개체의 필드와 부모 개체의 다른 필드 간의 시간 및 날짜 차이를 계산합니다.

객체 및 상위 객체 목록에 대해서는 의 &quot;상호 종속성 및 객체 계층 이해&quot; 섹션을 참조하십시오. [Adobe Workfront의 오브젝트 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
예를 들어 작업의 계획된 완료 일자와 상위 작업 또는 작업이 진행 중인 프로젝트의 계획된 완료 일자 간의 차이를 계산할 수 있습니다.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. 작업 목록으로 이동합니다.
1. 다음에서 **보기** 드롭다운 메뉴, 클릭 **새 보기**.

1. 클릭 **열 추가** 다음에 &quot;프로젝트 계획 완료 일자&quot; 또는 &quot;상위 완료 일자&quot;를 입력하십시오. **이 열에 표시** 필드에 입력한 후 목록에 표시되면 선택합니다.

1. 클릭 **열 추가** 및 을(를) 시작하고 &quot;계획된 완료 일자&quot;를 **이 열에 표시** 필드에 입력한 후 목록에 표시되면 선택합니다.

1. 클릭 **열 추가**&#x200B;을 클릭한 다음 을 클릭합니다 **텍스트 모드로 전환**.

1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 에서 찾은 텍스트 제거 **텍스트 모드** 상자를 표시하고 다음 코드 중 하나로 바꿉니다.

   * 프로젝트의 계획된 완료 일자와 태스크의 계획된 완료 일자 간의 차이를 표시하려면

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * 상위 작업의 계획된 완료 일자와 작업의 계획된 완료 일자 간의 차이를 표시하려면 다음을 수행합니다.

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. 클릭 **저장**, 그런 다음 **보기 저장**.
