---
title: 프로젝트 제한 개요
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront에는 프로젝트와 연결할 수 있는 개체 수에 대한 제한이 있습니다. Workfront을 통해 제품 성능을 향상시키고 경험을 향상시키기 위해 프로젝트 제한이 적용됩니다.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 809f1c3629c343a55305c0c617f4974dc05439bf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# 프로젝트 제한 개요

Adobe Workfront에는 프로젝트와 연결할 수 있는 개체 수에 대한 제한이 있습니다. Workfront을 통해 제품 성능을 향상시키고 경험을 향상시키기 위해 프로젝트 제한이 적용됩니다.

프로젝트와 연결된 다음 객체에는 다음과 같은 제한이 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>작업</p></td> 
   <td>  <p>프로젝트당 최대 작업 수는 5,000개입니다. 작업 수가 이 최대값에 도달하면 경고 메시지가 표시됩니다. 최대값에 도달하면 오류 메시지가 표시되고 추가 작업을 프로젝트에 추가할 수 없습니다.</p> <p>이 최대값에 도달하지 않으려면 종결된 작업에 대해 지정된 다른 프로젝트로 폐쇄된 작업을 이동합니다. 이러한 프로젝트에 대한 보고서를 조정해야 할 수 있습니다.</p>

<b>중요 사항</b>

작업에 많은 종속성이 있는 프로젝트의 경우 프로젝트의 작업 수가 최대 5,000개의 허용되는 작업보다 훨씬 적어야 합니다.

프로젝트 타임라인에 영향을 주거나 재계산을 방지할 수 있는 작업 종속성의 몇 가지 예는 다음과 같습니다.

<ul><li>하위 수</li>
   <li>여러 수준의 작업 들여쓰기</li>
   <li>선행 작업 수</li>
   <li>여러 할당</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>문제</p></td> 
   <td>  <p>프로젝트당 최대 문제 수는 10,000개입니다. 문제 수가 이 최대값에 근접하면 경고 메시지가 표시됩니다. 최대값에 도달하면 오류 메시지가 표시되고 추가 문제를 프로젝트에 추가할 수 없습니다.</p> <p>이 최대값에 도달하지 않으려면 종결된 문제에 대해 지정된 다른 프로젝트로 폐쇄된 이동 문제를 해결해야 합니다. 이러한 프로젝트에 대한 보고서를 조정해야 할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>지속 시간</p></td> 
   <td> <p>Workfront이 자동으로 타임라인을 계산하려면 프로젝트의 최대 지속 시간이 15년이어야 합니다. 프로젝트 지속 시간이 최대값에 도달하면 경고 메시지가 표시됩니다. 최대값에 도달하면 경고 메시지가 표시되고 자동 타임라인 계산이 더 이상 발생하지 않습니다.</p> <p>프로젝트 작업 날짜를 조정함으로써 프로젝트 기간이 15년 이하로 축소되는 즉시 자동 타임라인 계산이 다시 시작됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>타임라인 계산</p></td> 
   <td>Workfront은 6개월 동안 업데이트되지 않은 프로젝트에 대해 자동 타임라인 계산을 수행하지 않으며 업데이트가 수행되기 전까지 다시 시작하지 않습니다.<p>3개월 동안 업데이트되지 않은 프로젝트의 경우 Workfront에서는 야간 대신 매주 타임라인 계산을 수행합니다.</p><p>프로젝트 타임라인 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">프로젝트 타임라인 다시 계산</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->