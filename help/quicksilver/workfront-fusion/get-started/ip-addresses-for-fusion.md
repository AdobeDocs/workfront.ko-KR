---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion 액세스용 IP 주소
description: Adobe Workfront Fusion에는 Adobe Workfront 라이센스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 800cf889ff2729fca0c9d75d0ace0ecc1ee53a79
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에 액세스하기 위한 IP 주소

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion]에는 [!DNL Adobe Workfront license] 외에 [!DNL Adobe Workfront Fusion] 라이선스가 필요합니다.

허용 목록에 추가하다 방화벽 또는 메일 서버가 특정 공급업체에 대한 액세스만 허용하도록 구성된 경우 해당 공급업체에 특정 IP 주소를 추가하여 해당 환경과 [!DNL Adobe Workfront Fusion] 간에 열린 통신을 허용해야 합니다.

모든 Fusion IP 주소 및 도메인을 허용 목록에 추가하다에 추가하거나, 클러스터를 찾아 해당 클러스터의 IP 주소 및 도메인만 추가할 수 있습니다.

## 모든 Fusion IP 주소 및 도메인 추가

다음 IP 주소를 허용 목록에 추가합니다.

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

또한 조직에서 아웃바운드 네트워크 필터링을 사용하는 경우 허용 목록에 추가하다에 다음 도메인을 추가하여 시스템이 Workfront Fusion에 액세스할 수 있도록 합니다. 웹후크에 사용됩니다.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## 클러스터에 대해서만 Fusion IP 주소 및 도메인 추가

### 데이터 센터 식별

IP 주소는 데이터가 저장되는 위치에 따라 다릅니다.

URL을 통해 Fusion에 액세스하는 경우 URL을 검사하여 데이터 센터를 찾을 수 있습니다.

| URL | 데이터 센터 |
| --- | --- |
| `https://app.workfrontfusion.com/` | 미국 데이터 센터 |
| `https://app-eu.workfrontfusion.com/` | EU 데이터 센터 |
| `https://app-az.workfrontfusion.com/` | Azure 데이터 센터 |

experience.adobe.com을 통해 Fusion에 액세스하는 경우 브라우저에서 네트워크 탭을 확인하여 데이터 센터를 식별할 수 있습니다.

| URL | 데이터 센터 |
| --- | --- |
| `https://fusion.adobe.com`에 대한 호출 | 미국 데이터 센터 |
| `https://eu.fusion.adobe.com`에 대한 호출 | EU 데이터 센터 |
| `https://az.fusion.adobe.com`에 대한 호출 | Azure 데이터 센터 |

### 데이터 센터의 IP 주소 및 도메인 추가

[!DNL Workfront Fusion]이(가) 시스템에 액세스할 수 있도록 하려면 다음 IP 주소를 허용 목록에 추가하다에 추가하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU 데이터 센터</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 미국 데이터 센터</p> </td> 
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
   <td role="rowheader">[!DNL Adobe Workfront] EU 데이터 센터</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 미국 데이터 센터</p> </td> 
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

조직 허용 목록 허용 목록에 추가하다 설정에 대한 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.
