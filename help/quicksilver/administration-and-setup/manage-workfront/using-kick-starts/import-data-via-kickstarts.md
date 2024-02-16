---
user-type: administrator
product-area: system-administration
keywords: 킥스타트, 킥스타트, 킥스타트, 킥스타트
navigation-topic: use-kick-starts
title: 킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기
description: 킥스타트는 특별히 형식이 지정된 Excel 통합 문서로, Workfront으로 가져올 데이터로 채울 수 있습니다. Adobe Workfront은 킥스타트 데이터 가져오기에 설명된 대로 이 작업을 수행하는 데 사용할 수 있는 킥스타트 템플릿을 제공합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 22c8f41f725784e348c44b209b9bc1537b26c952
workflow-type: tm+mt
source-wordcount: '2725'
ht-degree: 6%

---

# 킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기

<!--Audited: 12/2023-->

킥스타트는 특별히 형식이 지정된 Excel 통합 문서로, Workfront으로 가져올 데이터로 채울 수 있습니다. Adobe Workfront은에 설명된 대로 이 작업을 수행하는 데 사용할 수 있는 킥스타트 템플릿을 제공합니다 [킥스타트 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

이 프로세스는 다음 3가지 주요 작업으로 나뉩니다.

* 먼저 킥스타트 템플릿을 스프레드시트 파일로 내보냅니다
* 둘째, 스프레드시트를 데이터로 채웁니다
* 마지막으로, 채워진 스프레드시트를 Workfront으로 가져옵니다

이러한 각 절차는 이 문서에서 적절한 순서로 요약되어 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p> 새로운 기능: 표준</p>
   또는
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>Workfront 관리자여야 합니다. </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 제한 사항

킥스타트 템플릿을 사용하여 많은 개체를 Workfront으로 가져올 수 있습니다. 그러나 다음 제한 사항을 고려하십시오.

* 이러한 방식으로 데이터를 가져오면 Workfront에 이미 존재하는 레코드에 대한 정보가 업데이트되지 않습니다.
* 새 레코드와 해당 정보만 가져올 수 있습니다.
* 가져오기가 시간 초과되지 않도록 한 번에 2,000개 이하의 레코드를 가져옵니다.

## 킥스타트 템플릿을 스프레드시트 파일로 내보내기

킥스타트 템플릿을 내보내면 빈 Excel 스프레드시트 통합 문서가 표시됩니다. 스프레드시트가 컴퓨터에 다운로드되면 스프레드시트를 사용하여 사용자 정보로 채운 다음 다시 Workfront으로 가져올 수 있습니다.

킥스타트 템플릿을 내보내려면 다음을 수행하십시오.

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  -->

1. 클릭 **시스템** > **데이터 가져오기(킥스타트)**.

1. 포함할 정보 유형을 선택합니다.

   선택하는 각 옵션은 내보낸 스프레드시트에 있는 여러 탭의 컬렉션을 나타냅니다. 예를 들어 **보고서** 옵션을 선택하면 보고서를 만드는 데 필요한 모든 개체가 스프레드시트에 포함됩니다(보기, 필터, 그룹화, 보고서).

   아래 나열된 모든 개체 유형을 사용하여 데이터를 Workfront으로 가져올 수 있습니다. 유일한 예외는 액세스 수준 옵션입니다. 내보내기의 액세스 수준 데이터 시트는 참조용으로 제공됩니다. 이 시트를 사용하면 ID별로 새 사용자 계정에 액세스 수준을 할당할 수 있습니다.)

   각 객체 유형에 대한 템플릿은 다음 파일 형식으로 내보낼 수 있으며, 다음과 같은 시트가 포함되어 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>오브젝트</strong> </p> </th> 
      <th> <p><strong>다음으로 내보내기</strong> </p> </th> 
      <th> <p><strong>내보낸 스프레드시트의 시트</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>대시보드</p> <p>시스템의 모든 대시보드를 내보낼 수 있습니다. 단일 내보내기에서 최대 100개의 특정 대시보드를 선택할 수 있습니다.</p> </td> 
      <td scope="col">ZIP 파일로 내보내기</td> 
      <td scope="col"> <p>매개변수</p> <p>설명 텍스트</p><p>매개변수 옵션</p> <p>매개변수 그룹</p> <p>범주 매개변수</p> <p>범주</p> <p>보고서</p> <p>포털 탭 섹션</p> <p>대시보드</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>보고서</p> <p>시스템의 모든 보고서를 내보낼 수 있습니다. 단일 내보내기에서 최대 100개의 특정 보고서를 선택할 수 있습니다.</p> </td> 
      <td scope="col">ZIP 파일로 내보내기 </td> 
      <td scope="col"> <p scope="col">매개변수</p> <p scope="col">설명 텍스트</p> <p scope="col">매개변수 옵션</p> <p scope="col">매개변수 그룹</p> <p scope="col">범주 매개변수</p> <p scope="col">범주</p> <p scope="col">보고서</p> <p scope="col">환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>승인</p> </td> 
      <td scope="col"> <p>Excel 파일로 내보내기</p> </td> 
      <td scope="col"> <p>단계 승인자</p> <p>승인 단계</p> <p>승인</p> <p>승인 진행</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>사용자 정의 데이터</p> </td> 
      <td scope="col"> <p>Excel 파일로 내보내기</p> </td> 
      <td scope="col"> <p>매개변수</p> <p>설명 텍스트</p>  <p>매개변수 옵션</p> <p>매개변수 그룹</p> <p>범주 매개변수</p> <p>범주</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>경비 유형</p> </td> 
      <td scope="col"> <p>Excel 파일로 내보내기</p> </td> 
      <td> <p>경비 유형</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td> <p>시간 유형</p> </td> 
      <td scope="col"> <p>Excel 파일로 내보내기</p> </td> 
      <td> <p>시간 유형</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td> <p>팀</p> </td> 
      <td scope="col"> <p>Excel 파일로 내보내기</p> </td> 
      <td> <p> 팀원</p> <p>팀</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>사용자</p> </td> 
      <td> <p>Excel 파일로 내보냅니다. 옵션의 전체 목록을 보려면 <strong>추가 옵션</strong>.</p> </td> 
      <td> <p>사용자</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td>액세스 수준</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p>액세스 수준</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td>할당</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p>할당</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td>회사</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 회사</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>이메일 템플릿</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p>이메일 템플릿</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>경비</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 경비'</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>외부 페이지</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 외부 페이지</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>필터</td> 
      <td>ZIP 파일로 내보내기</td> 
      <td> <p> 필터</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>그룹</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 그룹</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>그룹화</td> 
      <td>ZIP 파일로 내보내기</td> 
      <td> <p> 그룹화</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>시간</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 시간</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>문제</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 문제</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>작업 역할</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 작업 역할</p> <p>환경 설정 </p> </td> 
     </tr>

   <tr> 
      <td>마일스톤 경로</td> 
      <td> Excel 파일로 내보내기</td> 
      <td> <p> 마일스톤</p> <p>마일스톤 경로</p> <p>환경 설정 </p> </td> 
     </tr>

   <tr> 
      <td>참고</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 참고</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>Portfolio</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> Portfolio</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>프로젝트</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 대기열</p> <p>프로젝트</p> <p>라우팅 규칙</p> <p>대기열 주제</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>리소스 견적</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 리소스 견적</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>위험</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 위험</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>위험 유형</td> 
      <td> Excel 파일로 내보내기</td> 
      <td> <p> 위험 유형</p> <p>환경 설정</p> </td> 
     </tr> 
     <tr> 
      <td>스코어카드</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p>스코어카드 질문</p> <p>스코어카드 옵션</p> <p>스코어카드</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>작업</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 작업</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>템플릿</td> 
      <td> Excel 파일로 내보내기</td> 
      <td> <p> 대기열</p> <p>템플릿</p> <p>라우팅 규칙</p> <p>대기열 주제</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>템플릿 할당</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 템플릿 할당</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>템플릿 작업</td> 
      <td>Excel 파일로 내보내기</td> 
      <td> <p> 템플릿 작업</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>타임시트</td> 
      <td> Excel 파일로 내보내기</td> 
      <td> <p> 타임시트 프로필</p> <p>타임시트</p> <p>환경 설정 </p> </td> 
     </tr> 
     <tr> 
      <td>보기 </td> 
      <td> <p>ZIP 파일로 내보내기</p> </td> 
      <td> <p> 보기</p> <p>환경 설정 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **다운로드**.
1. 계속 [데이터로 스프레드시트 템플릿 채우기](#populate-the-spreadsheet-template-with-your-data) 빈 템플릿 스프레드시트를 정보로 채웁니다.

## 데이터로 스프레드시트 템플릿 채우기 {#populate-the-spreadsheet-template-with-your-data}

* [스프레드시트에 포함된 탭(데이터 시트) 개요](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [레코드 가져오기](#import-a-record)
* [날짜 포함](#include-dates)
* [와일드카드 사용](#use-wildcards)
* [ID에 대한 속성 이름 대체](#attribute-name-substitution-for-ids)

### 스프레드시트에 포함된 탭(데이터 시트) 개요

>[!TIP]
>
>킥스타트 템플릿을 채울 때 각 열의 정보 형식을 지정해야 하는 방법을 더 잘 이해하려면 가져오려는 개체에서 기존 Workfront 데이터로 킥스타트를 내보내는 연습을 고려해 보십시오. 자세한 내용은 [킥스타트를 통해 Adobe Workfront에서 데이터 내보내기](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

빈 킥스타트 템플릿을 열면 다양한 탭(데이터 시트)을 사용할 수 있습니다. 다운로드하도록 선택한 객체에 따라 다릅니다. 각 객체는 프로젝트, 작업, 시간, 대시보드 및 사용자와 같은 애플리케이션의 객체를 나타냅니다.

이러한 탭 중 하나를 열면 2행에 가져오는 동안 설정할 수 있는 각 객체의 필드가 표시됩니다. 열 헤더에서 &quot;set&quot;이라는 단어 뒤에 필드의 이름이 데이터베이스에 나타나는 대로 표시됩니다. 이러한 필드는 열 헤더 역할을 합니다.

>[!IMPORTANT]
>
>오류를 방지하려면 다음 사항을 확인하십시오.
>
>* 킥스타트 스프레드시트의 빈 첫 행을 삭제하지 마십시오.
>* 이러한 필드(열 헤더)를 어떤 방식으로든 삭제, 수정 또는 재배열하지 마십시오. 예를 들어, 순서나 이름을 변경하지 마십시오.
>* 열 헤더에 굵게 표시되는 모든 필드에 값을 추가합니다. 필수 필드를 나타냅니다.
>
>     그러나 필수 필드에 시스템 기본 설정에 설정된 기본값이 포함되어 있으면 이를 채우지 않아도 됩니다.
>
>     예를 들어 **프로젝트 프로젝트** 탭, **setCondition** 및 **setConditionType** 필드는 비워 둘 수 있지만 **집합 ID** 및 **setName** 열은 사용할 수 없습니다.
>
>* 특정 필드: **setResourceRevenue** 및 **setEnteredByID**&#x200B;는 시스템에서 자동으로 생성됩니다. 스프레드시트에서 이러한 필드에 대한 데이터를 입력하면 스프레드시트를 업로드할 때 킥스타트 프로세스가 우선합니다.

### 레코드 가져오기  {#import-a-record}

시트의 각 행은 고유한 오브젝트에 해당합니다.

1. 에 정보 추가 **isNew** 열:

   * 가져오려는 개체가 새 개체인 경우 **참** 행에서 데이터를 가져옵니다. 이 값은 대/소문자를 구분하므로 항상 모두 대문자로 입력해야 합니다.
   * 개체가 이미 Workfront에 있는 경우 **FALSE** 다음에서 **isNew** 행을 무시하는 열입니다. 이 값은 대/소문자를 구분하므로 항상 모두 대문자로 입력해야 합니다.

      * Workfront에 이미 존재하는 레코드는 업데이트되지 않습니다.
      * Workfront의 데이터가 있는 템플릿을 다운로드한 경우 기존 개체가 이미 로 표시되어 있습니다. **FALSE**.
      * 빈 템플릿을 다운로드한 경우에는 기존 객체에 대해 새 행을 추가할 필요가 없습니다.

1. 에 정보 추가 **ID** 다음 방법 중 하나로 열을 만듭니다.

   * 가져오려는 개체가 새 개체인 경우(입력한 경우) **참** 다음에서 **isNew** 열)에서 ID에 대한 숫자를 입력합니다. 이 번호는 스프레드시트에서 고유해야 합니다. 예를 들어 세 개의 객체를 가져오는 경우 객체 각각에 대해 1, 2, 3의 ID를 부여할 수 있습니다.

   * 개체가 Workfront에 이미 있는 경우 (및 **FALSE** 다음에 있음 **isNew** column)을 사용하고 기존 개체에 대한 새 정보를 가져오는 경우 ID는 해당 개체의 Workfront에 있는 영숫자 GUID여야 합니다.

   >[!TIP]
   >
   > Workfront에서 개체의 고유 GUID를 확인하려면 해당 개체에 대한 보고서를 만들고 ID 열을 보고서에 추가할 수 있습니다. 해당 열의 각 개체 값은 개체의 GUID입니다.

   * Workfront에 이미 존재하는 레코드는 업데이트되지 않습니다.
   * 데이터가 있는 템플릿을 다운로드한 경우 기존 개체에는 이미 ID로 GUID가 포함되어 있습니다.
   * 를 변경하여 기존 개체를 기반으로 새 개체를 가져올 수 있습니다 **FALSE** 끝 **참** 다음에서 **isNew** 열, ID 변경 및 가져오기 전에 필요한 데이터 조정

   ![그룹에 대한 샘플 ID](assets/kick-start-group-example.png)

   * 프로젝트를 가져올 때 그룹 ID를 표시해야 합니다.

      * 그룹이 Workfront에 이미 있는 경우 고유한 ID를 **집합 ID** 프로젝트용 필드입니다.
      * 그룹이 Workfront에 없는 경우 **그룹** 시트를 가져오기 파일로 설정한 다음 **isNew** 필드 대상 **참** 그룹 시트에서 새 그룹의 숫자 ID를 **ID** 열. 다음 **집합 ID** 새 프로젝트의 필드는 숫자와 일치해야 합니다. **ID** 새 그룹용입니다.

     **예:** 프로젝트의 경우 다음에 표시되는 값 **집합 ID** 열은 다음 중 하나여야 합니다.

      * Workfront 인스턴스의 기존 그룹에 대한 GUID
      * 의 ID 열에 있는 값(숫자) **그룹** 시트(가져오는 동안 새 그룹을 만드는 경우)

1. 가져오기 중에 채울 필수 필드 및 기타 필드의 입력 값.
1. (선택 사항) 사용자 지정 데이터를 추가하려면:

   * 가져오기 프로세스에 포함할 각 사용자 정의 필드에 대해 새 열을 만듭니다.
   * 해당 사용자 정의 필드에 대해 각 새 열의 이름을 다음과 같이 지정합니다. **DE:[Workfront에 표시되는 사용자 정의 필드의 이름]**. 예를 들어 사용자 정의 필드 &quot;DE: Departments&quot;를 만들 수 있습니다.
   * 열에서 **setCategoryId**&#x200B;이 사용자 정의 필드가 있는 기존 사용자 정의 양식의 GUID를 입력합니다. 사용자 정의 데이터를 가져올 때 이 필드가 필요합니다.
   * 사용자 지정 필드(예: 라디오 단추, 확인란 또는 목록)에 여러 데이터 값을 추가해야 하는 경우 환경 설정 탭에 나열된 세로 막대 사용자 지정 데이터 구분 기호 &quot;|&quot;를 사용하여 값을 구분하십시오.

     **예:** DE:Departments 열 아래에 A|D를 입력하여 사용자 정의 양식에서 부서 A 및 부서 D를 채웁니다.

### 날짜 포함  {#include-dates}

Workfront은 대부분의 날짜 형식을 처리할 수 있습니다. 그러나 스프레드시트의 날짜 열 형식이 날짜로 지정되어 있는지 확인해야 합니다. 열 형식이 일반, 숫자 또는 텍스트로 지정된 경우 가져오기가 실패합니다.

>[!TIP]
>
>가장 인기 있는 형식은 YYYY/MM/DD 형식입니다.
>
>예: 2023/07/10.

Workfront은 시간 값도 날짜의 일부로 허용합니다.

예: 07/10/2022 01:30 또는 07/10/2022 1:00 PM.

날짜에서 시간을 생략할 경우 Workfront은 다음 중 하나를 수행합니다.

* 이 시간은 오전 12:00이라고 가정합니다. 예상 날짜 결과를 보려면 시스템 시간대가 사용자의 시간대와 일치해야 합니다.
* 일정과 연관된 객체에 있는 경우 시간은 일정이 허용하는 가장 빠른 시간으로 지연됩니다.

>[!NOTE]
>
>UNIX 타임스탬프를 사용할 때는 값 끝에 3개의 추가 0을 포함해야 합니다.
>
>예를 들어 타임스탬프가 7336899000 셀에 7336899000000을 입력합니다.

### 와일드카드 사용 {#use-wildcards}

킥스타트 템플릿 스프레드시트를 채울 때 다음 와일드카드를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>와일드카드</strong> </p> </th> 
   <th> <p><strong>비헤이비어</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$오늘</p> </td> 
   <td> <p>에 사용되는 경우 <strong>setDate</strong> 필드, 이 와일드카드는 킥스타트를 가져오는 날의 날짜를 자정으로 설정합니다.</p> <p>필터에서 와일드카드에 허용된 표준 구문을 사용하여 와일드카드를 수정할 수 있습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>실제로 가져오기를 수행하는 요일에 관계없이 프로젝트를 가져온 주의 월요일에 시작하도록 하려면 다음을 사용할 수 있습니다. <strong>$$TODAYbw</strong>. 이렇게 하면 프로젝트의 계획된 시작 일자가 일요일 오전 12시로 설정됩니다. 그 시간에는 프로젝트 일정이 안 될 수도 있어서 월요일 아침 9시에 시작될 거야.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>에 사용되는 경우 <strong>setDate</strong> 필드, 이 와일드카드는 킥스타트 가져오기 중에 레코드를 만드는 순간에 따라 날짜를 설정합니다.</p> <p>필터에서 와일드카드에 허용된 표준 구문을 사용하여 와일드카드를 수정할 수 있습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>프로젝트를 가져온 후 3시간 후에 시작하려면 다음을 사용할 수 있습니다. <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>에 사용되는 경우 <strong>setAssignedToID</strong> 또는 기타 userID 기반 필드인 경우 이 와일드카드는 작업을 할당하거나 가져오기를 수행하는 개인과 레코드를 연결합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$고객</p> </td> 
   <td> <p>이 와일드카드는 특히 킥스타트 사용자 가져오기에 대해 추가되었습니다. Workfront 계정이 만들어지면 시스템 관리자 액세스 수준의 사용자가 만들어집니다. 기본 관리자에게 할당된 사용자 이름은 계정에서 다른 사용자를 만들 때 접두사로 사용할 수 있습니다.</p> <p>사용자 이름은 모든 고객에서 고유해야 하므로 John Smith와 같이 사용자 이름이 "jsmith"인 매우 일반적인 여러 개인이 있는 경우에 유용합니다. 사용자 이름 할당 앞에 기본 관리자 사용자 이름을 추가하면 각 사용자 이름이 고유합니다(예: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>팁: 사용자 이름이 시스템 전체에서 고유한지 확인할 수 있는 보다 우아한 방법은 개인 이메일 주소를 <strong>setUsername</strong> 필드.</p> </td> 
  </tr> 
 </tbody> 
</table>

### ID에 대한 속성 이름 대체  {#attribute-name-substitution-for-ids}

가능하면 ID를 사용하는 것이 좋지만 를 설정할 때 한 시트에서 다른 시트로 ID를 상호 참조하기가 불편한 경우가 있습니다 **setAttributeID** 값. 열 머리글을 변경하여 이름별로 값을 참조할 수 있습니다.

**예:**

* **프로젝트 가져오기**

  프로젝트를 가져올 때 **집합 ID** 로 이동하여 프로젝트 중 **그룹** 시트, 각 그룹 ID를 기록하고 올바른 셀에 붙여 넣습니다(**집합 ID** 열) **프로젝트 프로젝트** 시트.

  이는 몇 개의 그룹과 프로젝트만으로 작업할 때는 가능하지만, 여러 개의 그룹과 프로젝트를 수행하는 경우에는 실용적이지 않습니다.

  위에서 설명한 예에 대해 속성 이름 대체를 수행하려면 다음을 변경합니다 **집합 ID** 열 머리글에서 다음으로 **#setGroupID 이름 입력**. 그런 다음 이름별로 각 프로젝트의 그룹을 참조할 수 있습니다.

  >[!NOTE]
  >
  >속성 이름 대체를 사용하는 옵션은 기존 레코드에 대한 참조로만 제한됩니다. 동일한 가져오기에서 생성 중인 객체에는 이름 대체를 사용할 수 없습니다.

* **사용자 가져오기**

  사용자를 가져올 때 다음을 입력하십시오. **setRoleId** 의 역할 목록에서 **역할 역할** 탭.

  일부 역할 ID는 계정에 이미 존재하는 레코드에 대한 ID이고, 다른 ID는 가져오는 동안 만들어지는 ID입니다.

  기존 역할에 할당된 새 사용자 레코드의 경우 이름 대체를 사용할 수 있습니다. 새로 가져온 역할에 할당된 새 사용자 레코드의 경우에는 을(를) 수행할 수 없습니다.

  다음은 동일한 가져오기 파일에서 두 메서드를 모두 사용하는 방법입니다.

   * 스프레드시트의 왼쪽에 열을 추가합니다. **setRoleId** 열.
   * 새 열 이름 지정 **#setRoleID 이름 입력**.
   * 기존 레코드에 대한 역할 할당의 경우 **#setRoleID 이름 입력** 열.

     새 역할 레코드에 역할을 할당하려면 setRoleID의 역할 시트에 할당한 ID를 입력합니다.

     ![사용자의 역할 ID](assets/set-role-id.png)

## 스프레드시트 데이터를 Workfront으로 가져오기

Excel 템플릿을 데이터로 채운 후 해당 데이터를 Workfront에 업로드할 수 있습니다.

킥스타트 가져오기는 다음 파일 유형을 지원합니다.

* Excel (.xls 또는 .xlsx)
* 압축(.ZIP) 파일(.xlsx 또는 .xls 파일만 포함)

  >[!NOTE]
  >
  >다음 개체를 참조하는 Excel 스프레드시트를 가져올 때 .ZIP 파일을 사용해야 합니다.
  >
  >* 보고서
  >* 문서
  >* 아바타
  >* 속성 파일 보기, 필터링 또는 그룹화
  >
  >압축 가져오기 파일을 사용하는 경우 .ZIP 파일의 이름은 .xlsx 또는 .xls 파일과 같아야 하며 모든 파일의 구조 수준은 같아야 합니다(폴더 없음).

템플릿 스프레드시트 데이터를 Workfront으로 가져오려면 다음을 수행하십시오.

<!--1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. 클릭 **시스템** > **데이터 가져오기(킥스타트)**.

1. 다음에서 **킥스타트 스프레드시트로 데이터 업로드** 섹션, 클릭 **파일 선택**&#x200B;을 클릭한 다음 채워진 스프레드시트로 이동하여 선택합니다.

1. 클릭 **업로드.**

   Excel 파일을 Workfront에 업로드하는 데 5분 이상 걸리는 경우 애플리케이션 시간이 초과되어 Workfront에서 파일을 업로드할 수 없습니다.

   데이터를 더 작은 개체 배치로 가져오십시오.

1. (조건부) 이제 Workfront Fusion을 사용하는 경우 FLO 또는 시나리오를 설정할 수 있습니다.
