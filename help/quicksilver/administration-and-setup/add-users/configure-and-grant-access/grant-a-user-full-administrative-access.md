---
title: 사용자에게 전체 관리자 액세스 권한 부여
description: 사용자에게 Workfront에 대한 전체 관리자 액세스 권한을 부여할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# 사용자에게 전체 관리자 액세스 권한 부여

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>Adobe Admin Console에서 전체 관리자 액세스 권한을 부여하는 방법에 대한 지침은
>
>* 자세한 내용은 [Adobe Admin Console을 사용하여 Workfront에서 시스템 관리자 만들기](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* 문서에서 &quot;사용자 세부 사항 편집&quot; 섹션을 참조하십시오 [개별 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ( Adobe Admin Console 설명서)를 참조하십시오.
>* Adobe Admin Console 관리자에게 문의하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 관리자는 시스템 관리자 액세스 수준을 할당하여 다른 Workfront 관리자를 만들 수 있습니다. 이 액세스 수준을 가진 사용자는 스스로 만들지 않은 항목을 비롯하여 Workfront의 모든 항목에 대한 전체 관리 액세스 권한을 갖습니다.

>[!NOTE]
>
>이는 액세스 수준을 사용하여 사용자에게 시스템의 특정 영역에 대한 관리자 액세스 권한을 부여하는 것과 다릅니다. 자세한 내용은 다음을 참조하십시오.
>
>* [특정 영역에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Workfront 관리자 액세스와 관리 권한이 있는 계획 사용자 액세스 비교](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) 이 문서
>


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다. 자세한 내용은 <a href="#" class="MCXref xref selected">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 단일 사용자에게 전체 시스템 관리자 액세스 권한 부여

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 관리자 권한을 부여할 사용자의 이름을 클릭합니다.
1. 자세히 메뉴를 클릭합니다 ![](assets/more-icon.png)를 클릭한 다음 **편집**.

1. 설정 **개인 편집** 표시되는 상자를 클릭합니다. **액세스**.

1. 에서 **액세스 수준** 드롭다운 목록에서 **시스템 관리자** 액세스 수준.

   시스템에서 수행한 변경 사항에 따라 이 액세스 수준의 이름이 변경되었을 수 있습니다.

1. 클릭 **변경 사항을 저장합니다.**

   이제 사용자는 시스템에 전체 시스템 관리자 권한이 있습니다.

## Workfront 관리자 액세스와 관리 권한이 있는 계획 사용자 액세스 비교  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

아래 두 표는 Workfront 관리자 액세스 수준을 가진 사용자의 액세스 권한과 일부 관리 권한이 있는 계획 라이센스를 가진 사용자의 액세스 권한 간의 차이를 보여줍니다.

Workfront 관리자는 시스템의 모든 개체를 보고(개체를 만든 사람에 관계없이) 새 개체를 만들고, 기존 개체를 수정하거나 삭제할 수 있습니다. 시스템의 모든 객체에 대한 전체 액세스 권한이 있습니다.

한 영역에서 기능을 편집할 수 있는 계획 라이센스가 있는 사용자는 해당 영역의 기능에 대한 전체 액세스 권한을 갖습니다.

>[!NOTE]
>
>그룹 관리자로 지정된 계획 라이센스가 있는 사용자는 Workfront 관리자에 대해 허용되는 작업 중 일부를 수행할 수 있습니다. 이 사용자는 관리하는 그룹, 해당 하위 그룹, 이러한 그룹 및 하위 그룹의 사용자에 대해서만 이러한 작업을 수행할 수 있습니다. 자세한 내용은 [그룹 관리자](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [설정 영역에 대한 액세스](#access-to-the-setup-area)
* [객체에 대한 액세스](#access-to-objects)

### 설정 영역에 대한 액세스 {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>영역/개체</th> 
   <th>Workfront 관리자 </th> 
   <th>계획 라이선스 및 일부 관리 권한이 있는 사용자</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>프로젝트 환경 설정: 프로젝트</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>프로젝트 환경 설정: 작업 및 문제</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>프로젝트 환경 설정: 상태</td> 
   <td>전체 액세스</td> 
   <td> <p>액세스 권한 없음</p> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 환경 설정: 우선순위</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>프로젝트 환경 설정: 세속</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>프로젝트 환경 설정: 환율</td> 
   <td>전체 액세스</td> 
   <td>전체 액세스</td> 
  </tr> 
  <tr> 
   <td>프로세스: 승인</td> 
   <td> <p>전체 액세스</p> </td> 
   <td>전체 액세스</td> 
  </tr> 
  <tr> 
   <td>프로세스: 이정표 경로</td> 
   <td>전체 액세스</td> 
   <td>전체 액세스</td> 
  </tr> 
  <tr> 
   <td>사용자 정의 양식</td> 
   <td>전체 액세스</td> 
   <td> <p>사용자가 만든 사용자 지정 양식 또는 이러한 양식과 공유된 사용자 지정 양식을 관리합니다.</p> <p>사용자가 만든 사용자 지정 양식 또는 공유한 사용자 지정 양식을 관리하거나 기여 권한이 있는 개체에 첨부합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>휴지통: 최근에 삭제됨</td> 
   <td>전체 액세스</td> 
   <td> <p>그룹 관리자인 사용자는 자신이 관리하는 그룹에 할당된 프로젝트 및 해당 프로젝트와 관련된 작업, 문제 또는 문서를 복원할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>휴지통: 최근에 복원됨</td> 
   <td>전체 액세스</td> 
   <td>그룹 관리자라면 최근에 복원한 항목을 볼 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>작업 역할</td> 
   <td>전체 액세스</td> 
   <td> <p>기존 작업 역할을 수정하되 삭제하지 마십시오.</p> <p>새 작업 역할을 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>팀</td> 
   <td>전체 액세스</td> 
   <td> <p>팀을 만들 수 있는 액세스 권한이 없습니다.</p> <p>사용자를 만들거나 편집할 때 사용자에게 기존 팀을 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>그룹</td> 
   <td>전체 액세스</td> 
   <td> <p>그룹을 만들 수 있는 액세스 권한이 없습니다.</p> <p>그룹 관리자만 그룹 구성원, 하위 그룹 및 그룹 수준 상태가 관리하는 그룹의 상태를 관리할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>회사</td> 
   <td>전체 액세스</td> 
   <td>전체 액세스</td> 
  </tr> 
  <tr> 
   <td>다른 이름으로 로그인</td> 
   <td>전체 액세스 </td> 
   <td> <p>그룹 관리자 액세스 권한이 액세스 수준에서 활성화되고 그룹 관리자로 지정된 경우 해당 사용자는 자신이 관리하는 그룹의 사용자와 하위 그룹의 사용자로 로그인할 수 있습니다. 시스템 관리자로 로그인할 수 없습니다.<br>사용자를 위한 그룹 관리 액세스 활성화에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>일정</td> 
   <td>전체 액세스</td> 
   <td> <p>일정을 편집할 수 있는 액세스 권한이 없습니다.</p> <p>사용자 수준에서 기존 일정을 다른 사용자에게 추가하는 액세스 권한. </p> </td> 
  </tr> 
  <tr> 
   <td>작업표 및 시간: 작업표 프로필</td> 
   <td>전체 액세스</td> 
   <td> <p>사용자 수준에서 기존 작업표 프로필을 사용자에게 할당하기 위한 액세스 권한입니다.</p> <p>그룹 관리자인 사용자는 자신이 관리하는 그룹과 하위 그룹에 대한 작업표 프로필을 만들 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>작업표 및 시간: 시간 유형</td> 
   <td>전체 액세스</td> 
   <td> <p>사용자 수준에서 사용자에게 시간 유형을 할당할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>작업표 및 시간: 기본 설정</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>이메일: 알림: 이벤트 알림</td> 
   <td>모두 활성화/비활성화</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>이메일: 알림: 미리 알림 알림</td> 
   <td>전체 액세스</td> 
   <td>전체 액세스</td> 
  </tr> 
  <tr> 
   <td>이메일: 알림: 이메일 템플릿</td> 
   <td>전체 액세스</td> 
   <td> <p>전자 메일 템플릿을 편집할 수 있는 액세스 권한이 없습니다.</p> <p>미리 알림 알림에 기존 전자 메일 템플릿을 추가하는 액세스 권한.</p> </td> 
  </tr> 
  <tr> 
   <td>이메일: 자동 미리 알림</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>이메일: 초대</td> 
   <td>전체 액세스</td> 
   <td> <p>전자 메일 초대를 편집할 수 없습니다.</p> <p>[사람] 탭에서만 등록되지 않은 사용자에게 이메일 초대장을 다시 보낼 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>이메일: 설정</td> 
   <td>전체 액세스</td> 
   <td> <p>액세스 권한 없음</p> </td> 
  </tr> 
  <tr> 
   <td>스코어카드</td> 
   <td>전체 액세스</td> 
   <td> <p>전체 액세스</p> </td> 
  </tr> 
  <tr> 
   <td>경비 유형</td> 
   <td>전체 액세스</td> 
   <td> <p>액세스 권한 없음</p> </td> 
  </tr> 
  <tr> 
   <td>위험 유형</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>액세스 수준</td> 
   <td> <p>모든 액세스 수준을 수정할 수 있는 전체 액세스 권한</p> <p>시스템 관리자 및 외부 사용자 액세스 수준은 기본적으로 수정할 수 없습니다.</p> </td> 
   <td> <p>액세스 수준을 편집할 수 없습니다.</p> <p>사용자 수준에서 다른 사용자와 같거나 낮거나 같은 사용자에게 액세스 수준을 할당합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>인터페이스: 레이아웃 템플릿</td> 
   <td>전체 액세스</td> 
   <td> <p>사용자 수준에서 기존 레이아웃 템플릿을 다른 사용자에게 할당할 수 있는 액세스 권한. </p> <p>그룹 관리자로 지정된 사용자는 자신이 관리하는 그룹 및 하위 그룹에 대한 레이아웃 템플릿을 만들 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>인터페이스: 피드 업데이트</td> 
   <td>전체 액세스</td> 
   <td> <p>피드 업데이트를 수정할 수 있는 액세스 권한이 없습니다.</p> <p>사용자 지정 Forms을 편집할 때 피드 업데이트에서 추적할 필드를 추가할 수 있는 액세스 권한.</p> </td> 
  </tr> 
  <tr> 
   <td>인터페이스: 필터</td> 
   <td>전체 액세스</td> 
   <td> <p>설정 영역에서 필터를 만들 수 있는 액세스 권한이 없습니다.</p> <p>개체 목록에서 새 필터를 만들 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>인터페이스: 보기 횟수</td> 
   <td>전체 액세스</td> 
   <td> <p>설정 영역에서 뷰를 생성할 수 없습니다.</p> <p>객체 목록에서 새 뷰를 생성할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>인터페이스: 그룹화</td> 
   <td>전체 액세스</td> 
   <td> <p>설정 영역에서 그룹을 만들 수 없습니다.</p> <p>개체 목록에 새 그룹화를 만들려면 액세스 권한이 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>인터페이스: 목록 컨트롤</td> 
   <td>전체 액세스</td> 
   <td> <p>액세스 권한 없음</p> </td> 
  </tr> 
  <tr> 
   <td>문서: 클라우드 공급자</td> 
   <td>전체 액세스</td> 
   <td> <p>클라우드 공급자를 구성할 수 없습니다.</p> <p>클라우드 제공업체를 Workfront과 통합한 후 문서 탭에서 클라우드 제공업체와의 링크 문서에 액세스하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>문서: 메타데이터 매핑</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>문서: SharePoint 통합</td> 
   <td>전체 액세스</td> 
   <td> <p>SharePoint 통합을 구성할 수 있는 액세스 권한이 없습니다.</p> <p>Workfront와의 SharePoint 통합이 구성된 후 문서 탭에서 SharePoint으로 문서를 연결 및 연결할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>문서: 사용자 지정 통합</td> 
   <td>전체 액세스</td> 
   <td> <p>사용자 지정 통합을 구성할 수 있는 액세스 권한이 없습니다.</p> <p>타사 공급자가 Workfront과 통합되면 문서 탭에서 타사 공급자와 문서를 연결하는 데 액세스할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>시스템: 브랜딩</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>시스템: 고객 정보</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>시스템: 단일 사인온(SSO)</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>시스템: SSO용 사용자 업데이트</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>시스템: 킥스타트</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>시스템: 진단</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
  <tr> 
   <td>시스템: 기본 설정</td> 
   <td>전체 액세스</td> 
   <td>액세스 권한 없음</td> 
  </tr> 
 </tbody> 
</table>

### 객체에 대한 액세스 {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>영역/개체</th> 
   <th>Workfront 관리자 </th> 
   <th>계획 라이선스 및 일부 관리 권한이 있는 사용자</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>캘린더</td> 
   <td>전체 액세스</td> 
   <td>캘린더가 만들고 캘린더와 공유하는 달력을 관리합니다.</td> 
  </tr> 
  <tr> 
   <td>대시보드</td> 
   <td>전체 액세스</td> 
   <td>대시보드 가 만들고 대시보드 및 이들과 공유되는 대시보드를 관리합니다.</td> 
  </tr> 
  <tr> 
   <td>문서</td> 
   <td>전체 액세스</td> 
   <td>업로드하는 문서 또는 공유된 문서를 관리합니다.</td> 
  </tr> 
  <tr> 
   <td>문제</td> 
   <td>전체 액세스</td> 
   <td>만든 문제 또는 이들과 공유된 문제를 관리합니다.</td> 
  </tr> 
  <tr> 
   <td>포트폴리오</td> 
   <td>전체 액세스</td> 
   <td>포트폴리오 제작 또는 공유되는 포트폴리오 관리 </td> 
  </tr> 
  <tr> 
   <td>프로그램</td> 
   <td>전체 액세스</td> 
   <td>사용자가 만드는 프로그램 또는 이와 공유되는 프로그램을 관리합니다.</td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>전체 액세스</td> 
   <td>프로젝트가 만들거나 공유된 프로젝트를 관리합니다.</td> 
  </tr> 
  <tr> 
   <td>보고서</td> 
   <td>전체 액세스</td> 
   <td>보고서 또는 보고서 세트를 만들고 공유하여 관리합니다. 시스템 보고서를 보고, 복사하고, 편집합니다.</td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td>전체 액세스</td> 
   <td>사용자가 만드는 작업 또는</td> 
  </tr> 
  <tr> 
   <td>템플릿</td> 
   <td>전체 액세스</td> 
   <td>템플릿 생성 또는 템플릿과 공유되는 템플릿 관리</td> 
  </tr> 
  <tr> 
   <td>타임시트</td> 
   <td>전체 액세스</td> 
   <td>전체 액세스</td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td>전체 액세스</td> 
   <td> <p>제한된 액세스</p> <p>그룹 관리자가 아닌 사용자 또는 공개가 아닌 그룹에 그룹을 할당할 수 없습니다.</p> <p>액세스 수준을 사용자가 자신의 액세스 수준보다 높은 사용자에게 할당할 수 없습니다.</p> <p>그룹 관리자 액세스 권한이 액세스 수준에서 활성화되고 그룹의 그룹 관리자로 지정된 경우 그룹 관리자는 의 암호를 재설정하고 자신이 관리하는 그룹 및 해당 하위 그룹의 사용자로 로그인할 수 있습니다. 암호를 재설정하거나 시스템 관리자로 로그인할 수 없습니다.<br>사용자를 위한 그룹 관리 액세스 활성화에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
