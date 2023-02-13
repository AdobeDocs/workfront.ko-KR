---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 비즈니스 사례 재무 필드 개요
description: 비즈니스 사례 하위 탭에는 프로젝트의 재무 필드가 포함됩니다. 일부 재무 필드에 값이 있으려면 비즈니스 케이스의 해당 영역을 완료해야 합니다.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# 비즈니스 사례 재무 필드 개요

비즈니스 사례 하위 탭에는 프로젝트의 재무 필드가 포함됩니다. 일부 재무 필드에 값이 있으려면 비즈니스 케이스의 해당 영역을 완료해야 합니다.  

업무 사례에는 다음 프로젝트 재무 필드가 표시됩니다.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">필드 이름</th> 
   <th scope="col">설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>정렬됨 </td> 
   <td> <p>스코어카드에 따라 프로젝트의 정렬을 표시합니다. 높은 비율의 값은 프로젝트가 조직의 목적 및 목표에 잘 정렬되었음을 나타냅니다. <br>스코어카드 사용에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">스코어카드 만들기</a>.</p> <p>이 필드는 업무 사례 요약 영역에 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>예산 비용</td> 
   <td> <p>프로젝트를 시작할 때 프로젝트와 연관될 것으로 예상되는 총 비용.</p> <p>프로젝트에 대한 예산책정된 원가는 다음 공식으로 계산됩니다.<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront은 Resource Planner의 예산책정된 시간을 사용하여 예산책정된 노무비를 계산합니다.<br>예산책정된 원가 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">예산책정된 비용 계산</a>. </p> <p>이 필드는 업무 사례 요약 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>예산 경비</td> 
   <td> <p>프로젝트에 드는 모든 비용의 예산책정된 비용입니다. </p> <p>이것은 다음 수식으로 계산됩니다.</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>비용 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">프로젝트 비용 관리 </a>.</p> <p>이 필드는 비용 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>예산 인건비</td> 
   <td> <p>프로젝트에서 작업을 완료하기 위해 지정된 리소스와 연관된 비용입니다.</p> <p>프로젝트에 대한 예산책정된 노무비는 다음 공식으로 계산됩니다.<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Workfront은 Resource Planner의 예산책정된 시간을 사용하여 예산책정된 노무비를 계산합니다.<br>예산책정된 노무비 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해</a>.</p> <p>이 필드는 Business Case의 Resource Budgeting 영역에 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>비용 계획 비용</td> 
   <td> <p>예산책정된 비용 원가와 동일합니다. </p> <p>참고: 비용 계획 원가는 프로젝트의 계획 원가와 다릅니다. 비용 계획 원가는 프로젝트의 계획 비용 금액을 계산하지만 계획 원가는 프로젝트의 계획 시간을 사용하여 계산됩니다. </p> <p>이 필드는 각 비용에 대해 비용 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>순 가치</td> 
   <td> <p>이 값은 이익을 계산하고 비용을 제거한 후 프로젝트의 총 예상 값입니다.</p> <p>프로젝트에 대한 순 값은 다음 공식으로 계산됩니다.<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>순 값 계산에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">순 값 계산</a>.<br></p> <p>이 필드는 업무 사례 요약 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>계획된 이익</td> 
   <td>이 프로젝트가 완료되면 조직에 대한 금전적 혜택에 대한 수동 추정입니다. 모든 통화 금액일 수 있으며 사용자와 관리하는 각 프로젝트에 따라 다릅니다. 계획된 혜택은 음수 값을 가질 수 없습니다. 이 필드는 Business Case Summary 영역에 표시되며 Business Case의 Project Info 영역에서 편집할 수 있습니다. </td> 
  </tr> 
  <tr> 
   <td>잠재적 위험 비용</td> 
   <td> <p>이것은 프로젝트에 대한 모든 위험의 잠재적 비용입니다. </p> <p>다음 공식을 사용하여 계산됩니다.</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>프로젝트의 위험에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">프로젝트에서 위험 요소 생성 및 편집</a>.</p> <p>이 필드는 업무 사례 요약 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>잠재적 위험</td> 
   <td> <p>Business Case Summary에서 모든 위험 요소가 발생할 경우 그 확률을 기준으로 해당 위험 요소의 비용이 차지하는 금액입니다. 예를 들어, 잠재적 비용이 $100이고 발생 확률이 10%인 위험의 경우 잠재적 위험은 $10입니다. Business Case Summary의 잠재적 위험 요소는 다음 공식에 의해 계산됩니다.</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 모든 위험에 대해 </p> </td> 
  </tr> 
  <tr> 
   <td>위험 완화 비용</td> 
   <td> <p>프로젝트에서 발생할 수 있는 위험에 대한 완화 계획의 비용입니다.<br>프로젝트의 위험에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">프로젝트에서 위험 요소 생성 및 편집</a>.</p> <p>이 필드는 프로젝트에 지정된 각 위험에 대한 위험 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>위험 요소를 위한 잠재적 비용</td> 
   <td> <p>프로젝트에 정의된 위험들이 실제로 발생할 경우의 예상 재정 비용입니다. 그 위험성에 관계없이 말입니다. </p> <p>비즈니스 사례의 위험 영역에 각 위험에 표시되는 수동으로 갱신된 필드입니다. </p> </td> 
  </tr> 
  <tr> 
   <td>위험 총 잠재적 비용</td> 
   <td> <p>이는 실제 발생한 프로젝트에서 정의한 모든 위험들의 총 예상 재무 비용입니다. </p> <p>이것은 다음 수식으로 계산됩니다.</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>비즈니스 케이스의 위험 영역 제목 옆에 통화 번호로 표시됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
