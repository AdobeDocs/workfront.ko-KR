---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 에서 모듈 또는 시나리오 복사 [!DNL Adobe Workfront Fusion]
description: 에서 모듈 또는 시나리오 복사 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# 에서 모듈 또는 시나리오 복사 [!DNL Adobe Workfront Fusion]

에서 모듈, 모듈 그룹 또는 전체 시나리오를 복사할 수 있습니다. [!DNL Adobe Workfront Fusion]. 이 기능을 사용하면 시나리오 또는 시나리오 일부를 다시 작성하지 않고도 재사용할 수 있습니다

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
  <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr>
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

모듈을 복사하려면 먼저 시나리오에 모듈을 추가해야 합니다.

## 모듈 또는 모듈 그룹 복사

모듈을 복사하면 원본 모듈의 필드 값과 설정이 모두 유지됩니다.

모듈을 동일한 시나리오의 다른 영역 또는 다른 시나리오에 붙여넣을 수 있습니다.

모듈을 다른 시나리오에 붙여넣을 때 다음 사항을 고려하십시오.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 복사하지 않은 다른 모듈에서 정보를 가져오는 필드 값은 더 이상 해당 정보에 액세스할 수 없습니다. 새 시나리오에서 정보를 가져오려면 이러한 필드를 설정해야 합니다.
* 다른 팀이나 조직이 소유한 시나리오에 모듈을 붙여넣으면 모든 연결을 새 시나리오를 소유한 그룹이나 조직이 소유한 연결로 업데이트해야 합니다.

### 모듈 복사

모듈 그룹을 복사하는 것은 단일 모듈을 복사하는 것과 비슷합니다.

1. 복사할 모듈을 마우스 오른쪽 버튼으로 클릭합니다.

   >[!NOTE]
   >
   >를 눌러 두 개 이상의 모듈을 선택할 수 있습니다. [!UICONTROL 이동] 복사할 모듈을 클릭합니다. 모듈 그룹을 복사하면 연결 라인, 필터 또는 모듈 간 라우팅 로직도 복사됩니다.

1. 선택 **[!UICONTROL 모듈 복사]**.
1. 시나리오를 복사할 시나리오의 영역으로 커서를 이동합니다.
1. 마우스 오른쪽 단추를 클릭하고 다음을 선택합니다. **[!UICONTROL 붙여넣기]**.
1. 붙여넣은 모듈을 시나리오의 적절한 위치로 끌어 시나리오에 연결합니다.

   키보드 단축키를 사용하여 복사하여 붙여넣을 수도 있습니다.

## 복제를 통해 시나리오 복사

시나리오를 복제하면 시나리오 사본이 만들어지고 편집할 수 있습니다.

1. 시나리오 세부 사항 페이지를 엽니다.

   1. 다음을 클릭합니다. **[!UICONTROL 시나리오]** 왼쪽 패널에서 을 탭한 다음 세부 정보를 보려는 시나리오를 클릭합니다.

      또는

      에서 시나리오를 작업 중인 경우 [의 시나리오 편집기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)왼쪽 화살표 클릭 ![](assets/exit-editing-arrow.png) 창의 왼쪽 상단 모서리 근처.

1. 마우스 오른쪽 버튼 클릭 **[!UICONTROL 옵션]** 페이지의 오른쪽 상단에 있습니다.
1. 선택 **[!UICONTROL 복제]**.
1. (선택 사항) 새 시나리오의 이름을 입력합니다.
1. (선택 사항) 활성화 **[!UICONTROL 새 모듈의 상태를 복제되는 모듈과 동일하게 유지]** 복사된 시나리오에 원래 시나리오에 의해 처리된 가장 최근 레코드에 대한 정보도 포함됩니다.
1. 클릭 **[!UICONTROL 저장]** 시나리오를 만들려면.

## 블루프린트를 사용하여 시나리오 복사

시나리오 블루프린트는 주어진 시점의 주어진 시나리오의 배열, 매핑 및 필드 값을 나타냅니다. 시나리오 블루프린트를 컴퓨터의 JSON 파일로 내보낸 다음 새 시나리오를 만들 때 가져올 수 있습니다. 시나리오 블루프린트에서 가져온 시나리오는 편집할 수 있습니다.

시나리오 블루프린트는 전체 시나리오를 나타냅니다. 시나리오에서 특정 모듈만 복사하려는 경우 다음을 참조하십시오. [모듈 또는 모듈 그룹 복사](#copy-a-module-or-a-group-of-modules) 이 문서에서.

>[!NOTE]
>
>컨텍스트 내 블루프린트에 대한 정보 [!DNL Adobe Workfront], 참조 [블루프린트 개요](../../administration-and-setup/blueprints/blueprints-overview.md).

### 시나리오 블루프린트 내보내기

1. 시나리오에서 **[!UICONTROL 자세히]** 시나리오 설정 영역의 메뉴 아래에 표시됩니다.
1. 클릭 **[!UICONTROL 블루프린트 내보내기]**.

   JSON 파일이 생성되고 컴퓨터에 다운로드됩니다. 다음 위치에서 이 파일을 찾을 수 있습니다. [!DNL Downloads] 폴더를 삭제합니다.

### 블루프린트 가져오기

>[!IMPORTANT]
>
>블루프린트를 기존 시나리오로 가져오는 경우 시나리오 블루프린트가 기존 시나리오를 대체합니다. 블루프린트를 기존 시나리오에 추가할 수 없습니다.

1. 새 시나리오 만들기를 시작합니다.
1. 시나리오에서 **[!UICONTROL 자세히]** 시나리오 설정 영역의 메뉴 아래에 표시됩니다.
1. 클릭 **[!UICONTROL 블루프린트 가져오기]**.
1. 표시되는 대화 상자에서 **[!UICONTROL 찾아보기]**
1. 가져올 블루프린트로 이동한 다음 를 클릭합니다. **[!UICONTROL 열기]**.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   JSON 파일이 생성되고 컴퓨터에 다운로드됩니다. 다음 위치에서 이 파일을 찾을 수 있습니다. [!UICONTROL 다운로드] 폴더를 삭제합니다.

## 템플릿을 사용하여 시나리오 복사 및 재사용

템플릿을 의 시작점으로 만들 수 있습니다. [!DNL Workfront Fusion] 시나리오. 템플릿에서 시나리오를 만들 때 템플릿을 수정하지 않고 시나리오를 수정할 수 있습니다. 필드 값은 템플릿에 저장되지 않습니다.

템플릿 만들기 및 사용에 대한 자세한 내용은 [시나리오 템플릿](../../workfront-fusion/scenarios/templates/fusion-templates.md).
