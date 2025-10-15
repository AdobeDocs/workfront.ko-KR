---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '오류 메시지: 잘못된 매개변수: 전환 값'
description: '기존 사용자 정의 양식에서 사용자 정의 필드의 형식을 변경하려고 하면 ''잘못된 매개변수: 전환 값 &grave;&lt;...&gt;&grave;'' 오류 메시지가 표시됩니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 2%

---

# 오류 메시지: 잘못된 매개변수: 전환 값

## 문제

기존 사용자 정의 양식에서 사용자 정의 필드의 형식을 변경하려고 할 때 다음과 같은 오류 메시지가 표시됩니다. &quot;잘못된 매개변수: 전환 값 &quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 원인

이 메시지는 다음 시나리오에서 발생합니다.

예를 들어 텍스트 형식의 사용자 지정 필드가 있습니다.  이제 사용자 정의 필드의 형식을 통화로 변경합니다. Adobe Workfront 인스턴스 어딘가에 이 필드가 개체에 이미 첨부되어 있고 개체에 이미 지정된 정보가 있습니다. 하나 이상의 해당 필드에 있는 기존 정보의 형식이 이미 텍스트로 지정되어 있습니다. 따라서 필드의 형식은 통화로 변경할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>액세스 권한 편집 대상:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 캘린더 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 솔루션

다음을 수행합니다.

1. 이 필드가 사용자 지정 Forms과 연결되어 있을 수 있는 모든 개체에 대한 보고서를 작성합니다.\
   보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

1. 편집하려는 사용자 정의 필드를 보고서 보기에 포함하면 이 필드가 텍스트 값으로 채워진 오브젝트를 확인할 수 있습니다.
1. 텍스트 형식으로 표시되는 오브젝트의 사용자 정의 필드 값을 수정하고 [통화] 형식의 값을 지정한 다음 사용자 정의 양식의 형식 필드를 다시 변경해 보십시오.\
   또는\
   이미 텍스트 형식의 정보로 채워진 필드 값이 너무 많은 경우 사용자 정의 양식에 새 사용자 정의 필드를 추가하고 통화로 형식을 지정하는 것이 좋습니다.
