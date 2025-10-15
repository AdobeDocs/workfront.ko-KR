---
title: 클래식 레이아웃 템플릿 삭제
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 'Classic Workfront 경험의 레이아웃 템플릿은 더 이상 Workfront 인터페이스에서 사용할 수 없지만 여전히 Workfront 데이터에 영향을 줄 수 있습니다. 이로 인해 보고서 또는 대시보드의 레이아웃 템플릿(예: 다음 사용자와 공유)의 영향을 받는 필드에 불일치가 발생할 수 있습니다.'
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 55%

---

# 클래식 레이아웃 템플릿 삭제

Classic Workfront 경험의 레이아웃 템플릿은 더 이상 Workfront 인터페이스에서 사용할 수 없지만 여전히 Workfront 데이터에 영향을 줄 수 있습니다. 이로 인해 보고서 또는 대시보드의 레이아웃 템플릿(예: 다음 사용자와 공유)의 영향을 받는 필드에 불일치가 발생할 수 있습니다.

클래식 레이아웃 템플릿을 삭제하면 이러한 불일치를 해결할 수 있습니다. Workfront 인터페이스에서는 사용할 수 없으므로 은 Workfront API를 사용하여 삭제해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p>
        <p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## API 호출을 사용하여 클래식 레이아웃 템플릿 삭제

브라우저의 URL 표시줄에 API 호출을 입력하고 Enter 키를 누를 수 있습니다. 브라우저에 API 응답이 표시됩니다.

>[!NOTE]
>
>전역 및 시스템 레이아웃 템플릿은 삭제할 수 없습니다.

1. Workfront에 로그인.
1. 다음 API 호출을 사용하여 삭제하려는 레이아웃 템플릿을 찾습니다.
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 삭제하려는 레이아웃 템플릿의 ID를 기록해 두십시오.
1. 다음 API 호출을 사용하여 세션 ID를 찾습니다.
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >세션 ID를 누구와도 공유하지 마십시오.

1. 다음 API 호출에 레이아웃 템플릿 ID 및 세션 ID를 삽입합니다.
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 4단계의 API 호출을 브라우저의 URL 표시줄에 붙여넣고 Enter 키를 누릅니다.

   이렇게 되면 레이아웃 템플릿이 삭제됩니다.
