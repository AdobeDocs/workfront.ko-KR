---
title: 2024년 4분기 릴리스 개요
description: 이 페이지에서는 2024년 4분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 51e8faf8cc91546ccc1af551f359f81c2174c19b
workflow-type: tm+mt
source-wordcount: '2207'
ht-degree: 0%

---

# 2024년 4분기 릴리스 개요

이 페이지에서는 2024년 4분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.

<span class="preview">주기 외 기능(2024년 4분기 릴리스 날짜 이전에 프로덕션에 릴리스된 기능)은 노란색으로 강조 표시됩니다.</span>

>[!IMPORTANT]
>
>23.3 릴리스에는 조직을 월별 릴리스로 이동하는 옵션이 포함되었습니다. 따라서 Workfront은 월별 및 분기별 릴리스 트랙을 모두 고려하여 릴리스의 번호 지정 체계를 변경했습니다. 첫 번째 숫자는 연도를 지정하고 두 번째 숫자는 릴리스된 월을 나타냅니다. 예: 2024년 4월 릴리스는 24.4로 표시됩니다.
>
>월별 및 분기별 릴리스는 달리 지정하지 않는 한 해당 월의 두 번째 전체 주 목요일에 사용할 수 있습니다.
>
>| 월별 릴리스 | 분기별 릴리스 |
>|----|----|
>| <ul><li>24.8 (2024년 8월 15일)</li><li>24.9 (2024년 9월 12일)</li><li>24.10 (2024년 10월 17일)</li></ul> | <ul><li>24.10 (2024년 10월 17일)</li></ul> |
>
>각 분기의 최종 릴리스(이번 분기 24.10)의 경우 빠른 릴리스 일정을 사용하는 사용자는 하루 일찍 릴리스를 받게 됩니다.
>
>빠른 릴리스 프로세스에 대한 자세한 내용은 [빠른 릴리스 프로세스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하십시오.

## Adobe Workfront 개선 사항

* [관리자 개선 사항](#administrator-enhancements)
* [문서 관리 개선 사항](#document-management-enhancements)
* [홈 개선 사항](#home-enhancements)
* [통합 개선 사항](#integration-enhancements)
* [프로젝트 개선 사항](#project-enhancements)
* [증명 개선 사항](#proofing-enhancements)
* [보고서 및 대시보드 개선 사항](#report-and-dashboard-enhancements)
* [기타 개선 사항](#other-enhancements)
* [Workfront에서 곧 제거될 기능](#functionality-soon-to-be-removed-from-workfront)

### 관리자 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">이제 환경 프로모션에서 액세스 수준을 사용할 수 있습니다</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>환경 프로모션 기능의 기능을 확장하기 위해 액세스 수준을 포함하는 기능이 추가되었습니다. 이제 샌드박스 환경에서 액세스 수준을 구성한 다음 해당 액세스 수준을 프로덕션 환경으로 승격할 수 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 17일</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">사용자 정의 양식의 카운터가 필드 수를 표시합니다</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>사용자 정의 양식은 500개의 필드로 제한됩니다. 긴 형식에서는 형식에 몇 개의 필드가 있으며 한도에 도달하는지 여부를 알기 어려울 수 있습니다. 왼쪽 하단의 사용자 정의 양식에 카운터가 추가되었습니다. 카운터는 폼에 사용되는 필드 수를 표시하며 폼 디자이너 내에서 스크롤할 때 항상 표시됩니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 1일</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">이제 레이아웃 템플릿에서 "모두 선택" 옵션을 사용할 수 있습니다</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>레이아웃 템플릿으로 필드를 보다 쉽게 표시하거나 숨길 수 있도록 레이아웃 템플릿에서 세부 정보 보기의 개요 및 재무 영역에 "모두 선택" 확인란이 추가되었습니다. 이 옵션은 '사용자에게 표시되는 항목 사용자 지정' 아래에서 프로젝트, 작업, 문제, Portfolio 또는 프로그램을 선택한 경우에 사용할 수 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 8월 29일</p>
                        </li>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 8월 29일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">환경 프로모션 패키지 롤백</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>환경 프로모션을 보다 유연하고 쉽게 사용할 수 있도록 롤백 기능을 활성화했습니다. 이제 24시간 내에 패키지를 롤백하여 환경 프로모션 패키지의 영향을 받은 이전 구성을 보다 쉽게 복원할 수 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 8월 29일</p>
                        </li>
                        <li>
                            <p>빠른 릴리스를 위한 프로덕션: 24.9 릴리스 포함(2024년 9월 12일)</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    사용자 지정 양식 디자이너의 <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">레이아웃 단추는 두 개 또는 세 개의 열을 허용합니다</a></p>
                    <p>사용자 정의 양식 디자이너의 "레이아웃" 버튼을 사용하면 2열 또는 3열 작업 영역 중에서 선택할 수 있습니다. 원래 양식 디자이너는 세 개의 열을 사용하며 필드 설정은 맨 오른쪽 열에 표시됩니다. 두 개의 열을 선택하면 맨 왼쪽 열의 필드 라이브러리 옆에 필드 설정이 표시됩니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p><s>미리보기 릴리스: 2024년 8월 12일</s></p>
                        </li>
                        <li>
                            <p>빠른 릴리스를 위한 프로덕션: 해당 사항 없음</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 해당 사항 없음</p>
                        </li>
                    </ul>
                    <p><i>이 기능은 미리보기에서 제거되었으며 향후 릴리스와 함께 릴리스되지 않습니다.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### 문서 관리 개선 사항

>[!IMPORTANT]
>
>**문서 관리 개선 사항**&#x200B;에 나열된 기능은 단계별 릴리스의 일부이며, 특정 고객에게만 제공됩니다.

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">문서 목록에서 직접 문서 결정 상태 보기</a></p>
                    <p>이제 문서 목록에서 직접 문서의 결정 상태를 볼 수 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p><s>미리보기 릴리스: 2024년 10월 3일</s></p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">이전 검토자와 승인자를 새 문서 버전에 빠르게 추가</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>이제 이전 문서 버전에서 검토자와 승인자를 빠르게 추가할 수 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 3일</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### 홈 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">새 홈에서 내 승인 대기 중인 위젯에 대한 업데이트</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>내 승인 대기 위젯에 대해 다음과 같이 변경되었습니다.</p>
                        <ul>
                            <li>위젯 이름 변경됨: 이 위젯의 이름이 이제 내 승인입니다.</li>
                            <li>필터 옵션으로 제출한 승인이 추가되었습니다. 이제 이 위젯을 사용하여 새 홈에서 제출한 승인을 볼 수 있습니다.</li>
                            <li>기한: 이제 증명 기한이 설정된 경우 이를 볼 수 있습니다. 기한을 설정하지 않으면 기한의 기본값이 생성 일자로 설정됩니다.</li>
                        </ul>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 10일</p>
                        </li>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 10월 10일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">우선 순위 소개: 작업 소유자를 위한 단순하고 능률적이며 직관적인 Workfront 환경</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>우선 순위는 집중력과 생산성을 향상시켜 고객이 더 짧은 시간에 더 많은 성과를 달성하도록 지원합니다.</p>
                    <p>Priority 를 사용하면 다음과 같은 이점을 누릴 수 있습니다.</p>
                        <ul>
                            <li>일별 작업 관리 및 우선 순위 지정: 보다 명확성을 위해 통합 탐색으로 하루 또는 주일을 구성합니다.</li>
                            <li>생산성 향상: 클릭 수를 줄여 프로젝트 컨텍스트에 액세스하고 작업을 보다 신속하게 수행할 수 있습니다.</li>
                            <li>개인화된 기능: 작업 소유자를 위해 고유하게 설계된 기능의 이점을 누려보십시오.</li>
                        </ul>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 3일</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### 통합 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Outlook 통합 로그인 환경 개선 사항</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Outlook 통합에 대한 로그인 경험이 간소화되어 모든 고객이 IMS를 사용하는지 여부에 관계없이 Workfront에 로그인하는 동일한 버튼을 볼 수 있습니다. 이후 로그인 단계는 IMS 및 비 IMS 인스턴스에 대해 다르게 유지되지만 초기 페이지는 모든 사용자에 대해 동일합니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 8월 6일</p>
                        </li>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 8월 6일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### 프로젝트 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">새 작업 워크플로에 관련 할당이 더 추가됨</a></p>
                    [!BADGE In Production for Fast Release ]{type=Positive}
                    <p>프로젝트 및 프로젝트 작업 목록에 작업을 추가할 때 새 작업 상자의 할당 필드에 더 적절한 스마트 할당에 대해 동일한 기능을 추가했습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 2월 13일</p>
                        </li>
                        <li>
                            <p>빠른 릴리스를 위한 프로덕션: 24.5 릴리스 포함(2024년 5월 16일)</p>
                        </li>
                    </ul>
                <p><i>이 기능은 2024년 12월 19일 미리보기 및 25.1을 사용한 빠른 릴리스 프로덕션(2025년 1월)에서 제거됩니다.</i></p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">더 적절한 스마트 할당</a></p>
                    [!BADGE In Production for Fast Release ]{type=Positive}
                    <p>Workfront이 작업에 대한 스마트 할당을 계산하고 제안하는 데 사용하는 알고리즘을 변경했습니다. 새 알고리즘은 작업을 지정하는 Workfront의 작업 목록, 작업 헤더의 지정 영역, 홈 및 요약 패널에서 적용됩니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2023년 12월 21일</p>
                        </li>
                        <li>
                            <p>빠른 릴리스를 위한 프로덕션: 24.5 릴리스 포함(2024년 5월 16일)</p>
                        </li>
                    </ul>
                <p><i>이 기능은 2024년 12월 19일 미리보기 및 25.1을 사용한 빠른 릴리스 프로덕션(2025년 1월)에서 제거됩니다.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### 증명 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">데스크톱 증명 뷰어에 대한 복사/붙여넣기 문제 해결</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Desktop Proofing Viewer의 업데이트 섹션에서 콘텐츠가 잘못 붙여넣는 문제가 수정되었습니다.</p>
                    <p>신규 버전: 2.1.39</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 2일</p>
                        </li>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 10월 2일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">데스크톱 증명 뷰어 Windows 사용자를 위한 빈 화면 수정</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>일부 Windows 사용자가 뷰어를 연 후 빈 화면이 표시되는 새로운 2.1.36 Desktop Proofing Viewer 버전 문제를 해결했습니다. </p>
                    <p>Windows 사용자를 위한 새 버전: 2.1.37</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 8월 30일</p>
                        </li>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 8월 30일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">데스크톱 증명 뷰어에 대한 Chromium 업데이트</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>대화형 증명에서 UI 요소 문제를 해결하는 Chromium 126.0.6478.127을 지원하도록 데스크탑 증명 뷰어를 업그레이드하고 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 8월 29일</p>
                        </li>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 8월 29일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### 보고서 및 대시보드 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">기능</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">릴리스 날짜</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">새로운 플랜에 Workfront Data Connect 사용 가능</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Workfront Data Connect는 새로운 Workfront 계획 중 하나에 있는 조직에서 사용할 수 있습니다. Data Connect를 사용하면 조직은 비즈니스 인텔리전스 도구를 사용하여 분석하고 시각화하거나 외부에 저장할 수 있는 안전하고 확장 가능한 데이터 레이크로 데이터에 액세스할 수 있습니다. 또한 조직은 Data Connect를 사용하여 시간 기반 트렌드 분석, 변수 매핑, Workfront 데이터와 결합된 외부 시스템 데이터 분석과 같이 이전에 사용할 수 없었던 데이터 분석을 볼 수 있습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                    <p><i>새로운 Adobe Workfront 플랜 중 하나의 조직에서만 사용할 수 있습니다. Data Connect는 Ultimate 플랜에 포함되어 있으며 2025년 상반기에 Prime 및 Select 플랜의 추가 기능으로 구입할 수 있습니다.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### 기타 개선 사항

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">한 번의 클릭으로 프로젝트 또는 업데이트 요약</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>프로젝트 또는 업데이트 스트림의 주요 사항을 더 쉽게 볼 수 있도록 Workfront의 해당 영역에 요약 버튼을 추가했습니다. 이제 버튼을 클릭하여 AI Assistant에서 요약을 생성할 수 있습니다.</p><p>이전에는 사용자가 AI Assistant를 열고 프로젝트 요약을 생성하거나 스트림을 업데이트하라는 메시지를 입력할 수 있었습니다.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 10월 3일</p>
                        </li>
                        <li>
                            <p>모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Planning의 일반 가용성</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Workfront Planning은 Workfront 라이선스 외에 Workfront Planning 라이선스를 구입한 모든 고객이 사용할 수 있습니다. Workfront Planning에 대한 자세한 내용은 계정 담당자에게 문의하십시오.</p>
                    <p>분기별 최신 Workfront Planning 릴리스 정보는 아래의 <a href="#workfront-planning-enhancements">Workfront Planning 개선 사항</a> 섹션을 참조하십시오.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 2024년 8월 28일</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront에서 사용할 수 있는 Adobe AI 길잡이</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>작업을 보다 쉽게 수행할 수 있도록 Adobe의 AI Assistant를 Workfront에 추가했습니다. AI Assistant는 다음을 통해 도움을 줄 수 있습니다.</p>
                    <ul>
                        <li>작업 항목 및 문서를 요약하면 작업, 프로젝트 및 에셋에 대한 일반적인 이해를 신속하게 얻을 수 있습니다.</li>
                        <li>Experience League 설명서에서 정보를 제공하고, 지침과 참조 자료를 Workfront으로 가져오면서, 보다 심층적인 설명서로 연결합니다.</li>
                        <li>계산된 사용자 정의 양식 필드에 대한 수식 생성 및 세분화, 텍스트 프롬프트에서 수식 생성 또는 기존 수식에서 오류 찾기.</li>
                        </ul>
                        <p>Workfront 관리자는 조직에 대해 AI Assistant를 활성화하거나 비활성화할 수 있습니다. AI Assistant는 Select, Prime 및 Ultimate 플랜이 있는 인스턴스에 사용할 수 있습니다.</p>
                    </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 8월 28일</p>
                        </li>
                        <li>
                            <p class="preview">프로덕션 릴리스: 2024년 8월 28일</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2024년 4분기 동안의 룩앤필 업데이트</a></p>
                    <p>2024년 4분기 내에 Adobe Workfront 애플리케이션의 다양한 영역의 모양과 느낌에 대한 작은 업데이트가 이루어지고 있습니다. 특정 릴리스 날짜는 개별 릴리스 정보를 검토하십시오.</p>
                </td>
                <td><p><b>다음 날짜에 사용 가능:</b></p>
                    <ul>
                        <li>
                            <p>미리보기 릴리스: 2024년 4분기 릴리스 일정 전체</p>
                        </li>
                        <li>
                            <p><span class="preview">프로덕션 릴리스: 특정 날짜에 대한 릴리스 정보 검토</span></p>
                        </li>
                    </ul>
                </td>
            </tr>                            
        </tbody>
</table>

### Workfront에서 곧 제거될 기능

다음 기능은 곧 Workfront에서 제거될 예정입니다.

#### 24.10으로 기존 홈 환경 사용 중단

24.10 릴리스를 통해 기존의 홈 환경을 공식적으로 사용하지 않습니다. 사용자는 새로운 홈을 사용하는 것이 좋습니다. 홈은 사용이 중단되기 전에 추가 기능을 사용하여 계속 향상될 것입니다.

## 공지

### Workfront Fusion 개선 사항

Workfront Fusion의 새로운 기능은 2024년 4분기 릴리스 일정 이외의 케이던스로 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Fusion 릴리스 활동](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)을 참조하십시오.

### Workfront Planning 개선 사항

Workfront Planning의 새로운 기능은 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Planning 2024년 4분기 릴리스 활동](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md)을 참조하십시오.

### Workfront Scenario Planner 개선 사항

릴리스의 현재 시점에는 시나리오 플래너 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### Workfront Proof 개선 사항

릴리스의 현재 시점에는 Workfront Proof 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### Workfront 목표 개선 사항

릴리스의 현재 시점에는 Workfront 목표 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### API 버전 19

API 버전 19의 경우 일부 리소스 및 끝점을 수정했습니다. 일부 변경 사항은 새로운 기능을 지원하며, 다른 변경 사항을 통해 API를 통해 사용 가능한 정보를 보다 쉽게 사용할 수 있습니다.

새로운 기능 및 업데이트 내용은 [API 버전 19의 새로운 기능](/help/quicksilver/wf-api/api/new-api-version-19.md)을 참조하세요.

API 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 일정](/help/quicksilver/wf-api/api/api-version-support-schedule.md)을 참조하십시오.

### Workfront 유지 관리 업데이트

2024년 4분기 릴리스 중 유지 관리 업데이트에 대한 자세한 내용은 [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)를 참조하십시오.

### 교육 업데이트

각 Adobe Workfront 제품 릴리스의 학습 프로그램, 학습 경로, 비디오 및 안내서에 대한 최신 업데이트를 살펴보십시오. 자세한 내용은 [Workfront Tutorials 페이지](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)의 &quot;새로운 기능&quot; 섹션을 참조하십시오.
