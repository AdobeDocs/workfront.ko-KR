---
user-type: administrator
product-area: system-administration;projects
keywords: 킥스타트, 킥스타트, 킥스타트, 킥스타트
navigation-topic: use-kick-starts
title: 킥스타트 시나리오 간단한 프로젝트 및 작업 가져오기 준비
description: 킥스타트 방법을 사용하여 기본 프로젝트와 작업 가져오기에 사용할 수 있는 설정과 컨트롤에 대해 자세히 설명합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: 101a5a80d00a8113ce31222b92f77300a5b0ce8a
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 9%

---

# 킥스타트 시나리오: 간단한 프로젝트 및 작업 가져오기 준비

킥스타트 방법을 사용하여 기본 프로젝트와 작업 가져오기에 사용할 수 있는 설정과 컨트롤에 대해 자세히 설명합니다.

## 시나리오

구현 팀은 이 데이터를 시스템에 수동으로 입력하는 것이 아니라 활성 프로젝트에 대한 프로젝트 및 작업 정보를 가져오는 것이 좋습니다.

* [프로젝트](#projects)
* [작업 목록](#task-list)

### 프로젝트 {#projects}

다음 표에는 킥스타트 파일 형식에 매핑해야 하는 4개의 프로젝트와 기본 세부 정보가 나와 있습니다.

이 시나리오에서는 사용자를 이미 Adobe Workfront으로 가져왔다고 가정합니다. 사용자가 아직 Workfront에 없는 경우 다른 이름을 대체하거나 이 시나리오 전에 사용자와 함께 킥스타트 시나리오를 완료하십시오.

1. Workfront 구현.

   | 계획된 시작 일자 기준 | 오늘 |
   |---|---|
   | 프로젝트 관리자 | 제니퍼 캠벨 |
   | 프로젝트 스폰서 | 마크 루이스 |
   | 그룹 | 마케팅 |
   | 회사 | *귀사* |

   {style="table-layout:auto"}

1. HR 시스템 구현

   | 계획된 시작 일자 기준 | 20XX년 7월 14일 |
   |---|---|
   | 프로젝트 관리자 | 팸 레이놀즈 |
   | 프로젝트 스폰서 | 마크 루이스 |
   | 그룹 | 마케팅 |
   | 회사 | *귀사* |

   {style="table-layout:auto"}

1. 문서 관리 시스템 구현

   | 계획된 시작 일자 기준 | 20XX년 8월 22일 |
   |---|---|
   | 프로젝트 관리자 | 제니퍼 캠벨 |
   | 프로젝트 스폰서 | 레이 앤드루스 |
   | 그룹 | IT |
   | 회사 | *귀사* |

   {style="table-layout:auto"}

1. 새 캘린더 시스템을 구현합니다.

   | 계획된 시작 일자 기준 | 20XX년 9월 6일 |
   |---|---|
   | 프로젝트 관리자 | 팸 레이놀즈 |
   | 프로젝트 스폰서 | 레이 앤드루스 |
   | 그룹 | IT |
   | 회사 | *귀사* |

   {style="table-layout:auto"}

### 작업 목록 {#task-list}

다음 작업 목록에는 프로젝트에 대해 지나치게 단순화된 작업 목록이 표시됩니다. 프로젝트 간의 유일한 차이는 각 프로젝트의 시작 날짜와 진행 상황입니다.

상위 작업은 하위 작업의 기간, 작업 시간 및 완료율을 상속합니다. 요약 작업이 될 값에 대해서는 설정할 필요가 없습니다.

>[!NOTE]
>
>이 시나리오에 제공된 명령은에 제공된 단계별 지침만큼 명시적이지는 않습니다. [킥스타트 시나리오: 회사, 그룹, 역할 및 사용자 킥스타트 준비](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md). 회사 및 그룹 시트에서 값을 조회하고 복사하는 방법을 이미 학습했다고 가정합니다. 따라서 이러한 단계는 언급되지만 구체적인 설명은 제공되지 않습니다.

1. 구성.
1. 사용자를 가져옵니다.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당 대상:</td> 
      <td>레이 앤드루스</td> 
     </tr> 
     <tr> 
      <td role="rowheader">상위 작업</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td>1시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td>1시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>문서: 100%</p> <p>달력: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 권한을 설정합니다.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당 대상:</td> 
      <td>레이 앤드루스</td> 
     </tr> 
     <tr> 
      <td role="rowheader">상위 작업</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pred</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td>1시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td>1시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>문서: 100%</p> <p>달력: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 그룹을 작성합니다.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당 대상:</td> 
      <td>레이 앤드루스</td> 
     </tr> 
     <tr> 
      <td role="rowheader">상위 작업</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pred</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td>2일</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td>4시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>문서: 100%</p> <p>달력: 25%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 교육 준비

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당 대상:</td> 
      <td>크리스 매닝</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td>2일</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td>4시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>문서: 50%</p> <p>달력: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 지속적인 지원 정책을 수립합니다.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당 대상:</td> 
      <td>크리스 매닝</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td>2일</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td>4시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>문서: 50%</p> <p>달력: 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 롤아웃.

   | Pred | 1, 6, 7 |
   |---|---|

   {style="table-layout:auto"}

1. 사용자 교육.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">할당 대상:</td> 
      <td>크리스 매닝</td> 
     </tr> 
     <tr> 
      <td role="rowheader">상위 작업</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td>1일</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td>2시간</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 0%</p> <p>문서: 0%</p> <p>달력: 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 템플릿 다운로드

킥스타트 페이지로 이동합니다. 회사, 그룹, 프로젝트, 작업 및 사용자 객체를 선택합니다. 기존 데이터 포함 확인란을 선택합니다(회사, 그룹 및 사용자 ID를 빠르게 참조하려면 이 작업을 수행). 다운로드 단추를 클릭합니다.

## 프로젝트 세부 정보 입력

방금 다운로드한 Workfront.xlsx 파일을 엽니다. 프로젝트 프로젝트 시트로 이동합니다.

![](assets/im2.png)
Workfront에서 프로젝트를 이미 만들지 않았다면 비워 두어야 합니다.

![](assets/im10.png)

다음 프로젝트 필드에 대한 값을 설정합니다.

* **isNew 열 설정**
isNew 열의 3행부터 6행까지 TRUE를 입력합니다.
* **고유 ID 설정**
ID 열의 각 행에 고유한 ID를 입력합니다. 일반적으로 새 레코드를 만들 때 1에서 시작하는 정수가 잘 작동합니다.
* **프로젝트 이름 설정**
각 프로젝트의 이름을 setName 열에 입력합니다.
* **프로젝트 일정 설정**

  setScheduleID 필드에 프로젝트가 사용할 일정의 ID를 입력합니다

* **프로젝트 계획 시작 일자 설정**

  setPlannedStartDate 열에 날짜 및 시간을 입력하고 프로젝트를 시작할 시간 및 날짜를 입력합니다. 비워 두면 Workfront은 브라우저의 시간대에 따라 현재 날짜의 타임스탬프와 해당 날짜 자정의 타임스탬프로 프로젝트를 가져옵니다.

* **작업 번호 설정**
프로젝트 계획에 작업이 표시되는 순서를 제어하려면 setTaskNumber 열에 값을 입력합니다.
* **프로젝트 날짜를 제공합니다.**
setPlannedStartDate 열에 각 프로젝트의 계획된 시작 일자를 입력합니다.
* **필요한 기타 세부 정보를 설정합니다.**
필요에 따라 설명 또는 현재 상태 등 다른 세부 정보를 입력합니다. 그룹 그룹 시트에서 각 프로젝트의 그룹 ID를 조회하고 각 프로젝트의 setGroupID 열에 입력합니다. CMPY 회사 시트에서 프로젝트에 대한 회사 ID를 조회하고 setCompanyID 열에 입력합니다. 사용자 사용자 시트에서 각 프로젝트 소유자에 대한 사용자 ID를 조회하고 setOwnerID 열에 입력합니다. USER User 시트에서 각 프로젝트 스폰서에 대한 사용자 ID를 조회하고 setSponsorID 열에 입력합니다.

![](assets/im9.png)

>[!NOTE]
>
>상태 및 우선 순위 필드에 대해 허용되는 값은 Workfront의 워크플로 설정 영역에서 각 개체의 상태 및 우선 순위 환경 설정을 검토하여 찾을 수 있습니다.

## 작업 세부 정보 입력

킥스타트를 사용하여 프로젝트를 가져올 때 프로젝트의 작업에 대한 정보를 추가할 수 있습니다.

방금 다운로드한 Workfront.xlsx 파일을 엽니다. **TASK Task 시트로 이동합니다.**

Workfront에서 작업을 이미 만들지 않은 경우 이 시트는 비어 있어야 합니다.

![](assets/im8.png)

![](assets/im7.png)

![](assets/im6.png)

작업을 매핑하는 가장 쉬운 방법은 한 번에 하나의 프로젝트입니다(특히 각 프로젝트에서 작업이 동일한 경우). 그런 다음 첫 번째 프로젝트에 대한 작업 계획을 복사하고 후속 프로젝트에 대한 작업 계획을 약간 조정할 수 있습니다. 나머지 단계에서는 Workfront 구현 프로젝트에 대한 작업만 만드는 것으로 가정합니다. 시나리오에 따라 프로젝트당 9개의 작업을 가져오므로 isNew 열에 대해 3행부터 11행까지 TRUE를 입력합니다.

다음 작업 필드에 대한 값을 설정합니다.

* **ID 설정**
ID 열의 각 행에 고유한 ID를 입력합니다.
* **이름 설정**
setName 열에 작업 이름을 입력합니다.
* **프로젝트 ID 확인**
Workfront 구현 프로젝트에 대해 설정한 ID를 입력합니다. 프로젝트 프로젝트 시트 를 검토하여 ID가 올바른지 확인하십시오.
* **사용자 설정**
USER User 시트로 이동하여 각 작업에 할당된 사용자의 ID를 조회하고 setAssignedToID 열의 각 셀에 이러한 값을 입력합니다.
* **작업 관계 식별**
작업 2~5의 경우 setParentID 열에 1을 입력합니다. 작업 9의 경우 setParentID 열에 8을 입력합니다. setPrecedentString 열에서 각 전임 작업의 작업 번호를 입력합니다. 이 시나리오의 작업 8과 같이 작업에 여러 전임 작업이 있는 경우 쉼표를 사용하여 각 전임 작업 ID를 구분해야 합니다. 전임 작업은 전임 작업 관계 만들기 문서에 설명된 속기를 사용하여 비완료 시작 관계에서 지연으로 정의할 수 있습니다.
* **기간 설정**
setDuration 필드에 작업의 시간, 일, 주 또는 월 수를 입력하여 각 작업의 기간을 설정합니다. 그런 다음 setDurationUnit 필드에 기간 단위를 입력합니다.

  |   | 허용 값 |
  |---|---|
  | 분 | M |
  | 시간 | H |
  | 일 | D |
  | 주 | 주 |
  | 개월 | T |

  분은 또한 시간의 분수(예를 들어, minutets = 5시간)로 표현될 수 있다

* setWorkRequired 필드에서 각 작업에 대한 작업량을 설정합니다. 그런 다음 setWorkUnit 필드에 작업 단위를 입력합니다. 작업 필요 값이 duration과 다른 경우 setDurationType 필드에 A를 입력해야 합니다.

  | 기간 유형 | 허용 값 |
  |---|---|
  | 계산된 할당 | A |
  | 계산된 작업 | 주 |
  | 작업량 고정 | D |
  | 단순 | S |

* 각 작업의 setPercentComplete 필드에 완료율의 전체 숫자 표현을 입력합니다. 이 값에는 퍼센트 기호(%)를 포함하지 않아야 합니다.
* 필요에 따라 생성 중인 각 작업에 대한 설명 및 기타 세부 정보를 포함합니다.

  ![](assets/im5.png)

* 전임 작업 관계를 사용하고 있으므로 setPlannedStartDate 및 setTaskConstraint 열은 이 프로젝트의 타임라인을 작성하는 데 사용되지 않습니다. 대신 각 작업의 날짜를 입력할 수 있습니다. 이렇게 하려면 setTaskConstraint 열에도 유효한 작업 제한 사항을 제공해야 합니다. 이 필드의 유효한 값에 대한 자세한 내용은 작업 제한 및 관련 문서를 검토하십시오.

  이 시나리오의 경우 가져오려는 다른 프로젝트에 대한 작업을 가장 쉽게 작성하는 방법은 방금 정의한 작업을 복사하여 아래 12행부터 붙여넣는 것입니다. 그러면 다음을 수행합니다.

   1. ID 열에서 값의 번호를 다시 매깁니다.
   1. setProjectID 열을 다음 프로젝트에 대해 설정한 값으로 업데이트합니다.
   1. 이 프로젝트의 작업에 할당된 새 ID를 반영하도록 setParentID 및 setPrecedentString 값을 업데이트합니다.
   1. 작업 할당 및 완료율을 업데이트합니다.
   1. 다음 프로젝트의 작업에 대해 이 단계를 반복합니다.

* **Excel 파일 가져오기**

  에 제공된 지시 사항을 따르십시오. [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
