---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: 증명 생성 실패 문제 해결
description: 증명 작성 프로세스에는 가져오기 및 증명 생성이 모두 포함됩니다. 증명을 만들 때 파일을 가져오지 못하거나 파일을 가져온 후 증명을 생성하지 못하는 경우가 있습니다.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# 증명 생성 실패 문제 해결

증명 작성 프로세스에는 가져오기 및 증명 생성이 모두 포함됩니다. 증명을 만들 때 파일을 가져오지 못하거나 파일을 가져온 후 증명을 생성하지 못하는 경우가 있습니다.

>[!NOTE]
>
> 증명하려는 문서가 이 섹션에 나열된 기준과 일치하지 않는 경우 Adobe Workfront 지원 센터에 추가 조사를 문의하십시오.

## 가져오기 실패 이유

* 50개 이상의 파일이 포함된 결합된 증명을 만들었습니다.

## 증명 생성 실패 이유

* 지원되지 않는 파일 유형입니다.\
  지원되는 파일 형식 목록을 보려면 [지원되는 증명 파일 형식 및 크기 제한 개요](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)를 참조하십시오.

* 파일 구조는 파일 유형에 대한 비표준 구조입니다.
* 파일이 암호로 보호되어 있거나 콘텐츠 복사가 비활성화되어 있습니다.

  다른 유형의 파일과 달리 PDF 복사에 대한 보안 설정이 PDF에서 허용으로 설정되어 있으면 콘텐츠 파일을 증명으로 생성할 수 있습니다.

* 페이지 길이 또는 페이지 수가 한도를 초과했습니다.

  래스터화 후 최대 허용 페이지 길이는 195인치이고, 단일 증명에서 최대 허용 페이지 길이는 1,000페이지입니다.

* 파일이 손상되었거나 손상되었습니다.
* 새 증명 버전의 워크플로 마감이 과거입니다.

  이 문제는 빠른 증명 방법을 사용하여 새 증명 버전을 만들고 **문서 업로드 시 자동으로 증명 생성**&#x200B;을 선택한 경우에 발생합니다. 새 증명 버전은 이전에 생성한 증명에서 워크플로 기한을 고려합니다. 기한이 지난 경우 증명 생성이 실패합니다. 이를 해결하려면 향후 이전 버전에서 워크플로 기한을 설정하거나 새 증명 버전을 생성할 수 있습니다. 새 버전을 생성하는 경우 **자세히 > 새 버전 > 증명**&#x200B;을 사용하고 **향후 워크플로 기한**&#x200B;을 선택하십시오.

* 증명 PDF 파일 증명 시 증명 생성 실패의 원인은 다음과 같습니다.

   * 글꼴과 이미지는 외부 소스(예: 로컬 파일 시스템)에서 연결됩니다

     다른 컴퓨터나 Workfront Proof 내에 글꼴과 이미지를 표시하려면 PDF 파일에 글꼴과 이미지를 포함해야 합니다.

   * PDF 파일에 빈 레이어나 투명 또는 겹치는 필드가 포함되어 있습니다.

     이 문제를 일으키는 레이어나 오브젝트를 확인할 수 없는 경우 디자인/문서를 최적화된 PDF으로 내보냅니다(원치 않는 모든 요소가 제거됨).

