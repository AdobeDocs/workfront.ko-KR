---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 개인 증명 기본값 구성
description: 자신이 생성한 증명에 적용되는 개인 증명 기본 설정을 정의할 수 있습니다. 이 기본값은 Workfront에서 최초 증명을 생성하거나 새 증명 버전을 업로드할 때마다 적용됩니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# 개인 증명 기본값 구성

자신이 생성한 증명에 적용되는 개인 증명 기본 설정을 정의할 수 있습니다. 이 기본값은 Workfront에서 최초 증명을 생성하거나 새 증명 버전을 업로드할 때마다 적용됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
    <p>작업 또는 계획</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 개인 증명 기본값 구성

{{step1-to-proofing}}

1. 오른쪽 상단 모서리에서 아바타를 클릭하고 **개인 설정**&#x200B;을 선택합니다.
1. **증명 기본값** 탭을 선택한 후 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>기본 전자 메일 알림 설정</strong> </td> 
     </tr> 
     <tr> 
      <td>기본 이메일 경고</td> 
      <td>사용자가 이메일 업데이트를 받는 빈도를 선택합니다. 모든 활동 선택, 내 의견에 응답, 결정, 최종 결정, 시간별 요약, 일별 요약 또는 사용 안 함.</td> 
     </tr> 
     <tr> 
      <td>새 게스트 검토자에 대한 기본 이메일 경고</td> 
      <td>게스트 검토자가 이메일 업데이트를 받는 빈도를 선택하십시오. 옵션은 기본 이메일 경고에 대한 옵션과 동일합니다.</td> 
     </tr> 
     <tr> 
      <td>새 증명 알림</td> 
      <td>증명에 추가되면 알림을 받도록 선택합니다.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>메시지 설정</strong> </td> 
     </tr> 
     <tr> 
      <td>증명 제목 템플릿</td> 
      <td>증명을 공유할 때 이메일 제목에 표시할 내용을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td>증명 메시지 템플릿</td> 
      <td>증명을 공유할 때 이메일 본문에 표시할 내용을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>기본 증명 설정</strong> </td> 
     </tr> 
     <tr> 
      <td>모든 결정이 내려지면 증명 잠금</td> 
      <td>모든 결정을 내린 후 추가 변경으로부터 증명을 자동으로 잠그도록 선택합니다.</td> 
     </tr> 
     <tr> 
      <td>하나의 결정만 필요</td> 
      <td>증명에 대해 하나의 결정만 요구하도록 선택합니다.</td> 
     </tr> 
     <tr> 
      <td>로그인 필요</td> 
      <td> <p>Workfront Proof 로그인 자격 증명을 가진 사용자만 증명을 사용할 수 있도록 선택합니다.</p> <p>참고: Workfront Proof 자격 증명은 회사 사용자가 SSO를 하지 않는 한 Workfront 자격 증명과 다를 수 있습니다. 회사에서 SSO를 사용하는 경우에만 이 기능을 사용하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td>구독 활성화됨</td> 
      <td>조직 외부의 검토자가 공개 URL 또는 포함 코드를 통해 증명에 등록할 수 있도록 허용합니다. 이 옵션을 선택한 경우 구독자가 증명에 액세스하려면 이메일의 링크를 클릭해야 합니다. 외부 검토자가 증명에 액세스하기 위해 이메일 내의 링크를 클릭하도록 하려면 이 옵션을 선택합니다. 이 옵션은 공개 공유 옵션이 선택되어 있고 이 사용자가 만든 모든 증명에 적용되는 경우 기본적으로 활성화됩니다. </td> 
     </tr> 
     <tr> 
      <td>새 게스트 검토자에 대한 기본 역할</td> 
      <td>게스트 검토자에 대한 기본 증명 역할을 선택하십시오. 옵션은 기본 증명 역할의 옵션과 동일합니다.</td> 
     </tr> 
     <tr> 
      <td>원본 파일의 다운로드 차단</td> 
      <td>사용자가 원본 파일을 다운로드하지 못하도록 차단하도록 선택합니다. </td> 
     </tr> 
     <tr> 
      <td>내 기본 증명 역할</td> 
      <td>기본 증명 역할을 선택하십시오. </td> 
     </tr> 
     <tr> 
      <td>내 기본 마크업 색상</td> 
      <td>기본 마크업 색상을 선택합니다. </td> 
     </tr> 
    </tbody> 
   </table>
