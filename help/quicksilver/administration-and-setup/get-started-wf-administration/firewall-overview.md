---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 방화벽 개요
description: Adobe Workfront은 조직의 네트워크와 통신하므로 해당 통신을 허용하도록 조직의 방화벽을 구성해야 합니다. 방화벽은 인터넷으로부터 조직의 네트워크를 분리하여 기능하는 매우 효과적인 보안 조치입니다. 선택한 데이터 및 네트워크 트래픽만 조직의 네트워크로 이동하거나 네트워크의 외부로 이동할 수 있습니다. 방화벽은 데이터를 전송하거나 수신하는 사이트를 기준으로 데이터를 허용하거나 차단합니다. Adobe Workfront 관리자는 Workfront으로 또는 에서 전송된 데이터가 조직의 방화벽을 통과할 수 있는지 확인해야 합니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: 1c11be2d6de471bf456107b5c86a599766583f74
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# 방화벽 개요

Adobe Workfront은 조직의 네트워크와 통신하므로 해당 통신을 허용하도록 조직의 방화벽을 구성해야 합니다. 방화벽은 인터넷으로부터 조직의 네트워크를 분리하여 기능하는 매우 효과적인 보안 조치입니다. 선택한 데이터 및 네트워크 트래픽만 조직의 네트워크로 이동하거나 네트워크의 외부로 이동할 수 있습니다. 방화벽은 데이터를 전송하거나 수신하는 사이트를 기준으로 데이터를 허용하거나 차단합니다. Adobe Workfront 관리자는 Workfront으로 또는 에서 전송된 데이터가 조직의 방화벽을 통과할 수 있는지 확인해야 합니다.

이는 본질적으로 방화벽을 통해 데이터를 전송하거나 수신할 수 있는 사이트의 &quot;목록&quot;인 허용 목록에 추가하다를 통해 수행됩니다. 사이트는 다음 두 가지 방법 중 하나로 식별할 수 있습니다.

* **IP 주소**: 52.31.132.175과(와) 같은 일련의 숫자
* **도메인**: URL의 일부(예: `thisdomain`의 `www.thisdomain.com`).

Workfront은 웹 통신에 특정 IP 주소 및 도메인을 사용합니다. 조직에서 Workfront을 사용하려면 먼저 조직의 허용 목록에 추가하다에 추가해야 합니다.

일반적으로 네트워크 관리자가 허용 목록을 구성합니다. 조직의 네트워크 관리자와 협력하여 방화벽에서 이러한 IP 주소를 허용하는지 확인하십시오. 네트워크 관리자가 누구인지 모르는 경우 조직의 IT 부서에서 올바른 방향을 가리킬 수 있습니다.

>[!IMPORTANT]
>
>Workfront 관리자는 이러한 IP 주소 및 도메인이 조직의 허용 목록에 추가하다에 추가되었는지 확인해야 합니다. 직접 추가하지 않더라도 마찬가지입니다. Workfront에서 조직의 허용 목록에 추가하다를 구성할 수 없습니다.

## 방화벽 구성을 위한 정보 수집

Workfront에 대한 방화벽을 구성하려면 네트워크 관리자가 추가할 IP 주소 및 도메인을 알아야 합니다. 이 정보 중 일부는 Workfront 관리자만 사용할 수 있습니다. Workfront 관리자는 이 정보를 찾아 네트워크 관리자에게 제공해야 합니다.

>[!NOTE]
>
>보안에 대한 가장 좋은 방법은 조직에서 현재 사용 중인 기능에 연결하는 IP 주소 및 도메인만 추가하는 것입니다. 이 정보를 제공하면 이 모범 사례를 따를 수 있습니다.

네트워크 관리자에게 다음 정보를 제공합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">허용할 특정 IP 주소 및 도메인</td> 
   <td> <p>허용 목록에 추가하다 허용 목록에 추가하다 문서 <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">방화벽 구성</a>에는 조직에서 방화벽에 추가해야 하는 IP 주소 및 도메인 목록이 포함되어 있습니다. </p> <p>허용 목록에 추가하다 네트워크 관리자가 "방화벽 구성" 문서에 액세스할 수 없습니다. 그런 경우 제공해야 합니다. 하드(용지) 사본은 인쇄하지 않는 것이 좋습니다. 디지털 복사본을 사용하면 네트워크 관리자가 주소를 복사하고 붙여넣을 수 있으므로 하드 복사본으로 입력하는 것보다 빠르고 정확합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">내 클러스터</td> 
   <td>조직의 클러스터를 찾으려면 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">조직의 클러스터 및 Workfront 계획 보기</a>를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 플랜</td> 
   <td> <p>조직의 계획을 찾으려면 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">조직의 클러스터 및 Workfront 계획 보기</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">내 도메인</td> 
   <td> <p>도메인을 찾으려면 Workfront에 연결하는 데 사용하는 웹 주소를 확인하십시오.</p> <p>예: 웹 주소 <code>greatcompany.my.workfront.com</code>에서 도메인은 "greatcompany"입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">기타 Adobe Workfront 제품</td> 
   <td> <p>다음 중 하나에 대한 라이센스가 있으면 네트워크 관리자에게 문의하십시오.</p> 
    <ul> 
     <li> <p>Adobe Workfront 증명</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 통합</td> 
   <td>다음 중 하나를 사용하는 경우 네트워크 관리자에게 알립니다.
    <ul>
     <li><p>Microsoft Teams용 Workfront</p></li>
     <li><p>Outlook용 Workfront</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 기능</td> 
   <td> <p>다음을 사용하는 경우 네트워크 관리자에게 알립니다.</p> 
    <ul> 
     <li> <p>Workfront 테스트 드라이브</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>이러한 제품, 통합 또는 기능을 나중에 추가하는 경우 네트워크 관리자에게 문의하여 허용 목록을 조정해야 합니다.

### 조직의 클러스터 및 Workfront 계획 보기 {#view-your-organization-s-cluster-and-workfront-plan}

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** 클릭
1. 클러스터를 보려면 **고객 정보**&#x200B;를 선택하세요.

   클러스터가 **기본 정보** 섹션의 오른쪽 상단 근처에 표시됩니다.

   ![클러스터 찾기](assets/locate-cluster.png)

1. Workfront 플랜을 보려면 **라이선스**&#x200B;를 선택하세요.

   플랜이 페이지의 오른쪽 상단 근처에 표시됩니다.

   ![계획 찾기](assets/locate-plan.png)
