---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Adobe Workfront에서 언어 교정 라이센스가 있는 사용자 나열
description: 아래 방법 중 하나로 현재 Adobe Workfront에서 "사용자가 증명을 생성할 수 있습니다" 선택 사항이 활성화된 사용자를 볼 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Adobe Workfront에서 언어 교정 라이센스가 있는 사용자 나열

아래 방법 중 하나로 현재 Adobe Workfront에서 &quot;사용자가 증명을 생성할 수 있습니다&quot; 선택 사항이 활성화된 사용자를 볼 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>기존 계획: Select 또는 Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 편집:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 달력 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 사용자 보고서 만들기

사용자 보고서를 만들어 증명을 생성할 수 있는 사용자를 볼 수 있습니다.

1. 다음으로 이동 **보고** 영역.
1. 을(를) 클릭합니다. **새 보고서** 드롭다운 메뉴를 클릭한 다음 **사용자 보고서**.

1. 설정 **필터** 탭, **필터 규칙 추가**.

1. 사용 가능한 필드에서 를 확장합니다. **사용자**&#x200B;를 클릭한 다음 **증명 라이센스 있음**.

1. 선택 **Equal** > **True**.

   ![report_propoflicenses.png](assets/report-prooflicenses-350x135.png)

1. 클릭 **저장+닫기**.

   이 보고서에는 Workfront에 언어 교정 라이센스가 할당된 모든 사용자가 표시됩니다.

## 사람 보기 업데이트

사람 보기에서 새 열을 추가하여 증명을 생성할 수 있는 사용자를 볼 수 있습니다.

1. 로 이동합니다. **사람** 영역.
1. 을(를) 클릭합니다. **사람** 탭.
1. 에서 **보기** 드롭다운 메뉴에서 다음 중 하나를 수행합니다.

   * 기존 보기에 이 정보를 추가하려면 사용자 지정할 보기를 선택한 다음 **보기 사용자 지정**.
   * 이 정보를 새 보기에 추가하려면 **새 보기**.

1. 클릭 **열 추가**.
1. 사용 가능한 필드에서 를 확장합니다. **사용자**&#x200B;를 클릭한 다음 **증명 라이센스 있음**.

1. 클릭 **완료**&#x200B;를 클릭한 다음 **보기 저장** 또는 **새 보기로 저장**.

   보기가 표시됩니다 **True** 또는 **False** 사용자에게 언어 교정 라이센스가 할당되었는지 여부에 따라 다릅니다.
