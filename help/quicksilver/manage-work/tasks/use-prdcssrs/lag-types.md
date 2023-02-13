---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 지연 유형 개요
description: 지연은 종속 작업을 시작할 수 있을 때까지 강제 선행 작업이 완료된 후 경과해야 하는 시간(양수 지연) 또는 종속 작업이 선행 작업이 시작되기 전에 시작할 수 있는 시간(음수 지연)입니다.
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# 지연 유형 개요

지연은 종속 작업을 시작할 수 있을 때까지 강제 선행 작업이 완료된 후 경과해야 하는 시간(양수 지연) 또는 종속 작업이 선행 작업이 시작되기 전에 시작할 수 있는 시간(음수 지연)입니다.

후속 태스크의 계획, 예상 및 예상 일자는 이전 태스크의 지연 및 계획, 예상 시작(완료) 일자를 고려하여 계산됩니다.

## 액세스 요구 사항

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업의 지연 및 지연 유형 표시

이전 관계를 정의할 때 작업의 지연 유형을 표시할 수 있습니다.

* [작업의 선행 작업 섹션에서 지연 유형 표시](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [작업 목록에서 지연 유형 표시](#indicate-lag-types-in-a-task-list)

### 작업의 선행 작업 섹션에서 지연 유형 표시 {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 선행 작업 및 지연 유형을 정의할 작업으로 이동합니다.
1. 클릭 **선행 작업** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **선행 작업**.
1. 클릭 **선행 작업 추가**.
1. (선택 사항) 프로젝트 간 선행 작업을 추가하려면 를 바꿉니다 **상위 프로젝트** 다른 프로젝트에 이름을 지정합니다.
1. 선행 작업의 이름을 입력하고 목록에 표시될 때 선택합니다.
1. 을(를) 선택합니다 **종속성 유형**.

   이전 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 을(를) 지정합니다 **지연** 숫자 값을 사용한 금액. 음수 숫자를 지정하여 음수 지연을 나타낼 수 있습니다.
1. 다음 옵션 중에서 선택하여 전임자에 대해 표시할 지연 유형을 식별합니다.

   * **일**
   * **캘린더 일자**
   * **백분율**
   * **요일**
   * **요일(0이 아님)**

      이러한 지연 유형 및 그 계산 방법에 대한 자세한 내용은 섹션을 참조하십시오 [지연 유형 개요](#lag-types-overview) 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

### 작업 목록에서 지연 유형 표시  {#indicate-lag-types-in-a-task-list}

1. 작업 목록으로 이동한 후 **표준** 에서 보기 **보기** 드롭다운 메뉴

1. 의 내부를 클릭합니다. **선행 작업** 선행 작업과 지연 금액을 지정할 작업에 해당하는 열입니다.
1. 공백 없이 다음을 입력합니다.

   * 선택한 작업의 선행 작업으로 표시할 작업 수입니다.
   * 작업 사이에 나타낼 종속성 유형의 약어입니다

      종속성 유형에 대한 약어에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * 다음 중 하나 **+** 긍정적인 지연 또는 **-** 시차증

   * 시차 횟수
   * 사용하려는 Lag Type의 약어입니다.

      지연 유형의 약어에 대한 자세한 내용은 섹션을 참조하십시오 [지연 유형 개요](#lag-types-overview) 참조하십시오.
   예를 들어, 이전 작업이 있고 2일의 지연 시간이 양수임을 나타내려면 다음을 입력합니다

   ```
   1fs+2d
   ```

   선행 작업 열에 있습니다.

1. 키보드에서 Enter 키를 클릭하여 작업에 대한 변경 사항을 저장합니다.

## 지연 유형 개요 {#lag-types-overview}

지연 시간이 필요한 작업의 예는 나무를 목재로 절단하는 것일 수 있습니다. 갓 베인 목재는 잘라 내기 전에 오랫동안 말려야 한다면, 나무를 깎고 목재로 절단하는 사이에 시간이 걸릴 것이다.

다음 테이블에서는 지연 유형 및 각 지연 유형에 대한 시간을 나타내는 방법을 보여줍니다.

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>값</strong> </p> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>일(d)</p> </td> 
   <td> <p>종속성에 의해 연결된 두 작업 사이의 지연 시간은 작업 일 단위로 측정됩니다. 기본 지연 유형입니다. </p> <p>예를 들어, 2일의 작업 지연 없이 완료 시작 종속성이 있고 이전 작업이 금요일에 완료되면 종속 작업은 수요일에 시작됩니다. 주말 일수는 지연의 일부로 간주되지 않는다. </p> <p>참고: 일수의 최대 지연 제한은 366입니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>달력 일(c)</p> </td> 
   <td> <p>휴일과 주말을 포함하여 두 작업 사이의 지연은 달력 일 단위로 측정됩니다. </p> <p>참고: 이 지연 유형은 비근무일을 지연의 일부로 계산하지만 종속 작업은 비근무일에 시작할 수 없습니다. 이 지연 유형으로 종속 태스크가 비근무일에 시작하는 경우 종속 태스크의 계획 시작 일자는 다음 작업일에 스케줄링됩니다. </p> <p>예를 들어 2일 지연이 있는 완료 시작 종속성이 있고 이전 작업이 목요일에 완료되면 종속 작업은 일요일이 아닌 월요일에 시작됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>백분율(p 또는 pe)</p> </td> 
   <td> <p>지연 시간은 이전 작업을 완료하는 예상 시간의 백분율로 표시됩니다. </p> <p>예를 들어 10일 이전 작업 사이에 20% 지연이 있는 완료 시작 종속성이 있는 경우, 시스템은 이전 작업 기간의 20%가 되는 일을 계산하여 이를 지연으로 사용합니다. 이 경우 작업이 완료된 후 2일이 됩니다. </p> <p>참고: 백분율에 대한 최대 지연 제한은 2000%입니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>요일(w) </p> </td> 
   <td> <p>두 작업 사이의 지연은 선행 작업의 계획된 완료 날짜가 포함된 주의 요일을 표시하여 측정됩니다.</p> <p>이 지연 유형의 경우 요일의 각 날이 숫자와 연결됩니다.</p> 
    <ul> 
     <li>일요일=1</li> 
     <li>월요일=2</li> 
     <li>화요일=3</li> 
     <li>수요일=4</li> 
     <li>목요일=5</li> 
     <li>금요일=6</li> 
     <li>토요일=7</li> 
    </ul> <p>후임자의 계획 시작 일자가 현재 주의 화요일과 화요일이 이전 주의 계획 완료 일자 이전임을 나타내려면 다음과 같은 공식을 사용하여 후임자를 코딩합니다. </p> <p><code style="font-style: normal;">4fs-3w</code> </p> <p>참고: 선행 작업의 계획 완료 일자 요일에 대한 화요일이 경과된 경우, 후속 태스크의 계획 시작 일자는 해당 주의 첫 사용 가능한 작업일입니다. </p> <p>지연이 현재 주의 토요일과, 토요일이 이전 주의 계획 완료 일자 이후임을 나타내려면, 다음 공식을 사용하여 후임자에게 코드를 지정합니다.</p> <p><code style="font-style: normal;">4fs+7w</code> </p> <p>토요일이 비근무일인 경우, 다음 가용 일자(양수 지연 표시)가 후임자의 계획 시작 일자로 선택됩니다. </p> <p>과거 또는 미래 주를 나타내려면 지연 유형의 일 번호 앞에 숫자를 추가할 수 있습니다. </p> <p>예를 들어 10주 전 월요일인 경우 이 코드를 사용하여 후임자의 전임자를 나타낼 수 있습니다.</p> <p><code>4fs-102w</code> </p> <p>10은 10주 전을 나타내고 2는 월요일에 지정된 번호입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>요일(0 제외)</p> </td> 
   <td> <p>이전 작업의 시간이 지정된 요일에 끝나는 경우를 제외하고 두 작업 사이의 지연 시간은 요일 지연 유형과 동일하게 측정됩니다. 그런 다음 지연 시간이 인접 주(+/-)로 계산됩니다. </p> <p>이 경우 지연 시간은 0일 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 음수 지연 개요

음수 지연 을 사용하여 선행 작업이 종료되기 전에 작업을 시작할 필요성이나 능력을 나타낼 수 있습니다.

음수 대전을 사용할 때는 다음 규칙을 고려하십시오.

* 음수 지연(Negative Lag)을 사용하면 작업의 시작/완료 날짜가 프로젝트의 계획 시작/완료 날짜 이전이나 이후가 될 수 없습니다. 이 날짜는 프로젝트의 시작 스케줄 필드에 지정됩니다.

   이 경우 다음 사항을 고려하십시오.

   * 프로젝트를 완료 날짜로부터 스케줄링합니다.
   * 프로젝트의 마지막 작업은 작업 제약 조건에 대한 완료 필수 를 사용해야 합니다. 프로젝트에 있는 모든 작업을 고려할 수 있도록 작업에 충분한 기간을 제공하는 것이 좋습니다. 나머지 작업은 가능한 한 빨리 제약 조건에 잘 작동합니다.

* 작업과 함께 Finish-Start 선행 관계를 사용하면 오류 메시지가 나타날 수 있습니다.

   이 경우 다음 사항을 고려하십시오.

   * 작업 간 완료 - 완료 선행 관계를 설정합니다.
   * 후속 작업의 기간은 작업 사이의 예상 지연 시간(일)과 같거나 이를 초과해야 합니다.
