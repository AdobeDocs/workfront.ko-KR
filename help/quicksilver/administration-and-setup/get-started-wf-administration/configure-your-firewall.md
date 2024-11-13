---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 허용 목록에 추가하다 방화벽 구성
description: 허용 목록에 추가하다 방화벽 또는 메일 서버가 특정 공급업체에 대해서만 액세스를 허용하도록 구성된 경우 특정 IP 주소를 해당 공급업체에 추가해야 합니다. 이렇게 하면 환경과 Adobe Workfront 서버 간에 통신이 열리고 사용자가 Workfront에서 메시지를 보내고 Active Directory 또는 LDAP와 함께 SSO를 사용할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: df3885233140c5d0af542c8999226f7934c1329f
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 0%

---

# 허용 목록에 추가하다 방화벽 구성

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 Admin Console에 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>조직에서 Adobe Admin Console에 온보딩한 경우 Adobe을 구성하려면 [허용 목록 앱 및 서비스에 사용할 수 있는 도메인](https://helpx.adobe.com/enterprise/kb/network-endpoints.html)을 참조하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 프로시저 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.

>[!NOTE]
>
>조직이 허용 목록에 추가하다를 구성하는 방식은 각 조직마다 고유합니다. IT 팀과 협력하여 조직의 절차를 식별하고 이러한 추가 사항을 구현합니다.

허용 목록에 추가하다 방화벽 또는 메일 서버가 특정 공급업체에 대해서만 액세스를 허용하도록 구성된 경우 특정 IP 주소를 해당 공급업체에 추가해야 합니다. 이렇게 하면 사용자 환경과 Adobe Workfront 서버 간에 통신이 열리고 다음 프로세스가 허용됩니다.

* Workfront 애플리케이션에서 메시지 보내기

  >[!NOTE]
  >
  >조직의 Workfront 인스턴스가 Adobe IMS를 사용하여 활성화된 경우 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

* 사용자 정의 문서 통합 구성 시 문서 웹후크 사용
* Workfront 이벤트 구독 사용

  자세한 내용은 [이벤트 구독 API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680)를 참조하십시오.

또한 전자 메일 메시지가 배달될 때 암호화하려면 특정 포트를 열어야 합니다.

## 사용할 수 있는 Workfront 허용 목록

조직에 Enterprise 플랜이 있는 경우 두 개의 Workfront 허용 목록을 구성할 수도 있습니다.

* **전자 메일 허용 목록**: 사용자가 Workfront에 저장된 전자 메일을 보낼 수 있는 위치를 제어할 수 있습니다. 허용 목록에 추가하다 자세한 내용은 [전자 메일 구성](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)을 참조하십시오.
* **IP 허용 목록**: Workfront에 대한 액세스를 지정한 45개의 IP 주소 또는 IP 주소 범위로 제한하여 Workfront 응용 프로그램에 추가적인 보안 계층을 제공합니다. 자세한 내용은 [IP 주소로 Adobe Workfront에 대한 액세스 제한](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)을 참조하십시오.

## Workfront 클러스터 찾기

프로덕션 환경이 실행되는 클러스터에 따라 방화벽의 IP 주소를 허용 목록에 추가하다에 추가해야 합니다.

조직의 클러스터를 찾으려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **시스템**&#x200B;을 클릭한 다음 **고객 정보**&#x200B;를 선택합니다.
1. 페이지 오른쪽 상단에서 **클러스터 설정** 필드를 찾습니다. 조직의 클러스터가 여기에 나열됩니다.

   CL01은 클러스터 1을 참조하고, CL02는 클러스터 2를 참조합니다.

자세한 내용은 문서 [방화벽 개요](../../administration-and-setup/get-started-wf-administration/firewall-overview.md)에서 [조직의 클러스터 및 Workfront 계획 보기](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) 섹션을 참조하십시오.

## 허용 목록에 추가하다에 추가할 IP 주소

>[!IMPORTANT]
>
>정적 IP 주소로 구성할 수 없어 Workfront이 활성화되지 않은 경우 일부 허용 목록에 추가하다 통합이 작동하지 않습니다. 다음 통합을 사용하려면 허용 목록에 추가하다를 비활성화해야 합니다.
>
>* Google Workspace용 Workfront
>* Outlook용 Workfront
>* Salesforce용 Workfront

* [클러스터 1, 2, 3, 5, 7, 8 및 9를 허용하는 IP 주소](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* 클러스터 4](#ip-addresses-to-allow-for-cluster-4)에 대해 허용할 [IP 주소
* 클러스터 6](#ip-addresses-to-allow-for-cluster-6)을(를) 허용할 [IP 주소
* 테스트 드라이브를 허용할 [IP 주소](#IP%20Addre2)
* [이벤트 구독을 구현할 때 허용할 IP 주소](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [향상된 인증을 허용하는 IP 주소](#ip-addresses-to-allow-for-enhanced-authentication)
* [Workfront Fusion 액세스를 위해 추가할 IP 주소](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Jira용 Workfront 사용을 위해 추가할 IP 주소](#ip-addresses-to-add-for-using-workfront-for-jira)
* [모든 클러스터에 추가할 URL Workfront](#urls-to-add-for-all-clusters-workfront)

### 클러스터 1, 2, 3, 5, 7, 8 및 9를 허용하는 IP 주소 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

프로덕션 환경이 클러스터 1, 2, 3, 5, 7, 8 또는 9에 있는 경우 다음 IP 주소를 허용해야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">SSO, 문서 웹후크 또는 기타 기능의 경우</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 애플리케이션에서 이메일을 받으려면</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>다음 IP 주소에 대한 자세한 내용은 <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">21.1 릴리스와 함께 Adobe Workfront 전자 메일에 대한 새 IP 주소</a>를 참조하세요.</p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 클러스터 4에서 허용할 IP 주소 {#ip-addresses-to-allow-for-cluster-4}

프로덕션 환경이 클러스터 4에 있는 경우 SSO를 위해 다음 IP 주소를 추가하고 Webhook 통합을 문서화하고 Workfront 애플리케이션에서 이메일을 받으십시오.

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

다음 IP 주소에 대한 자세한 내용은 [21.1 릴리스와 함께 Adobe Workfront 전자 메일에 대한 새 IP 주소](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)를 참조하세요.

* 23.251.239.98
* 23.251.239.99

### 클러스터 6을 허용할 IP 주소 {#ip-addresses-to-allow-for-cluster-6}

프로덕션 환경이 클러스터 6에 있는 경우 다음 IP 주소를 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 애플리케이션에서 이메일을 받으려면</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">이메일 서비스를 사용하려면</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Mailgun 이메일 서비스를 사용하려면</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 클러스터 10을 허용할 IP 주소

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

### 테스트 드라이브를 허용할 IP 주소

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">테스트 드라이브를 사용할 때 Workfront 애플리케이션에서 이메일을 받으려면</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">테스트 드라이브를 사용할 때 SSO 및 문서 Webhook 통합</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>사용자가 Workfront에서 이메일을 받으려면 이 주소도 허용 목록에 추가하다에 추가되어야 합니다.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 이벤트 구독을 구현할 때 허용할 IP 주소  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

모든 환경에 대해 다음 IP 주소를 추가하여 Workfront 이벤트 구독에서 페이로드를 받습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 유럽 지역 고객용</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">유럽 이외의 지역 고객</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 향상된 인증을 허용하는 IP 주소 {#ip-addresses-to-allow-for-enhanced-authentication}

미리 보기 또는 프로덕션에 대해 향상된 인증을 사용하려면 다음 IP 주소를 추가하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">환경이 클러스터 1, 2, 3, 5, 7, 8 또는 9에 있는 경우</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">환경이 Cluster 4에 있는 경우</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Workfront Fusion 액세스를 위해 추가할 IP 주소  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Workfront Fusion을 활성화하려면 다음 IP 주소를 허용 목록에 추가하다에 추가하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU 데이터 센터</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 미국 데이터 센터</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Microsoft Azure 클러스터에서</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

또한 조직에서 아웃바운드 네트워크 필터링을 사용하는 경우 허용 목록에 추가하다에 다음 도메인을 추가하여 시스템이 Workfront Fusion에 액세스할 수 있도록 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU 데이터 센터</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 미국 데이터 센터</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] Microsoft Azure 클러스터에서</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>아웃바운드 네트워크 필터링은 흔하지 않습니다. 네트워크 관리자에게 문의하여 허용 목록에 추가하다를 업데이트해야 하는지 확인하십시오.

### Jira용 Workfront 사용을 위해 추가할 IP 주소 {#ip-addresses-to-add-for-using-workfront-for-jira}

Jira 통합에 Workfront을 사용하려면 다음 IP 주소를 허용 목록에 추가하다에 추가하십시오.

회사 서버에서도 jira.workfront.com 도메인에 액세스할 수 있어야 합니다. 이 도메인은 Workfront과 Jira 사이에서 미들웨어 역할을 하므로 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 유럽 지역 고객용</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">유럽 이외의 지역 고객</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront 액세스를 위해 추가할 도메인

조직에서 아웃바운드 네트워크 필터링을 사용하는 경우 허용 목록에 추가하다에 다음 도메인을 추가하여 시스템이 Workfront에 액세스할 수 있도록 합니다.

>[!NOTE]
>
>아웃바운드 네트워크 필터링은 흔하지 않습니다. 네트워크 관리자에게 문의하여 허용 목록에 추가하다를 업데이트해야 하는지 확인하십시오.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/
* *.static.workfront.com

  다음 도메인을 모두 제외하는 정적 도메인입니다. 원하는 경우 개별 도메인을 추가할 수 있습니다.

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com


## 모든 클러스터에 추가할 URL Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">도움말 컨텐츠가 Workfront 환경에 표시되도록 하려면</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof이 모든 클러스터의 Workfront에 액세스할 수 있도록 하려면 모든 환경에 추가하십시오</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Workfront에서 증명을 보는 데 필요</li> 
     <li>*.proofhq.com - Workfront Proof에서 증명을 보는 데 필요</li> 
     <li>*.proofhq.eu - Workfront Proof에서 증명을 보는 데 필요</li> 
    </ul> <p><b>참고</b>:  <p>Workfront Proof용 허용 목록에 추가하다에 IP 주소를 추가하는 것은 지원되지 않습니다. Workfront이 AWS으로 이동한 후 다이내믹했습니다. 대신 Workfront Proof 도메인만 허용하는 것이 좋습니다.</p> <p>허용 목록에 추가하다에 이러한 도메인을 추가하는 데 문제가 있고 대신 IP 주소가 필요한 경우 Workfront 고객 지원 센터에 문의하십시오.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Proof 액세스를 위해 추가할 IP 주소 및 URL

다양한 기능을 사용하려면 다음 IP 주소를 허용 목록에 추가해야 합니다.

* [콜백 및 Webcapture 증명](#for-callbacks-and-webcapture-proofs)
* [발신 이메일의 경우](#for-outgoing-email)

### 콜백 및 웹 캡처 증명 {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US(클러스터 1, 2, 3, 5 및 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU(Cluster 4)</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>참고</b>: DNS 서버 옵션은 더 이상 지원되지 않습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 발신 이메일의 경우 {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US(클러스터 1, 2, 3, 5 및 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU(Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 최상의 Workfront Proof 성능을 위해 열 포트

Workfront Proof에서 증명을 로드하거나 사용할 수 없는 문제가 발생하는 경우 다음 포트를 여십시오.

* 5671
* 5672
* 15671

## 암호화된 이메일을 위해 열 포트

Workfront 애플리케이션의 이메일은 포트 465 및 587을 사용하여 암호화되어 전송됩니다. 메일 서버가 암호화된 이메일을 지원하지 않는 경우 이메일은 포트 25를 사용하여 암호화되지 않은 상태로 전달됩니다.

## Workfront 지원의 이메일 알림

Workfront 지원에서 이메일을 받지 못하는 경우 필요한 Salesforce IP 주소 및 도메인을 추가해야 합니다. 자세한 내용은 허용할 Salesforce IP 주소 및 도메인에 대한 Salesforce 도움말 문서를 참조하십시오.
