---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 자동화된 워크플로우를 사용하여 고급 증명 만들기
description: 자동화된 워크플로우를 사용하면 프로세스가 복잡하거나 검토를 위해 컨텐츠를 동일한 사람에게 정기적으로 보내는 경우 검토 프로세스를 보다 쉽게 관리할 수 있습니다. 증명은 스테이지에서 스테이지로 이동하고 Adobe Workfront은 검토할 때가 되면 각 사용자에게 알려줍니다. 자동화된 워크플로우에 대한 자세한 내용은 자동화된 워크플로우 개요를 참조하십시오.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# 자동화된 워크플로우를 사용하여 고급 증명 만들기

자동화된 워크플로우를 사용하면 프로세스가 복잡하거나 검토를 위해 컨텐츠를 동일한 사람에게 정기적으로 보내는 경우 검토 프로세스를 보다 쉽게 관리할 수 있습니다. 증명은 스테이지에서 스테이지로 이동하고 Adobe Workfront은 검토할 때가 되면 각 사용자에게 알려줍니다. 자동화된 워크플로우에 대한 자세한 내용은 [자동화된 워크플로우 개요](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

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
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 자동화된 워크플로우를 사용하여 고급 증명 만들기

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 탭.
1. 클릭 **새로 추가** > 증명, 컨텐츠를 업로드한 다음 아래 나열된 섹션을 통해 작동합니다.

   또는

   기존 문서를 마우스로 가리킨 다음 **증명 만들기** > **고급 증명** 및 아래 나열된 섹션을 통해 작업할 수 있습니다.

## 증명 단계 구성

1. 워크플로우 유형 섹션에서 **자동화된**.
1. (선택 사항) Workfront 관리자가 만들고 사용자와 공유한 자동화된 워크플로우 템플릿을 사용하려면 을 클릭합니다 **템플릿 추가**&#x200B;을 클릭하고 표시되는 상자에서 템플릿을 선택한 다음 를 클릭합니다. **템플릿 추가**.

   >[!NOTE]
   >
   >자동화된 워크플로우 템플릿을 사용할 때는 다음 사항을 고려하십시오.
   >   
   >* 자동화된 워크플로우 템플릿의 설정은 증명을 위해 자동화된 워크플로우를 사용하여 수행할 수 있는 작업을 결정합니다. 예를 들어 템플릿에서 스테이지 추가 단추가 비활성화된 경우 증명의 자동화된 워크플로우 설정을 사용하여 작업할 때에는 표시되지 않습니다.
   >* 사용자가 자동화된 워크플로우 템플릿의 용지에 추가되지만, 증명에 검토자로 이미 있으면 템플릿을 적용하면 검토자가 스테이지에서 제거됩니다. 스테이지에 다른 검토자를 추가하지 않으면 메시지를 통해 검토자를 추가하라는 메시지가 표시됩니다.
   >* 자동화된 워크플로우 템플릿을 수정하는 기능은 에 설명된 대로 Workfront 관리자가 구성한 템플릿 설정에 따라 다릅니다. 템플릿을 수정하는 기능이 비활성화되어 있으면 템플릿 소유자만 수정할 수 있습니다.


1. 자동화된 워크플로우의 첫 번째 단계를 구성합니다.

   1. (선택 사항) 첫 번째 단계의 이름을 만들려면 **1단계**&#x200B;를 입력한 다음 이름을 입력합니다.
   1. 에서 **수신자** 스테이지의 섹션에서 스테이지에 검토자를 추가합니다.

      >[!NOTE]
      > 
      >스테이지에 검토자를 추가할 때는 다음 사항을 고려하십시오.
      > 
      >* 전자 메일 주소가 있는 스테이지에 외부 사용자를 추가할 수 있습니다.
      >* 사용자를 스테이지에 추가한 후에는 증표에 해당 사용자에 대한 설정을 구성할 수 있습니다.
      >* 사용자를 다른 스테이지로 직접 드래그하거나 사용자를 스테이지로 드래그할 수 있습니다 **단계** 다이어그램. 여러 사용자를 선택하려면 Shift+Ctrl(Windows의 경우) 또는 Shift+Command(Mac의 경우)를 누릅니다.
      >* 한 번만 검토자를 증표에 추가할 수 있습니다. 이는 동일한 사람을 증명의 두 단계 이상에 추가할 수 없음을 의미합니다.
      >* 비공개 단계에 추가되지 않은 검토자는 해당 단계에서 작성한 증명 또는 댓글에 해당 단계를 볼 수 없습니다.
      >* 기본적으로 스테이지에 사용자를 추가하면 사용자가 증명을 만들 때부터 증명을 볼 수 있는 액세스 권한을 부여합니다.\
      >   Workfront 관리자는 워크플로우가 사용자가 추가된 단계에 들어갈 때까지 사용자에게 증명 액세스를 제한할 수 있습니다.


   1. 클릭 **스테이지 설정**.
   1. 클릭 **단계 활성화** 스테이지를 활성화할 방법을 나타내는 옵션입니다.

      첫 번째 단계에 대해서만 선택할 수 있습니다 **증명 작성 시**, **특정 날짜 및 시간에**, 또는 **수동으로**.

   1. (조건부) 선택한 경우 **특정 날짜 및 시간에** 이전 단계에서 스테이지를 활성화할 날짜와 시간을 선택합니다 **활성화** 상자가 표시됩니다.

   1. 다음 옵션 중 하나를 사용하여 스테이지를 추가로 구성합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">단계 최종 기한 설정</td>
         <td><p>스테이지의 기한을 설정하려면 <strong>최종 기한 옵션</strong> 드롭다운 목록. 그런 다음 <strong>기한</strong>다음 중 하나를 수행합니다.</p>
          <ul>
           <li>선택한 경우 <strong>특정 날짜 설정</strong>: 원하는 마감 날짜 및 시간을 선택합니다.</li>
           <li>선택한 경우 <strong>단계 활성화 날짜에서 계산</strong>: 단계 활성화 날짜에 추가할 비즈니스 일수를 선택하여 마감일을 결정합니다.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">스테이지 잠금</td>
         <td>스테이지를 잠글 수 있는 시기를 지정합니다. </td>
        </tr>
        <tr>
         <td role="rowheader">기본 의사 결정 권한을</td>
         <td><p>스테이지에서 기본 의사 결정자를 선택합니다(승인자 이상의 증명 역할이 있는 단계에 한 명 이상의 사람을 추가한 후에만 사용 가능). 1차 결정자를 선택하면 <strong>한 가지 결정만 필요합니다</strong> 이 단계에서 옵션을 사용할 수 없습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">이 단계에 대해 하나의 결정만 필요</td>
         <td>의사 결정권자 중 한 명이 결정을 내리면 전체 검토 프로세스를 종료합니다.<p>에서 사용자를 지정한 경우에는 이 옵션을 사용할 수 없습니다 <strong>주요 의사 결정권자</strong>드롭다운 메뉴</p></td>
        </tr>
        <tr>
         <td role="rowheader">이 스테이지를 비공개로 설정</td>
         <td>다음 사용자만 이 단계 동안 수행된 댓글 및 결정을 볼 수 있습니다. 감독, Workfront 관리자 및 Workfront 증명 관리자</td>
        </tr>
       </tbody>
      </table>

1. 다른 스테이지를 추가하고 구성하려면:

   1. 클릭 **새로운 단계**.
   1. (선택 사항) 첫 번째 단계의 이름을 만들려면 **2단계** 또는 **3단계**, **4단계**, 기타 등)를 입력한 다음 이름을 입력합니다.

   1. 을(를) 클릭합니다. **단계 활성화**&#x200B;그런 다음 옵션을 선택하여 스테이지의 활성화 여부를 자동으로 또는 수동으로 지정합니다.

      옵션 외에 **증명 작성 시**, **특정 날짜 및 시간에**, 또는 **수동으로**&#x200B;에서는 이전 단계에서 발생한 내용에 따라 달라지는 옵션을 선택할 수 있습니다.

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. 이전 단계에서 발생한 내용에 따라 단계 활성화 옵션을 선택한 경우 나타나는 옵션을 사용하여 활성화 설정을 구성합니다.

      예를 들어, **이전 단계 상태가 변경되는 경우**&#x200B;에서 을(를) 선택합니다. **이전 단계**&#x200B;를 선택한 다음, **상태가 (으)로 변경됨** 상자.

1. 단계를 더 추가하려면 필요한 경우 이전 단계를 반복합니다.

   자동화된 워크플로우에 단계를 추가하면 화면에 다이어그램 양식이 표시됩니다.

   ![](assets/stages-diagram-350x213.png)

1. 계속 [증명에 대한 이메일 설정 구성](#configure-email-settings-for-the-proof) 아래의 제품에서 사용할 수 있습니다.

## 증명에 대한 이메일 설정 구성 {#configure-email-settings-for-the-proof}

1. 에서 **이메일 알림** 섹션에서 선택한 사용자에게 이메일 알림 및 사용자 지정 메시지를 전송할지 여부를 선택합니다 [자동화된 워크플로우를 사용하여 고급 증명 만들기](#workflow) 이 문서의 앞 부분:

   <table>
      <tbody>
      <tr>
      <td>이 증명에 대해 수신자에게 알림</td>
      <td>사용자에게 이메일 알림을 전송하려면 이 옵션을 선택합니다. When <strong>기본 공유</strong> 에서 선택됨 <strong>워크플로우</strong> 섹션을 통해 증명을 만들 때 이메일 알림이 전송됩니다. When <strong>자동화된 워크플로우</strong> 에서 선택됨 <strong>워크플로우</strong> 섹션에 있는 경우, 증명으로 인해 사용자가 연결된 자동화된 워크플로우의 단계가 되면 이메일 알림이 전송됩니다.</td>
      </tr>
      <tr>
      <td>사용자 지정 메시지 추가</td>
      <td>알림에 사용자 지정 메시지를 포함하려면 이 옵션을 선택합니다. 제목과 메시지 본문을 지정할 수 있습니다. 메시지 본문에 굵게, 글머리 기호 및 하이퍼링크와 같은 서식 있는 텍스트 서식이 포함될 수 있습니다.</td>
      </tr>
      </tbody>
      </table>


1. 계속 [증명 설정 구성](#configure-proof-settings) 아래의 제품에서 사용할 수 있습니다.

## 증명 설정 구성 {#configure-proof-settings}

1. 에서 **증명 설정** 섹션에서 다음 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">로그인 필요 - 증명은 다른 사용자만 공유할 수 있습니다</td> 
      <td>이 옵션이 비활성화되어 있으면(기본값) URL을 가진 모든 사용자가 증명을 볼 수 있습니다. <br>이 옵션을 선택한 경우:
       <ul>
        <li>Workfront 증명 사용자만 증명을 볼 수 있습니다.</li>
        <li>증명에 추가되지 않으면 사용자가 증명에 로그인할 수 없습니다.</li>
        <li>구독을 사용하도록 설정할 수 없습니다.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 증명에 필요한 결정은 하나만</td> 
      <td>이 옵션을 선택하면 결정권자 중 한 명이 결정을 하면 리뷰가 완료됩니다.<br>이 옵션은 기본적으로 비활성화됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요</td> 
      <td>사용자는 증명을 결정할 때 사용자 이름과 암호를 지정해야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 모든 결정을 내릴 때 증명 잠금</td> 
      <td>이 설정을 사용하면 모든 결정을 수행한 후 증명 상태가 잠깁니다. 최종 승인자가 결정을 내릴 때 상태가 자동으로 잠금 해제에서 잠금으로 변경됩니다.<br>이 옵션은 기본적으로 비활성화됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">원본 파일 다운로드</td> 
      <td>이 옵션을 선택하면 검토자가 증명을 만든 원본 파일을 다운로드할 수 있습니다.<br>이 옵션을 선택 취소하면 더 이상 다운로드 아이콘이 표시되지 않습니다.<br>이 옵션은 기본적으로 활성화되어 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통해 증명 공유</td> 
      <td>이 옵션을 선택하면 공개 URL 또는 포함 코드를 통해 증명을 공유할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통해 증명 구독</td> 
      <td>이 옵션을 선택하면 증명에 명시적으로 추가되지 않은 사람이 증명에 가입할 수 있습니다. 증명을 구독하는 사람에게 다음 설정에서 정의하는 역할 및 전자 메일이 부여됩니다.
       <ul>
        <li><strong>가입자 역할:</strong> 증명을 구독하는 모든 검토자에게 할당된 기본 증명 역할입니다. </li>
        <li><strong>구독자에 대한 전자 메일 경고 설정:</strong> 증명을 구독하는 모든 검토자에게 할당된 기본 전자 메일 경고입니다.</li>
       </ul><p>
        <ul>
         <li><strong>다음에 필요한 이메일 링크를 통한 증명 액세스:</strong> 구독자가 증명 링크가 포함된 이메일을 수신하는지 여부를 구성합니다. 선택할 수 있습니다 <strong>이메일 없음</strong> (증명 액세스에 이메일 링크가 필요하지 않음), <strong>증명 알림 이메일만</strong> (구독자는 확인 없이 이메일을 통해 증명의 링크를 수신함) 또는 <strong>유효성 검사 및 증명 알림 이메일</strong> (구독자는 이메일을 통해 증명의 링크를 받고 링크를 클릭하여 증표에 액세스해야 하며, 이 옵션의 목적은 사용자가 액세스할 수 있는 올바른 이메일 주소를 입력했는지 확인하는 것입니다.)</li>
        </ul><p><strong>참고:</strong> 증명에 자동화된 워크플로우가 첨부된 경우 모든 구독이 증명 소유자에 대한 확인 이메일을 생성하므로 사용자가 추가되어야 하는 단계를 결정할 수 있습니다.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **증명 만들기**.

   Workfront에서 선택한 문서 또는 웹 사이트의 증명을 생성하기 시작합니다. 파일 크기와 유형에 따라 문서 업로드의 지연 시간이 다를 수 있습니다. 더 큰 파일이 생성되려면 시간이 더 오래 걸리므로 기다려 주십시오. 페이지에서 멀리 이동할 수 있으며 Workfront에서 계속해서 파일을 생성합니다. 최대 파일 업로드 크기는 4GB입니다.

1. 증명을 생성한 후 **공개 증명** 교정 뷰어를 실행하려면

   ![](assets/open-proof-350x132.png)

   계정에 언어 교정이 설정되어 있지 않은 사용자는 여전히 문서를 보고 증명에 주석을 달 수 있습니다 [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
