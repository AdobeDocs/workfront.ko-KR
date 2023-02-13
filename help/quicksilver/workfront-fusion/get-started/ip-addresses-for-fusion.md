---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion 액세스를 위한 IP 주소
description: Adobe Workfront Fusion에는 Adobe Workfront 라이선스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# 액세스하기 위한 IP 주소 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 를 사용하려면 [!DNL Adobe Workfront Fusion] 라이센스 [!DNL Adobe Workfront license].

방화벽이나 메일 서버가 특정 공급업체에만 액세스할 수 있도록 구성되어 있는 경우, 해당에 특정 IP 주소허용 목록에 추가하다를 추가하여 환경과 [!DNL Adobe Workfront Fusion].

다음 IP 주소를에 허용 목록에 추가하다 추가하여 [!DNL Workfront Fusion] 시스템에 액세스하려면

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
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

또한 조직에서 아웃바운드 네트워크 필터링을 사용하는 경우 시스템에 다음 도메인을 추가하여 허용 목록에 추가하다 시스템이 Workfront Fusion에 액세스할 수 있도록 합니다.

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
 </tbody> 
</table>

>[!NOTE]
>
>아웃바운드 네트워크 필터링은 일반적입니다. 네트워크 관리자에게 문의하여에 맞게 업데이트할 허용 목록에 추가하다 필요가 있는지 확인하십시오.

조직 설정에 대한 자세한 내용은 다음을 허용 목록에 추가하다 참조하십시오 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
