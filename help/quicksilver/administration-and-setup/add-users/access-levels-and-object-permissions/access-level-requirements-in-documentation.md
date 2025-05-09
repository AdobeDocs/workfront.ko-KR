---
title: Workfront 설명서의 액세스 요구 사항
content-type: reference
product-area: system-administration
keywords: 액세스,수준,시스템,관리자,플래너,작업자,검토자,요청자,외부,사용자
navigation-topic: access-levels
description: Workfront 설명서 방법 문서에는 해당 절차에 필요한 액세스 및 권한을 설명하는 표가 포함되어 있습니다. 이 문서에서는 액세스 요구 사항 테이블에 대해 자세히 설명하고 자세한 내용을 볼 수 있는 링크를 제공합니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 1%

---

# Workfront 설명서의 액세스 요구 사항

Workfront 설명서 방법 문서에는 해당 절차에 필요한 액세스 및 권한 요구 사항을 설명하는 표가 포함되어 있습니다. 이 액세스 요구 사항 테이블을 사용하면 Workfront에서 특정 작업을 수행할 수 있는지 여부 또는 수행할 수 없는 이유를 이해할 수 있습니다. 이 문서에서는 액세스 요구 사항 테이블의 각 요소에 대해 설명하고, 문제 해결 팁과 보다 심층적인 정보에 대한 링크를 제공합니다.

특정 문서의 액세스 요구 사항 테이블에 행이 없으면 해당 작업에 대한 해당 형식의 요구 사항이 없습니다.

일부 행에는 &quot;새로 만들기&quot; 및 &quot;현재&quot;라는 레이블이 지정된 정보가 포함되어 있습니다. 일부 조직은 새로운 모델로 운영되고 다른 조직은 여전히 현재 모델을 사용하고 있는 상황에서 Workfront이 새로운 가격 및 패키징 모델로 전환하고 있기 때문이다. 조직에서 사용하는 모델을 확인하려면 Workfront 관리자에게 문의하십시오. 이 문서의 [액세스 요구 사항 테이블](#the-access-requirements-table) 섹션에서 자세한 내용과 정보 링크를 찾을 수 있습니다.

>[!NOTE]
>
>이 표의 필드 중 어떤 것이 사용자에게 적용되는지에 대한 질문이 있는 경우 Workfront 관리자에게 문의하십시오.

## 액세스 요구 사항 테이블

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> Adobe Workfront 플랜은 조직이 구매한 기능 세트를 참조합니다. 대부분의 Workfront 기능은 모든 계획에서 사용할 수 있으며 몇 가지 예외를 제외하고 대부분 전략 계획 및 엔터프라이즈 제어와 관련되어 있습니다. 
   <ul><li>조직이 새 패키징 모델이나 현재 패키징 모델에 있는지 여부를 포함하여 조직이 사용하는 Adobe Workfront 계획을 알아보려면 Workfront 관리자에게 문의하십시오.</li>
   <li>Workfront 관리자가 조직의 Workfront 계획을 찾는 방법에 대한 지침은 <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">조직의 클러스터 및 Workfront 계획 보기</a>를 참조하십시오.</li><li>새로운 Workfront 플랜에 대한 자세한 내용은 <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront 가격 및 패키징</a>을 참조하십시오.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> Adobe Workfront 라이선스는 사용자에게 할당된 라이선스에 포함된 Workfront 기능 집합을 가리킵니다. 예를 들어 한 명의 사용자는 완료 작업 항목 표시 및 로깅 시간을 포함하는 라이선스를 보유하고 있는 반면 다른 사용자는 에셋을 승인하거나 요청을 제출할 수만 있는 라이선스를 보유하고 있습니다. <p> 
   <ul>
   <li>할당된 라이선스를 확인하려면 Workfront 관리자에게 문의하십시오.</li>
   <li>Adobe Workfront은 새로운 가격 및 패키징 모델로 전환하고 있습니다. 라이센스에 대한 자세한 내용은 다음을 참조하십시오.
   <ul>
   <li>새로 만들기: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">새 라이선스 개요</a></li>
   <li>현재: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">라이선스 개요</a></li></ul></li>
   <li>올바른 액세스 수준을 가지고 있지만 여전히 액세스 권한이 없는 경우 Workfront 관리자가 액세스 수준에서 추가 제한을 설정하는지 확인하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Workfront은 Workfront 외에도 구매할 수 있는 몇 가지 제품을 제공합니다.
   <p>이러한 추가 제품 내에서 수행되는 절차를 설명하는 문서는 여기에 필수 제품을 나열합니다.</p>
   <ul>
   <li>Adobe Experience Manager Assets 또는 Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Workfront 시나리오 플래너</li>
   <li>Workfront Planning</li>
   </ul>
   <p>조직에서 이러한 추가 제품 중 하나를 구입했는지 확인하려면 Workfront 관리자에게 문의하십시오.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준</td> 
   <td> 액세스 수준은 Workfront에서 수행할 수 있는 작업에 대한 권한 집합이며, Workfront 관리자가 설정합니다. <p>Workfront에는 Workfront 라이선스에 해당하는 기본 제공 액세스 수준이 있지만 Workfront 관리자는 더 많은 액세스 수준을 만들어 조직에 필요한 권한 세트를 더 정확하게 반영할 수 있습니다.</p>
   <ul>
    <li>Adobe Workfront은 새로운 가격 및 패키징 모델로 전환하고 있습니다. 각 모델의 액세스 수준에 대한 자세한 내용은 다음을 참조하십시오.
   <ul>
   <li>새로 만들기: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">새 액세스 수준 개요</a></li>
   <li>현재: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">액세스 수준 개요</a></li></ul></li>
    <li>액세스 수준에 대한 세부 정보를 확인하려면 Workfront 관리자에게 문의하십시오</li>
    <li>Workfront 관리자인 경우 액세스 수준의 특정 개체에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront 액세스 권한 구성</a>을 참조하십시오.</li>  
   <li>올바른 액세스 수준을 가지고 있지만 여전히 액세스 권한이 없는 경우 Workfront 관리자가 액세스 수준에서 추가 제한을 설정하는지 확인하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td><p>개체 사용 권한은 개별 Workfront 개체를 만들 때 또는 개체를 사용자와 공유할 때 필요한 액세스 권한을 의미합니다. 예를 들어 액세스 수준에서 프로젝트를 볼 수 있더라도 프로젝트를 보려면 특정 프로젝트에 대한 보기 액세스 권한이 있어야 합니다. 액세스 요구 사항 테이블의 이 섹션에서는 문서에서 작업을 수행하는 데 필요한 특정 객체 권한에 대해 설명합니다.</p>
   <p>개체에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청</a>을 참조하십시오.</p><p>개체 공유에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">개체 공유</a>를 참조하십시오.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">레이아웃 템플릿</td> 
   <td><p>레이아웃 템플릿은 기본 메뉴에서 볼 수 있는 항목을 제어하며 Workfront 관리자가 구성합니다. 이 줄에서는 작업을 수행하기 위해 주 메뉴에 포함되어야 하는 Workfront의 특정 영역을 확인합니다.</p><p>일반적으로 문서에서 메인 메뉴의 영역을 클릭하도록 지시하고 해당 영역이 메인 메뉴에 표시되지 않으면 Workfront 관리자에게 문의하여 해당 영역을 사용할 수 있는지 확인하십시오.</p><p>
   Workfront 관리자가 기본 메뉴를 구성하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">레이아웃 템플릿을 사용하여 기본 메뉴 사용자 지정</a>을 참조하십시오.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion 라이선스</td> 
   <td>Adobe Workfront Fusion에는 Workfront과 다른 별도의 라이선스 모델이 있습니다. 
   <ul><li>현재: 현재 라이선스 모델은 수행된 작업 수를 기반으로 하며, 조직에서 수행할 수 있는 작업에 대해서는 제한이 없습니다. </li>
   <li>레거시: 레거시 라이선스는 시나리오가 서드파티 애플리케이션에 연결할 수 있는지 또는 시나리오가 Workfront 자동화에만 사용되는지 여부를 기반으로 합니다. </li>
   </ul>
   Fusion 라이선스에 대한 자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion 라이선스</a>를 참조하십시오.
   </td> 
  </tr> 
 </tbody> 
</table>
