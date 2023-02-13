---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 참고 보고서에서 모든 업데이트 보기
description: 참고 보고서에서 모든 업데이트 보기
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 참고 보고서에서 모든 업데이트 보기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

객체의 업데이트 영역에는 기본적으로 최대 200개의 업데이트가 표시됩니다. 객체에 대해 사용자가 입력한 모든 업데이트를 보려면 모든 갱신을 표시하는 노트 보고서를 생성할 수 있습니다.

>[!NOTE]
>
>보고서를 작성하여 분개 입력 보고서를 사용하여 미리 보기에서 객체에 대한 업데이트를 볼 수 있습니다. 자세한 내용은 [업데이트 영역에 대한 보고서](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>액세스 권한 편집:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 달력 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오.<br>Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보기</p> <p>참고: 객체에 대한 보기 권한 이상의 권한이 없는 경우 해당 객체에 대한 정보가 보고서에 표시되지 않습니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 참고 보고서 만들기

객체에 대한 메모를 위한 보고서를 작성하는 것은 객체에 관계없이 동일합니다.

예를 들어, 프로젝트에 있는 모든 참고에 대한 노트 보고서를 만들려면 다음을 수행합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **보고서**.
1. 클릭 **새 보고서**, 그런 다음 **참고**.

1. (선택 사항) **보기 횟수**, 그런 다음 **열 추가** 를 추가하려면 **이름** 의 **프로젝트** 를 클릭합니다. 

1. (선택 사항) **그룹화**, 그런 다음 **그룹화 추가** 그룹화 기준 **프로젝트 이름**&#x200B;여러 프로젝트에 대해 동시에 보고하는 경우,\
   이렇게 하면 노트를 각 프로젝트별로 그룹화하여 보고서를 쉽게 읽을 수 있습니다. 

1. (선택 사항) **필터,** 그런 다음 **필터 규칙 추가** 를 눌러 하나의 프로젝트 또는 특정 프로젝트에 대해서만 필터링합니다.

1. (조건부 및 선택 사항) **프로젝트 이름** 로서의 **Equal** 업데이트를 보려는 프로젝트의 프로젝트 이름으로 이동합니다.  

1. 클릭 **저장 + 닫기**.\
   프로젝트에 대한 최소 보기 권한이 있는 모든 사용자가 프로젝트에 입력한 모든 업데이트가 보고서에 표시됩니다.
