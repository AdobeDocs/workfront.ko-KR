---
title: Adobe Workfront Planning 요청 제출
description: 누군가가 Adobe Workfront Planning의 레코드 유형 페이지에서 요청 양식에 대한 링크를 귀하에게 공유하면 요청을 추가하여 요청 양식과 연관된 레코드 유형에 대한 레코드를 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 1%

---

# Adobe Workfront Planning 요청을 제출하여 레코드 생성

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

누군가가 Adobe Workfront Planning의 레코드 유형 페이지에서 요청 양식에 대한 링크를 귀하에게 공유하면 요청을 추가하여 요청 양식과 연관된 레코드 유형에 대한 레코드를 생성할 수 있습니다.

Workfront 사용자와 외부 사용자는 Planning 레코드 유형에 요청을 제출하고 레코드를 생성할 수 있습니다. <!--double check on the external users-->

이 문서에서는 레코드 유형에 새 레코드를 추가하도록 요청을 제출하는 방법에 대해 설명합니다.

작업 영역 관리자가 요청 양식을 만들고 레코드 유형과 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront 계획<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td>
   <td>
<p>임의 </p>  
<p>각 Workfront 계획 계획에 포함된 내용에 대한 자세한 내용은 <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront 가격 및 패키징</a>을 참조하십시오. </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>External, Contributor, Light 또는 Standard 라이센스</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <p>Workfront 사용자인 경우 작업 영역에 대한 이상의 권한 보기</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront의 계획 영역에 액세스하려면 주 메뉴에서 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>
   <p> 하지만 Workfront Planning에 요청을 제출하는 데 계획 영역에 액세스할 필요는 없습니다. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Workfront Planning 요청 양식에 요청을 제출하려면 먼저 다음 조건을 충족해야 합니다.

* Workfront Planning에는 다음이 있어야 합니다.

   * 작업 영역
   * 요청 양식과 연결된 레코드 유형입니다. 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

* 액세스 가능한 방식으로 요청 양식을 링크와 공유해야 합니다. 다음과 같은 시나리오가 있습니다.

   * Workfront 계정이 있는 경우 링크는 내부 직원과만 공유되었으며 작업 영역에 액세스할 수 있습니다. Workfront 외부 사용자는 내부적으로 공유된 링크에 액세스할 수 없습니다.
   * Workfront 계정이 없는 경우 링크가 외부 사용자와 공유되었습니다. Workfront 사용자는 외부 사용자와 공유되는 링크에 액세스할 수도 있습니다.

* 양식에 대한 링크가 만료되지 않아야 합니다.

## Workfront Planning에 요청 제출에 대한 고려 사항

* 양식에 대한 특정 링크 없이 Workfront Planning 요청에 대한 요청 양식에 액세스할 수 없습니다.
* 요청을 Workfront Planning에 제출한 후에는 요청을 편집할 수 없습니다.
* 제출된 각 요청은 사용하는 양식과 관련된 레코드 유형에 대한 레코드를 만듭니다.
* 요청 양식을 제출하여 생성된 레코드는 다른 방법을 통해 추가된 레코드와 구분할 수 없습니다. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

## Workfront Planning에 요청 제출

1. Workfront Planning 레코드 유형에서 사용자와 공유되는 링크로 이동합니다.

1. 양식에서 사용할 수 있는 필드를 업데이트합니다. 별표가 있는 필드는 필수입니다.

   >[!TIP]
   >
   >   Workfront **제목** 필드를 사용할 수 있는 경우 Workfront Planning에 표시되지 않을 수 있습니다. 레코드 유형에 추가될 때 새 레코드를 식별할 수 있도록 요청의 필드를 가능한 한 많이 업데이트하는 것이 좋습니다.

1. **제출**&#x200B;을 클릭합니다.

   양식이 제출되고 새 레코드가 양식과 연결된 레코드 유형에 추가됩니다.





