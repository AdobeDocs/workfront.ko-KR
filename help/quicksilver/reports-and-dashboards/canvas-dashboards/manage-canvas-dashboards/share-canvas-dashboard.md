---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: 캔버스 대시보드 공유
description: 다른 Adobe Workfront 사용자가 보거나 편집할 수 있도록 캔버스 대시보드를 공유할 수 있습니다.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: d76ad0d51f28191cbd04af950e10a2247414830e
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# 캔버스 대시보드 공유

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>&#x200B;>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

다른 Adobe Workfront 사용자가 보거나 편집할 수 있도록 캔버스 대시보드를 공유할 수 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td> 
   <td> 
<p>임의 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td> 
<p>현재: 플랜 </p> 
<p>새로운 기능: 표준</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td><p>보고서, 대시보드 및 캘린더에 대한 액세스 보기</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td><p>대시보드를 공유할 대시보드에 대한 권한 보기</p>
   <p>대시보드 권한을 할당하려면 대시보드에 대한 권한을 관리하십시오.</p>
  </td> 
  </tr>
</tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 대시보드 공유에 대한 고려 사항

* 대시보드는 사용자, 팀, 그룹, 작업 역할 또는 회사 리소스와 공유할 수 있습니다.

* 기본적으로 대시보드 작성자는 대시보드에 대한 관리 권한을 갖습니다.

* 시스템 관리자와 관리 권한이 있는 사용자는 대시보드에 대한 보기 또는 관리 액세스 권한을 부여할 수 있습니다.

* 대시보드에 대한 보기 권한이 있는 사용자는 대시보드에 대한 보기 액세스 권한을 부여할 수 있습니다.

* 대시보드를 공유할 때 대시보드가 공유되는 리소스는 대시보드에 표시된 보고서에 대한 권한을 상속합니다.

* 대시보드가 레이아웃 템플릿을 통해 배포되면 대시보드(및 해당 보고서)에 대한 자동 보기 권한이 레이아웃 템플릿에 할당된 모든 리소스에 부여됩니다.


## 캔버스 대시보드 공유


{{step1-to-dashboards}}

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. **캔버스 대시보드** 페이지에서 공유할 대시보드를 선택합니다.

1. 페이지의 오른쪽 상단 모서리에서 **공유** 단추를 클릭합니다. **대시보드 공유** 대화 상자가 나타납니다.

1. **액세스 권한 부여** 필드에서 캔버스 대시보드를 공유할 특정 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 선택합니다.

1. (선택 사항) 대시보드에 대한 리소스의 액세스를 편집하려면 이름 옆에 있는 **보기**&#x200B;를 클릭한 다음 나타나는 드롭다운 목록에서 **관리**&#x200B;를 선택합니다.

   >[!NOTE]
   >
   > 사용자에게 액세스 수준을 통해 할당된 대시보드에 대한 편집 권한이 없는 경우 대시보드에 대한 관리 권한을 할당할 수 없습니다.

1. 대시보드를 공유할 각 리소스에 대해 5-6단계를 반복합니다.

1. **공유** 단추를 클릭합니다. 받는 사람은 대시보드가 사용자와 공유되었음을 알리는 전자 메일 알림을 받으며, 이제 **대시보드** > **캔버스 대시보드** > **공유 대시보드**&#x200B;에서 액세스할 수 있습니다.

   >[!NOTE]
   >
   > 이메일 알림에 대한 개별 사용자 환경 설정 및 시스템 제외가 적용될 수 있습니다. <br>
   > 알림은 사용자와 직접 공유할 때만 전송됩니다. 그룹, 역할, 회사 및 팀에 공유해도 전자 메일 알림이 생성되지 않습니다.<br>
   > 레이아웃 템플릿에서 상속된 권한은 대시보드 액세스에 대한 이메일 알림을 생성하지 않습니다.
