---
title: 각 객체 유형에 대한 기능에 대한 구성 가능한 액세스
description: 이 문서에서는 각 액세스 수준의 각 객체 유형에 대해 Adobe Workfront 관리자가 허용할 수 있는 사항에 대해 설명합니다. 또한 각 액세스 수준 유형에 대한 기본 구성이 무엇인지 설명합니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '3436'
ht-degree: 10%

---

# 각 객체 유형에 대한 기능에 대한 구성 가능한 액세스

이 문서에서는 각 액세스 수준의 각 객체 유형에 대해 Adobe Workfront 관리자가 허용할 수 있는 사항에 대해 설명합니다. 또한 각 액세스 수준 유형에 대한 기본 구성이 무엇인지 설명합니다.

각 액세스 수준의 개체 유형에 사용할 수 있는 모든 기능에 대한 자세한 내용은 [각 개체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)을 참조하십시오.

## 프로젝트

각 액세스 수준에서 프로젝트에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너(플랜 라이선스 유형)</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 프로젝트를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 프로젝트에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>복사</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>보기</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 프로젝트를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 프로젝트에 대한 제한된 편집 액세스를 허용합니다. 작업자 액세스 수준에서 편집 액세스가 플래너 액세스 수준(프로젝트에 대한 전체 편집 액세스 허용)과 비교하여 어떻게 제한되는지 보려면 문서 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">각 개체 유형에 사용할 수 있는 기능</a>의 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">프로젝트</a> 섹션을 참조하십시오.</p> <p>이를 미세 조정하려면 프로젝트를 공유하는 기능을 구성할 수 있습니다. [편집] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> (기본 선택) <p>프로젝트 공유를 활성화하거나 비활성화하도록 세부 조정할 수 없기 때문에 보기 액세스가 제한됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>프로젝트에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 작업

각 액세스 수준에서 작업에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 작업 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 작업에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 작업 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 작업에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> (기본 선택)<p>프로젝트 공유를 활성화하거나 비활성화하도록 세부 조정할 수 없기 때문에 보기 액세스가 제한됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>작업에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 문제

각 액세스 수준에서 문제에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b></p><p>이를 미세 조정하려면 문제를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문제에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 문제를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문제에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 문제를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문제에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 문제를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문제에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>문제에 대한 액세스를 사용할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 포트폴리오

각 액세스 수준에서 포트폴리오에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 포트폴리오 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 포트폴리오에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> <p>포트폴리오에 액세스할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>포트폴리오에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 프로그램

각 액세스 수준에서 프로그램에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 프로그램을 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 프로그램에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> <p>프로그램에 액세스할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>프로그램에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 보고서, 대시보드 및 캘린더

각 액세스 수준에서 보고서, 대시보드 및 달력에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b></p><p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 동작을 사용하지 않도록 설정하거나 사용하도록 설정하십시오. 기본적으로 둘 다 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>기본 제공 보고서 보기</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
     <li> <p><b>편집</b>(기본 선택): 보고서, 대시보드 및 일정에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. <b>기본 제공 보고서 보기</b>, <b>보고서를 공개적으로 공유</b> 및 <b>시스템 전체에서 공유</b>를 제외하고 모든 보고서를 기본적으로 사용할 수 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>기본 제공 보고서 보기</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>보고서 공개(외부)</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> (기본 선택)<p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 동작을 사용하지 않도록 설정하거나 사용하도록 설정하십시오. 기본적으로 둘 다 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>기본 제공 보고서 보기</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b>(기본 선택)<p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 동작을 사용하지 않도록 설정하거나 사용하도록 설정하십시오. 공유 옵션만 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>기본 제공 보고서 보기</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b>(기본 선택): 공유된 보고서, 대시보드 및 일정에 대한 보기 전용 액세스를 허용합니다.</p> <p>이를 미세 조정하려면 기본 제공 보고서를 보는 기능을 구성할 수 있습니다. <b>보기</b> 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>기본 제공 보기</b>(기본적으로 비활성화됨)을(를) 비활성화하거나 사용하도록 설정합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>보고서, 대시보드 및 캘린더에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 필터, 보기 및 그룹화

각 액세스 수준에서 필터, 보기 및 그룹화에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b></p><p>이를 미세 조정하려면 필터, 보기 및 그룹화를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 필터, 보기 및 그룹화에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b></p><p>이를 미세 조정하려면 필터, 보기 및 그룹화를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 필터, 보기 및 그룹화에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 필터, 보기 및 그룹화를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 필터, 보기 및 그룹화에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b>:</p> <p>이를 미세 조정하려면 필터, 보기 및 그룹화를 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 필터, 보기 및 그룹화에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>필터, 보기 및 그룹화에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 문서

각 액세스 수준에서 문서에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 문서 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문서에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. <b>공개적으로 문서 공유</b> 및 <b>시스템 전체 공유</b>를 제외하고 모든 기능을 기본적으로 사용할 수 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>공개적으로(외부적으로) 문서 공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b></p><p>이를 미세 조정하려면 문서 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문서에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. <b>공개적으로 문서 공유</b> 및 <b>시스템 전체 공유</b>를 제외하고 모든 기능을 기본적으로 사용할 수 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>공개적으로(외부적으로) 문서 공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 문서 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문서에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 동작을 사용하지 않도록 설정하거나 사용하도록 설정하십시오. 마지막 두 개, <b>공개적으로 문서 공유</b> 및 <b>시스템 전체 공유</b>를 제외하고 모두 기본적으로 사용됩니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>공개적으로(외부적으로) 문서 공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b></p><p>이를 미세 조정하려면 문서 공유 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 문서에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>이 액세스 수준에서는 문서에 대한 액세스를 구성할 수 없습니다. 하지만 외부 사용자는 Workfront을 사용하여 문서를 보고, 검토하고, 다운로드할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자

각 액세스 수준에서 사용자를 위해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b></p><p>이를 미세 조정하려면 사용자의 연락처 정보를 보는 기능을 구성할 수 있습니다. <b>보기</b> 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>연락처 정보 보기</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 사용자에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 동작을 사용하지 않도록 설정하거나 사용하도록 설정하십시오. 처음 두 옵션인 <b>만들기</b> 및 <b>삭제</b>만 기본적으로 활성화됩니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li>사용 관리자(모든 사용자)</li> 
       <li> <p>사용자 관리자(그룹 사용자)</p> </li> 
      </ul> <p>두 개의 사용자 관리 옵션에 대한 자세한 내용은 문서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>의 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 지정 액세스 수준을 사용하여 사용자를 편집하는 사용자 액세스 구성</a> 섹션을 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li><p> <b>보기</b>(사용 가능한 옵션만)</p><p>이를 미세 조정하려면 사용자의 연락처 정보를 보는 기능을 구성할 수 있습니다. <b>보기</b> 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>연락처 정보 보기</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li><p> <b>보기</b>(사용 가능한 옵션만)</p> <p>이를 미세 조정하려면 사용자의 연락처 정보를 보는 기능을 구성할 수 있습니다. <b>보기</b> 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>연락처 정보 보기</b> 옵션(기본적으로 비활성화됨)을 활성화하거나 비활성화합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b>(사용 가능한 옵션만)</p><p>이를 미세 조정하려면 사용자의 연락처 정보를 보는 기능을 구성할 수 있습니다. <b>보기</b> 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>연락처 정보 보기</b> 옵션(기본적으로 비활성화됨)을 활성화하거나 비활성화합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>사용자에게 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 팀

각 액세스 수준에서 팀에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li><b>보기</b> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. 기본적으로 둘 다 비활성화되어 있습니다.</p> 
      <ul> 
       <li>모든 팀 보기</li> 
       <li> <p>내 그룹과 관련된 팀 보기</p> </li> 
      </ul> </li> 
     <li> <p><b>편집</b>(기본 선택): 팀에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. <b>내가 속한 팀 편집</b>을 제외한 모든 팀이 기본적으로 활성화됩니다.</p> 
      <ul> 
       <li>만들기</li> 
       <li>삭제</li> 
       <li> <p>내가 속한 팀 편집</p> </li> 
       <li> <p>내가 관리하는 그룹의 팀 편집(그룹 관리자 전용)</p> </li> 
       <li> <p>모든 팀 보기</p> </li> 
       <li> <p>내 그룹과 관련된 팀 보기</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <b>보기</b>
      <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. 둘 다 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li>모든 팀 보기</li> 
       <li> <p>내 그룹과 관련된 팀 보기</p> </li> 
      </ul> </li> 
     <li> <p><b>편집</b>(기본 선택): 팀에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. 첫 번째 옵션인 <b>내가 속한 팀 편집</b>만 기본적으로 비활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>내가 속한 팀 편집</p> </li> 
       <li> <p>모든 팀 보기</p> </li> 
       <li> <p>내 그룹과 관련된 팀 보기</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b>(사용 가능한 옵션만)</p> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. 둘 다 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>모든 팀 보기</p> </li> 
       <li>내 그룹과 관련된 팀 보기</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <p><b>보기</b>(사용 가능한 옵션만)</p> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. 둘 다 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>모든 팀 보기</p> </li> 
       <li>내 그룹과 관련된 팀 보기</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>팀에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>


## 템플릿

각 액세스 수준에서 템플릿에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li><p> <b>보기</b></p> <p>이를 미세 조정하려면 템플릿을 공유하는 기능을 구성할 수 있습니다. [보기] 단추에서 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음 <b>공유</b> 옵션(기본적으로 활성화됨)을 비활성화하거나 활성화하십시오.</p> </li> 
     <li> <p><b>편집</b>(기본 선택): 템플릿에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 이 모든 기능은 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li> <p>만들기</p> </li> 
       <li> <p>삭제</p> </li> 
       <li> <p>공유</p> </li> 
       <li> <p>시스템 전체 공유</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <p><b>액세스 권한 없음</b>(사용 가능한 옵션만)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <p><b>액세스 권한 없음</b>(사용 가능한 옵션만)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <p><b>액세스 권한 없음</b>(사용 가능한 옵션만)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>템플릿에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 재무 데이터

각 액세스 수준에서 재무 데이터에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <p><b>보기</b>:</p> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. 둘 다 기본적으로 활성화되어 있습니다.</p> 
      <ul> 
       <li>역할 과금 및 비용 요금 보기</li> 
       <li> <p>사용자 과금 및 비용 요금 보기</p> </li> 
      </ul> </li> 
     <li> <p><b>편집</b>(기본 선택): 재무 데이터에 대한 전체 편집 액세스를 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>보기</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션 중 하나를 비활성화하거나 활성화하십시오*. <b>역할 청구 및 비용 요금 보기</b> 및 <b>사용자 청구 및 비용 요금 보기</b> 옵션 중 마지막 두 가지 옵션만 기본적으로 활성화됩니다.</p> 
      <ul> 
       <li>역할 과금 및 비용 요금 편집</li> 
       <li> <p>사용자 과금 및 비용 요금 편집</p> </li> 
       <li>역할 과금 및 비용 요금 보기</li> 
       <li> <p>사용자 과금 및 비용 요금 보기</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li> <p><b>액세스 권한 없음</b>(기본 선택)</p> </li> 
     <li> <b>보기</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <p><b>액세스 권한 없음</b>(기본 선택)</p> </li> 
     <li><b>보기</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <p><b>액세스 권한 없음</b>(사용 가능한 옵션만)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>재무 데이터에 액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 이러한 옵션에 대한 자세한 내용은 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)를 참조하십시오.

## 리소스 관리

각 액세스 수준에서 리소스 관리에 대해 다음 옵션을 구성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액세스 수준</th> 
   <th>옵션</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>플래너 </td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b> </li> 
     <li> <p><b>편집</b>(기본 선택): 리소스 관리에 대한 전체 편집 액세스 권한을 허용합니다.</p> <p>이 설정을 미세 조정하려면 <b>편집</b> 단추의 톱니바퀴 아이콘 <img src="assets/gear-icon-in-access-levels.png">을(를) 클릭한 다음, 다음 옵션을 비활성화하거나 활성화하십시오. 첫 번째 옵션인 <b>플래너에서 우선 순위 및 예산 시간 편집</b>만 기본적으로 사용됩니다.</p> 
      <ul> 
       <li> <p> 플래너에서 우선 순위 및 예산 시간 편집</p> </li> 
       <li> <p>리소스 풀 관리</p> <p><b>참고</b>: 리소스 풀을 관리하려면 사용자가 재무 데이터에 대한 추가 액세스 권한과 프로젝트 재무 관리에 대한 사용 권한이 필요합니다. 재무 데이터에 대한 액세스 권한이 없는 플래너 사용자에게 리소스 관리 액세스 권한을 부여하는 경우 사용자는 리소스 플래너에서 시간별 할당을 계속 볼 수 있지만 비용 보기로 전환하거나 비즈니스 사례를 볼 수는 없습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a> 및 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">개체에 대한 재무 권한 공유</a>를 참조하십시오.</p> </li> 
       <li> <p>업무 균형자에서 계획된 시간 업데이트</p> <p><b>참고</b>: 업무 균형자에서 계획된 시간을 업데이트하려면 [고급 설정]에서 [할당]을 사용하도록 설정하여 사용자에게 개체에 기여할 수 있는 권한이 있어야 합니다. 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 공유 권한 개요</a>를 참조하십시오.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>보조 </td> 
   <td> 
    <ul> 
     <li><b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>검토자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b> </li> 
     <li> <b>보기</b>(기본 선택)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>요청자</td> 
   <td> 
    <ul> 
     <li> <b>액세스 권한 없음</b>(사용 가능한 옵션만) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>외부 사용자</td> 
   <td> <p>액세스할 수 없습니다. 외부 사용자는 Workfront을 사용하여 문서를 검토 및 다운로드하고 공유된 캘린더를 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 시나리오 플래너 영역

모든 액세스 수준에 대한 기본 설정은 액세스 없음입니다. Workfront 관리자는 이를 모든 플래너, 작업자 및 검토자 액세스 수준에 대한 보기 또는 편집 액세스 권한으로 변경할 수 있습니다.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>플랜에 대한 링크가 다른 사용자와 공유되는 경우에만 다른 사용자가 만든 플랜을 볼 수 있습니다.

## Workfront 목표 영역

기본 액세스 수준 6개 모두(및 라이선스 유형 4개 모두)는 Workfront 목표를 편집하고 볼 수 있습니다.

편집 이 기본 옵션입니다.
