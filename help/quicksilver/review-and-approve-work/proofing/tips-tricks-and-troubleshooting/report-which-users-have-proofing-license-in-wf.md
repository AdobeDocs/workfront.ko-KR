---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Adobe Workfront에서 증명 라이선스가 있는 사용자 나열
description: 다음 방법 중 하나로 현재 Adobe Workfront에서 "사용자가 증명을 생성할 수 있음" 옵션이 활성화된 사용자를 확인할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Adobe Workfront에서 증명 라이선스가 있는 사용자 나열

다음 방법 중 하나로 현재 Adobe Workfront에서 &quot;사용자가 증명을 생성할 수 있음&quot; 옵션이 활성화된 사용자를 확인할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>기존 플랜: Select 또는 Premium</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 편집 대상:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 캘린더 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## 사용자 보고서 만들기

사용자 보고서를 만들어 증명을 생성할 수 있는 사용자를 확인할 수 있습니다.

1. **보고** 영역으로 이동합니다.
1. **새 보고서** 드롭다운 메뉴를 클릭한 다음 **사용자 보고서**&#x200B;를 클릭합니다.

1. **필터** 탭에서 **필터 규칙 추가**&#x200B;를 클릭합니다.

1. 사용 가능한 필드에서 **사용자**&#x200B;를 확장한 다음 **증명 라이선스 있음**&#x200B;을 클릭합니다.

1. **같음** > **참**&#x200B;을 선택하세요.

   ![report_proflicenses.png](assets/report-prooflicenses-350x135.png)

1. **저장+닫기**&#x200B;를 클릭합니다.

   이 보고서는 증명 라이선스가 할당된 Workfront의 모든 사용자를 표시합니다.

## 인물 보기 업데이트

사람 보기에서 새 열을 추가하여 증명을 생성할 수 있는 사용자를 볼 수 있습니다.

1. **사람** 영역으로 이동합니다.
1. **사람** 탭을 클릭합니다.
1. **보기** 드롭다운 메뉴에서 다음 중 하나를 수행합니다.

   * 기존 보기에 이 정보를 추가하려면 사용자 지정할 보기를 선택한 다음 **보기 사용자 지정**&#x200B;을 클릭합니다.
   * 새 보기에 이 정보를 추가하려면 **새 보기**&#x200B;를 클릭하세요.

1. **열 추가**&#x200B;를 클릭합니다.
1. 사용 가능한 필드에서 **사용자**&#x200B;를 확장한 다음 **증명 라이선스 있음**&#x200B;을 클릭합니다.

1. **완료**&#x200B;를 클릭한 다음 **보기 저장** 또는 **새 보기로 저장**&#x200B;을 클릭합니다.

   사용자에게 증명 라이선스가 할당되었는지 여부에 따라 보기에 **True** 또는 **False**&#x200B;이(가) 표시됩니다.
