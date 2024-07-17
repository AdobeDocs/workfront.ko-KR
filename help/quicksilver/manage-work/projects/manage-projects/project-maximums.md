---
title: 프로젝트 제한 개요
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront에는 프로젝트와 연결할 수 있는 개체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront 환경을 개선하기 위해 프로젝트 제한이 적용됩니다.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 프로젝트 제한 개요

Adobe Workfront에는 프로젝트와 연결할 수 있는 개체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront 환경을 개선하기 위해 프로젝트 제한이 적용됩니다.

프로젝트와 연관된 다음 객체에는 다음과 같은 제한이 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>작업</p></td> 
   <td>  <p>프로젝트당 최대 작업 수는 5,000개입니다. 작업 수가 이 최대값에 근접하면 경고 메시지가 표시됩니다. 최대값에 도달하면 오류 메시지가 표시되고 프로젝트에 추가 작업을 추가할 수 없습니다.</p> <p>이 최대값에 도달하지 않도록 닫힌 작업을 닫힌 작업으로 지정된 다른 프로젝트로 이동합니다. 이러한 프로젝트에 대한 보고서를 조정해야 할 수 있습니다.</p>

<b>중요</b>

작업에 많은 종속성이 있는 프로젝트의 경우 타임라인 계산 시 또는 프로젝트에서 작업할 때 성능이 저하될 수 있습니다.

이러한 이유로 복잡한 종속성이 있는 프로젝트의 작업 수는 최대 허용 작업 5,000개보다 훨씬 적어야 합니다.

프로젝트의 타임라인을 다시 계산하는 데 영향을 주거나 영향을 주지 않는 작업 종속 기능의 몇 가지 예는 다음과 같습니다.

<ul><li>하위 수</li>
   <li>여러 수준의 작업 들여쓰기</li>
   <li>전임 작업 수</li>
   <li>여러 할당</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>문제</p></td> 
   <td>  <p>프로젝트당 최대 문제 수는 10,000개입니다. 문제 수가 이 최대값에 근접하면 경고 메시지가 표시됩니다. 최대값에 도달하면 오류 메시지가 표시되고 프로젝트에 추가 문제를 추가할 수 없습니다.</p> <p>이 최대값에 도달하지 않도록 닫힌 문제를 닫힌 문제로 지정된 다른 프로젝트로 이동합니다. 이러한 프로젝트에 대한 보고서를 조정해야 할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>기간</p></td> 
   <td> <p>Workfront이 타임라인을 자동으로 계산하려면 프로젝트의 최대 기간이 15년이어야 합니다. 프로젝트 기간이 최대값에 가까워지면 경고 메시지가 표시됩니다. 최대값에 도달하면 경고 메시지가 표시되고 자동 타임라인 계산이 더 이상 발생하지 않습니다.</p> <p>프로젝트의 작업 날짜를 조정하여 프로젝트의 기간이 15년 이하로 감소하면 자동 타임라인 계산이 재개됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>타임라인 계산</p></td> 
   <td>Workfront은 6개월 동안 업데이트되지 않은 프로젝트에 대해 자동 타임라인 계산을 수행하지 않으며 업데이트가 이루어질 때까지 다시 시작하지 않습니다.<p>3개월 동안 업데이트되지 않은 프로젝트의 경우 Workfront은 매일 밤 대신 매주 타임라인 계산을 수행합니다.</p><p>프로젝트 타임라인 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">프로젝트 타임라인 다시 계산</a>을 참조하십시오. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->