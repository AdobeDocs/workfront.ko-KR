---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 개인 교정 기본값 구성
description: 사용자가 만든 증명에 적용되는 개인 증명 기본 설정을 정의할 수 있습니다. 이러한 기본값은 Workfront에서 첫 번째 증명을 생성하거나 새 증명 버전을 업로드할 때마다 적용됩니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 개인 교정 기본값 구성

사용자가 만든 증명에 적용되는 개인 증명 기본 설정을 정의할 수 있습니다. 이러한 기본값은 Workfront에서 첫 번째 증명을 생성하거나 새 증명 버전을 업로드할 때마다 적용됩니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: 선택 또는 더 높음</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 개인 교정 기본값 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **교정**.

1. 오른쪽 상단 모서리에서 아바타를 클릭하고 을(를) 선택합니다 **개인 설정**.
1. 을(를) 선택합니다 **교정 기본값** 탭한 다음, 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>기본 전자 메일 알림 설정</strong> </td> 
     </tr> 
     <tr> 
      <td>기본 이메일 경고</td> 
      <td>사용자가 이메일 업데이트를 받는 빈도를 선택합니다. 모든 활동, 내 댓글에 대한 회신, 결정, 최종 결정, 시간별 요약, 일별 요약 또는 사용 안 함을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td>새 게스트 검토자에 대한 기본 전자 메일 경고</td> 
      <td>게스트 검토자가 이메일 업데이트를 받는 빈도를 선택합니다. 옵션은 기본 이메일 경고의 옵션과 동일합니다.</td> 
     </tr> 
     <tr> 
      <td>새로운 증명 알림</td> 
      <td>증명에 추가될 때 알림을 수신하도록 선택합니다.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>메시지 설정</strong> </td> 
     </tr> 
     <tr> 
      <td>증명 제목 템플릿</td> 
      <td>증명을 공유할 때 이메일의 제목에 사용자가 볼 내용을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td>증명 메시지 템플릿</td> 
      <td>증명을 공유할 때 전자 메일 본문에 사용자가 볼 내용을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>기본 증명 설정</strong> </td> 
     </tr> 
     <tr> 
      <td>모든 결정을 내릴 때 증명 잠금</td> 
      <td>모든 결정을 수행한 후 추가 변경 시 증명을 자동으로 잠그도록 선택합니다.</td> 
     </tr> 
     <tr> 
      <td>하나의 결정만 필요</td> 
      <td>한 가지 증명만 요구할 것을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td>로그인 필요</td> 
      <td> <p>Workfront 증명 로그인 자격 증명이 있는 사용자만 증명을 사용할 수 있도록 선택합니다.</p> <p>참고: Workfront 증명 자격 증명은 회사 사용자가 SSO를 하지 않는 한 Workfront 자격 증명과 다를 수 있습니다. 회사 사용자가 SSO하는 경우에만 이 기능을 사용하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td>구독이 활성화됨</td> 
      <td>조직 외부의 검토자가 공개 URL 또는 포함 코드를 통해 증명에 등록할 수 있도록 허용합니다. 이 옵션을 선택하면 가입자가 이메일의 링크를 클릭하여 증표에 액세스할 수도 있습니다. 외부 검토자가 전자 메일 내의 링크를 클릭하여 증표에 액세스하도록 하려면 이 옵션을 선택합니다. 이 옵션은 공개 공유 옵션을 선택하고 이 사용자가 만든 모든 증명에 적용되는 경우 기본적으로 활성화됩니다. </td> 
     </tr> 
     <tr> 
      <td>새 게스트 검토자에 대한 기본 역할</td> 
      <td>게스트 검토자에 대한 기본 증명 역할을 선택합니다. 옵션은 기본 증명 역할의 옵션과 동일합니다.</td> 
     </tr> 
     <tr> 
      <td>원본 파일의 다운로드 차단</td> 
      <td>사용자가 원본 파일을 다운로드하지 못하도록 선택합니다. </td> 
     </tr> 
     <tr> 
      <td>기본 증명 역할</td> 
      <td>기본 증명 역할을 선택합니다. </td> 
     </tr> 
     <tr> 
      <td>내 기본 마크업 색상</td> 
      <td>기본 마크업 색상을 선택합니다. </td> 
     </tr> 
    </tbody> 
   </table>
