---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 방화벽 개요
description: Adobe Workfront은 조직의 네트워크와 통신하므로 해당 통신을 허용하도록 조직의 방화벽을 구성해야 합니다. 방화벽은 조직의 네트워크를 인터넷에서 분리하여 작동시키는 매우 효과적인 보안 조치입니다. 선택된 데이터와 네트워크 트래픽만 조직의 네트워크로 이동하거나 나갈 수 있도록 합니다. 방화벽은 데이터를 보내거나 받는 사이트를 기반으로 데이터를 허용하거나 차단합니다. Adobe Workfront 관리자는 Workfront으로 전송되거나에서 전송한 데이터가 조직의 방화벽을 통과하는지 확인해야 합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 방화벽 개요

Adobe Workfront은 조직의 네트워크와 통신하므로 해당 통신을 허용하도록 조직의 방화벽을 구성해야 합니다. 방화벽은 조직의 네트워크를 인터넷에서 분리하여 작동시키는 매우 효과적인 보안 조치입니다. 선택된 데이터와 네트워크 트래픽만 조직의 네트워크로 이동하거나 나갈 수 있도록 합니다. 방화벽은 데이터를 보내거나 받는 사이트를 기반으로 데이터를 허용하거나 차단합니다. Adobe Workfront 관리자는 Workfront으로 전송되거나에서 전송한 데이터가 조직의 방화벽을 통과하는지 확인해야 합니다.

이 작업은 본질적으로 허용 목록에 추가하다 방화벽을 통해 데이터를 전송하거나 수신할 수 있는 &quot;허용&quot; 사이트의 &quot;목록&quot;인를 통해 수행됩니다. 사이트는 다음 두 가지 방법 중 하나로 식별할 수 있습니다.

* **IP 주소**: 52.31.132.175 같은 일련의 숫자
* **도메인**: www.thisdomain.com에 있는 &quot;thisdomain&quot;과 같은 URL의 일부

Workfront은 웹 커뮤니케이션에 특정 IP 주소 및 도메인을 사용합니다. 조직에서 Workfront을 사용하려면 먼저 허용 목록에 추가하다 조직의에 이러한 코드를 추가해야 합니다.

일반적으로허용 목록에 추가하다는 네트워크 관리자가 구성합니다. 조직의 네트워크 관리자와 함께 방화벽이 이러한 IP 주소를 허용하는지 확인합니다. 네트워크 관리자가 누구인지 모르는 경우 조직의 IT 부서에서 귀하를 올바른 방향으로 안내할 수 있습니다.

>[!IMPORTANT]
>
>Workfront 관리자는 이러한 IP 주소 및 도메인이 조직의에 추가되어 있는지 확인해야 허용 목록에 추가하다 합니다. 직접 추가하지 않더라도 마찬가지입니다. Workfront이 조직의을 구성할 수 허용 목록에 추가하다 없습니다.

## 방화벽 구성을 위한 정보 수집

Workfront에 대한 방화벽을 구성하려면 네트워크 관리자가 추가할 IP 주소와 도메인을 알고 있어야 합니다. 이 정보 중 일부는 Workfront 관리자만 사용할 수 있습니다. Workfront 관리자는 이 정보를 찾아 네트워크 관리자에게 제공해야 합니다.

>[!NOTE]
>
>보안에 대한 우수 사례는 조직에서 사용하고 있는 기능에 연결하는 IP 주소 및 도메인만 추가하는 것입니다. 이 정보를 제공하면 이 모범 사례를 따를 수 있습니다.

네트워크 관리자에게 다음 정보를 제공합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">허용할 특정 IP 주소 및 도메인</td> 
   <td> <p>기사 <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">방화벽 허용 목록에 추가하다 구성</a> 에는 조직에서 해당에 추가해야 하는 IP 주소 및 도메인 목록이 포함되어 허용 목록에 추가하다 있습니다. </p> <p>네트워크 관리자가 "방화벽 구성" 문서에 액세스하지 못할 수 있습니다. 그런 경우에는 제공해야 합니다. 하드(종이) 사본은 인쇄하지 않는 것이 좋습니다. Digital Copy를 사용하면 네트워크 관리자가 주소를 복사하여 붙여넣을 수 있으며, 이는 하드 카피에서 입력하는 것보다 더 빠르고 정확합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">클러스터</td> 
   <td>조직의 클러스터를 찾으려면 다음을 참조하십시오 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">조직의 클러스터 및 Workfront 계획 보기</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 플랜</td> 
   <td> <p>조직의 계획은 다음 중 하나입니다.</p> 
    <ul> 
     <li> <p>기업 </p> </li> 
     <li> <p>비즈니스 </p> </li> 
     <li> <p>Pro </p> </li> 
     <li> <p>팀 </p> </li> 
    </ul> <p>계획을 찾으려면 다음을 참조하십시오 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">조직의 클러스터 및 Workfront 계획을 봅니다.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">도메인</td> 
   <td> <p>도메인을 찾으려면 Workfront에 연결하는 데 사용하는 웹 주소를 확인합니다.</p> <p>예: 웹 주소에서 <code>greatcompany.my.workfront.com</code>, 도메인은 "greatcompany"입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">기타 Adobe Workfront 제품</td> 
   <td> <p>다음 중 하나에 대한 라이센스가 있으면 네트워크 관리자에게 알립니다.</p> 
    <ul> 
     <li> <p>Adobe Workfront 증명</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 통합</td> 
   <td>다음 중 하나를 사용하는 경우 네트워크 관리자에게 문의하십시오.
    <ul>
     <li><p><p>지라용 Workfront</p></p></li>
     <li><p>G Suite용 Workfront</p></li>
     <li><p>Microsoft Teams용 Workfront</p></li>
     <li><p>Workfront for Outlook</p></li>
     <li><p>Salesforce용 Workfront</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 기능</td> 
   <td> <p>다음 중 하나를 사용하는 경우 네트워크 관리자에게 알립니다.</p> 
    <ul> 
     <li> <p>Workfront 테스트 드라이브</p> </li> 
     <li> <p>Workfront 어센트</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>이러한 제품, 통합 또는 기능을 나중에 추가하는 경우 네트워크 관리자에게 문의하여 해당 제품허용 목록에 추가하다를 조정해야 합니다.

### 조직의 클러스터 및 Workfront 계획 보기 {#view-your-organization-s-cluster-and-workfront-plan}

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** 왼쪽 패널에서
1. 클러스터를 보려면 **고객 정보**.

   클러스터가 의 오른쪽 상단 근처에 표시됩니다 **기본 정보** 섹션을 참조하십시오.

   ![](assets/locate-cluster.png)

1. Workfront 계획을 보려면 **라이선스**.

   계획이 페이지 하단에 표시됩니다.

   ![](assets/locate-plan.png)
