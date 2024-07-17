---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 이메일 알림에 회신
description: 프로젝트, 작업, 문제 및 기타 오브젝트에 대한 댓글에서 생성된 Workfront 이메일 알림에 응답하여 Adobe Workfront 애플리케이션에서 작성한 원래 댓글에 답글을 추가할 수 있습니다.
author: Nolan and Alina
feature: Get Started with Workfront
exl-id: fea88410-8f37-49d0-9f5d-9fbac4ab5de6
source-git-commit: 886b5d9084cb1bfb63157152f05fa20128d34903
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# 이메일 알림에 회신

<!-- Audited: April 2024-->

이메일 알림 구성 방식에 따라 액세스 권한이 있는 특정 오브젝트가 업데이트될 때 이메일 알림을 받을 수 있습니다.

다음과 같은 방법으로 이메일 알림에서 업데이트에 회신할 수 있습니다.

* 이메일 내의 댓글 버튼을 사용하여 Workfront으로 다시 이동하고 업데이트 영역에서 업데이트에 회신할 수 있습니다.
* 받은 이메일에 답장을 보냅니다. 답글 이메일이 원래 의견에 대한 Workfront 답글로 추가됩니다.

<!--
>[!NOTE]
>
>Replying to updates by email is not available for environments on Cluster 6.
-->

다음 오브젝트에 대한 댓글로 생성된 Workfront 이메일에 응답할 수 있습니다.

* 프로젝트
* 작업
* 문제
* 문서
* 템플릿 및 템플릿 작업
* Portfolio
* 프로그램
* 반복
* 타임시트

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>새로운 기능: 문제 및 문서에 대한 기여자 이상, 기타 모든 오브젝트에 대한 라이트 이상</p>
   <p>현재: 문제 및 문서에 대해 요청 이상, 다른 모든 객체에 대해 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>답글을 게시하려는 오브젝트에 대한 보기 이상의 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>답글을 게시하려는 오브젝트에 대한 이상의 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 이메일 알림에서 업데이트에 회신

이메일 알림을 받으면 이메일 알림에서 연결된 Workfront 개체를 빠르게 열고 회신을 통신 스레드에 바로 추가할 수 있습니다.

1. Workfront의 업데이트로 생성된 이메일 알림을 엽니다.

   ![email.png](assets/email-350x202.png)
1. 전자 메일 알림에서 **댓글**&#x200B;을 클릭합니다.

   개체에 대한 세부 정보 페이지가 Workfront에서 열립니다.

1. 회신을 추가할 업데이트로 이동합니다.

   대화에 적극적으로 참여하는 사용자를 보는 것 외에도 해당 업데이트 스레드의 맨 위에서 각 회신에서 누가 태그 지정되었는지 확인할 수 있습니다. 이러한 사용자는 오브젝트에 가입된 사용자와 함께 오브젝트에 대한 업데이트나 회신이 있을 때마다 알림을 받습니다. 더 많은 사용자를 태그 지정하려면 [업데이트에 다른 사용자 태그 지정](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.

1. **회신,**&#x200B;을 클릭하고 회신을 입력한 다음 **회신**&#x200B;을 클릭합니다.

   답글이 댓글 달기 스레드에 새 댓글로 추가됩니다.

## 이메일 알림에 회신하여 오브젝트에 업데이트 추가

Workfront 이메일 알림을 받으면 Workfront에 로그인하지 않고도 통신 스레드에 업데이트를 빠르게 추가할 수 있습니다.

>[!IMPORTANT]
>
>* 이메일 알림에 회신하려면 먼저 업데이트를 트리거한 오브젝트를 볼 권한이 있어야 합니다.
>
>* 제출 오류를 방지하려면 Outlook 사용자는 회신을 입력하기 전에 기존 이메일 콘텐츠를 삭제해야 합니다.

Workfront 이메일에 업데이트를 추가하려면 다음 작업을 수행하십시오.

1. 이메일 애플리케이션에서 응답하려는 Workfront 이메일을 연 다음 원본 이메일에서 회신 이메일 창을 엽니다.

   >[!NOTE]
   >
   >    다른 사람이 전달한 이메일 알림에 답장을 보낼 수 없습니다.


1. 이메일 회신에 업데이트를 입력합니다.

   첨부 파일이 허용되지 않으며 이메일의 업데이트에 적용된 서식 있는 텍스트 서식이 업데이트 탭에서 볼 때 업데이트에 표시되지 않습니다.
1. **보내기**&#x200B;를 클릭합니다.

   업데이트가 개체의 통신 스레드에 대한 응답으로 추가됩니다.
