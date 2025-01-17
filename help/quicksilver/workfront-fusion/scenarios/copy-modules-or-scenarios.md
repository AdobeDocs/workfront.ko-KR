---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion]에서 모듈 또는 시나리오 복사'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 모듈 또는 시나리오 복사

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [모듈 또는 시나리오 복사](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/copy-modules-or-scenarios.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion]에서 모듈, 모듈 그룹 또는 전체 시나리오를 복사할 수 있습니다. 이 기능을 사용하면 시나리오 또는 시나리오 일부를 다시 작성하지 않고도 재사용할 수 있습니다

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr>
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

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
   >[!UICONTROL shift]를 누른 채 복사할 모듈을 클릭하면 둘 이상의 모듈을 선택할 수 있습니다. 모듈 그룹을 복사하면 연결 라인, 필터 또는 모듈 간 라우팅 로직도 복사됩니다.

1. **[!UICONTROL 모듈 복사]**&#x200B;를 선택합니다.
1. 시나리오를 복사할 시나리오의 영역으로 커서를 이동합니다.
1. 마우스 오른쪽 단추를 클릭하고 **[!UICONTROL 붙여넣기]**&#x200B;를 선택합니다.
1. 붙여넣은 모듈을 시나리오의 적절한 위치로 끌어 시나리오에 연결합니다.

   키보드 단축키를 사용하여 복사하여 붙여넣을 수도 있습니다.

## 복제를 통해 시나리오 복사

시나리오를 복제하면 시나리오 사본이 만들어지고 편집할 수 있습니다.

1. 시나리오 세부 사항 페이지를 엽니다.

   1. 왼쪽 패널의 **[!UICONTROL 시나리오]** 탭을 클릭한 다음 자세히 설명하려는 시나리오를 클릭합니다.

      또는

      [의 시나리오 편집기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)에서 시나리오를 작업하는 경우 창의 왼쪽 위 모서리 근처에 있는 왼쪽 화살표 ![](assets/exit-editing-arrow.png)을(를) 클릭합니다.

1. 페이지 오른쪽 상단의 **[!UICONTROL 옵션]**&#x200B;을 마우스 오른쪽 단추로 클릭합니다.
1. **[!UICONTROL 복제]**&#x200B;를 선택합니다.
1. (선택 사항) 새 시나리오의 이름을 입력합니다.
1. (선택 사항) 복사한 시나리오에 원본 시나리오에서 처리한 최신 레코드에 대한 정보도 포함되도록 **[!UICONTROL 복제되는 모듈과 동일한 새 모듈의 상태를 유지]**&#x200B;합니다.
1. 시나리오를 만들려면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 블루프린트를 사용하여 시나리오 복사

시나리오 블루프린트는 주어진 시점의 주어진 시나리오의 배열, 매핑 및 필드 값을 나타냅니다. 시나리오 블루프린트를 컴퓨터의 JSON 파일로 내보낸 다음 새 시나리오를 만들 때 가져올 수 있습니다. 시나리오 블루프린트에서 가져온 시나리오는 편집할 수 있습니다.

시나리오 블루프린트는 전체 시나리오를 나타냅니다. 시나리오에서 특정 모듈만 복사하려면 이 문서의 [모듈 또는 모듈 그룹 복사](#copy-a-module-or-a-group-of-modules)를 참조하십시오.

>[!NOTE]
>
>[!DNL Adobe Workfront]의 컨텍스트에서 블루프린트에 대한 자세한 내용은 [블루프린트 개요](../../administration-and-setup/blueprints/blueprints-overview.md)를 참조하십시오.

### 시나리오 블루프린트 내보내기

1. 시나리오에서는 시나리오 설정 영역의 **[!UICONTROL 자세히]** 메뉴를 클릭합니다.
1. **[!UICONTROL 블루프린트 내보내기]**&#x200B;를 클릭합니다.

   JSON 파일이 생성되고 컴퓨터에 다운로드됩니다. [!DNL Downloads] 폴더에서 이 파일을 찾을 수 있습니다.

### 블루프린트 가져오기

>[!IMPORTANT]
>
>블루프린트를 기존 시나리오로 가져오는 경우 시나리오 블루프린트가 기존 시나리오를 대체합니다. 블루프린트를 기존 시나리오에 추가할 수 없습니다.

1. 새 시나리오 만들기를 시작합니다.
1. 시나리오에서는 시나리오 설정 영역의 **[!UICONTROL 자세히]** 메뉴를 클릭합니다.
1. **[!UICONTROL 블루프린트 가져오기]**&#x200B;를 클릭합니다.
1. 표시되는 대화 상자에서 **[!UICONTROL 찾아보기]**&#x200B;를 클릭합니다
1. 가져올 블루프린트로 이동하여 **[!UICONTROL 열기]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   JSON 파일이 생성되고 컴퓨터에 다운로드됩니다. [!UICONTROL 다운로드] 폴더에서 이 파일을 찾을 수 있습니다.

## 템플릿을 사용하여 시나리오 복사 및 재사용

[!DNL Workfront Fusion] 시나리오의 시작점으로 템플릿을 만들 수 있습니다. 템플릿에서 시나리오를 만들 때 템플릿을 수정하지 않고 시나리오를 수정할 수 있습니다. 필드 값은 템플릿에 저장되지 않습니다.

템플릿 만들기 및 사용에 대한 자세한 내용은 [시나리오 템플릿](../../workfront-fusion/scenarios/templates/fusion-templates.md)을 참조하세요.
