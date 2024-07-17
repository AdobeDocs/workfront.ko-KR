---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 비즈니스 사례 재무 필드 개요
description: 비즈니스 사례 하위 탭에는 프로젝트의 재무 필드가 포함됩니다. 일부 재무 필드가 값을 가지려면 비즈니스 사례의 해당 영역을 완료해야 합니다.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 2%

---

# 비즈니스 사례 재무 필드 개요

비즈니스 사례 하위 탭에는 프로젝트의 재무 필드가 포함됩니다. 일부 재무 필드가 값을 가지려면 비즈니스 사례의 해당 영역을 완료해야 합니다.  

비즈니스 사례에는 다음 프로젝트 재무 필드가 표시됩니다.

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
   <td> <p>스코어카드에 따른 프로젝트 정렬을 표시합니다. 높은 백분율 값은 프로젝트가 조직의 목적 및 목표와 잘 일치함을 나타냅니다. <br>스코어카드 사용에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">스코어카드 만들기</a>를 참조하십시오.</p> <p>이 필드는 비즈니스 사례 요약 영역에 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>예산 비용</td> 
   <td> <p>프로젝트가 시작될 때 프로젝트와 연결될 것으로 예상되는 총 비용입니다.</p> <p>프로젝트의 예산 원가는 다음 공식에 의해 계산됩니다.<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront은 리소스 플래너의 예산 시간을 사용하여 예산 인건비를 계산합니다.<br>예산 비용 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">예산 비용 계산</a>을 참조하세요. </p> <p>이 필드는 비즈니스 사례 요약 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>예산 경비</td> 
   <td> <p>프로젝트에 대한 모든 비용의 예산 비용. </p> <p>이는 다음 공식에 의해 계산됩니다.</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>경비 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">프로젝트 경비 관리 </a>을(를) 참조하십시오.</p> <p>이 필드는 경비 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>예산 인건비</td> 
   <td> <p>프로젝트에서 작업을 완료하기 위해 할당된 리소스와 관련된 비용입니다.</p> <p>프로젝트의 예산 인건비는 다음 공식에 의해 계산됩니다.<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront은 리소스 플래너의 예산 시간을 사용하여 예산 인건비를 계산합니다.<br>예산 인건비 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트 예산 인건비 및 예산 시간 이해</a>를 참조하십시오.</p> <p>이 필드는 비즈니스 사례의 리소스 예산 책정 영역에 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>경비 계획 비용</td> 
   <td> <p>이는 예산 경비와 동일합니다. </p> <p>주: 경비 계획 원가가 프로젝트의 계획 원가와 다릅니다. 비용 계획된 비용은 프로젝트의 비용에 대한 계획된 금액으로 계산되지만, 계획된 비용은 프로젝트의 계획된 시간을 사용하여 계산됩니다. </p> <p>이 필드는 각 경비의 경비 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>순 가치</td> 
   <td> <p>이는 편익을 계산하고 비용을 제거한 후 프로젝트의 총 기대 가치이다.</p> <p>프로젝트의 순 가치(Net Value)는 다음 공식에 의해 계산됩니다.<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>순 가치 계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">순 가치 계산</a>을 참조하십시오.<br></p> <p>이 필드는 비즈니스 사례 요약 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>계획된 이익</td> 
   <td>이 프로젝트가 완료될 때 조직의 금전적 혜택에 대한 수동 예상. 통화는 얼마든지 가능하며 사용자와 관리하는 각 프로젝트에 따라 다릅니다. 계획된 혜택은 음수 값을 가질 수 없습니다. 이 필드는 비즈니스 사례 요약 영역에 표시되며 비즈니스 사례의 프로젝트 정보 영역에서 편집할 수 있습니다. </td> 
  </tr> 
  <tr> 
   <td>잠재적 위험 비용</td> 
   <td> <p>이는 프로젝트에 수반되는 모든 위험의 잠재적 비용이다. </p> <p>이는 다음 공식을 사용하여 계산됩니다.</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>프로젝트의 위험에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">프로젝트의 위험 만들기 및 편집</a>을 참조하세요.</p> <p>이 필드는 비즈니스 사례 요약 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>잠재적 위험</td> 
   <td> <p>비즈니스 사례 요약에서, 이는 모든 위험이 발생해야 하는 경우, 그 확률에 따라 발생하는 비용의 금액입니다. 예를 들어, 위험의 잠재적 비용이 $100이고 발생 확률이 10%인 경우, 잠재적 위험은 $10이다. 비즈니스 사례 요약의 잠재적 위험은 다음 공식에 의해 계산됩니다.</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 모든 위험에 대해. </p> </td> 
  </tr> 
  <tr> 
   <td>위험 완화 비용</td> 
   <td> <p>예상 위험에 대한 완화 플랜 비용은 프로젝트에서 발생할 수 있습니다.<br>프로젝트 위험에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">프로젝트 위험 만들기 및 편집</a>을 참조하세요.</p> <p>이 필드는 프로젝트에 지정된 각 위험에 대한 위험 영역에 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>위험 1개에 대한 잠재적 비용</td> 
   <td> <p>프로젝트에 정의된 위험이 확률과 관계없이 실제로 발생할 경우의 예상 재정 비용이다. </p> <p>비즈니스 사례의 위험 영역에 있는 각 위험에 표시되는 수동으로 업데이트된 필드입니다. </p> </td> 
  </tr> 
  <tr> 
   <td>총 잠재적 비용 위험</td> 
   <td> <p>이는 프로젝트에 정의된 모든 위험이 실제로 발생했을 때의 총 예상 재무 비용입니다. </p> <p>이는 다음 공식에 의해 계산됩니다.</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>비즈니스 사례의 위험 영역 제목 옆에 통화 번호로 표시됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
