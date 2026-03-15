---
title: 2024년 3분기 릴리스 개요
description: 이 페이지에서는 2024년 3분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# 2024년 3분기 릴리스 개요

이 페이지에서는 2024년 3분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.

라이브 24.7 릴리스 웨비나가 취소되었지만 [여기에서 24.7 기능에 대한 비디오 데모를 볼 수 있습니다](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">주기 외 기능(2024년 3분기 릴리스 날짜 이전에 프로덕션에 릴리스된 기능)은 노란색으로 강조 표시됩니다.</span>

>[!IMPORTANT]
>
>23.3 릴리스에는 조직을 월별 릴리스로 이동하는 옵션이 포함되었습니다. 따라서 Workfront은 월별 및 분기별 릴리스 트랙을 모두 고려하여 릴리스의 번호 지정 체계를 변경했습니다. 첫 번째 숫자는 연도를 지정하고 두 번째 숫자는 릴리스된 월을 나타냅니다. 예: 2024년 4월 릴리스는 24.4로 표시됩니다.
>
>월별 및 분기별 릴리스는 달리 지정하지 않는 한 해당 월의 두 번째 전체 주 목요일에 사용할 수 있습니다.
>
>| 월별 릴리스 | 분기별 릴리스 |
>|----|----|
>| <ul><li>24.5 (2024년 5월 16일)</li><li>24.6 (2024년 6월 13일)</li><li>24.7 (2024년 7월 18일)</li></ul> | <ul><li>24.7 (2024년 7월 18일)</li></ul> |
>
>빠른 릴리스 프로세스에 대한 자세한 내용은 [빠른 릴리스 프로세스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하십시오.

## Adobe Workfront 개선 사항

* [향상된 관리자 기능](#administrator-enhancements)
* [Financial Management 개선 사항](#financial-management-enhancements)
* [통합 개선 사항](#integration-enhancements)
* [프로젝트 개선 사항](#project-enhancements)
* [증명 개선 사항](#proofing-enhancements)
* [리소스 관리 개선 사항](#resource-management-enhancements)
* [기타 개선 사항](#other-enhancements)

### 향상된 관리자 기능

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">비즈니스 규칙을 사용할 수 있습니다.</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>이제 관리자는 Workfront의 설정 영역에서 비즈니스 규칙을 추가할 수 있습니다.</p>
                        <p>비즈니스 규칙을 사용하면 Workfront 객체에 검증을 적용하고 특정 조건이 충족될 때 사용자가 객체를 생성, 편집 또는 삭제하지 못하도록 할 수 있습니다. 규칙은 사용자 정의 양식의 계산된 필드와 유사한 공식을 사용하여 작성됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 7월 4일</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)</p>
                            </li>
                        </ul>
                        <p><i>새 Ultimate 플랜의 조직에서만 사용할 수 있습니다.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Adobe Workfront에서 일반적으로 사용할 수 있는 사용자 정의 양식 디자이너</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>24.7 릴리스에서는 양식 디자이너를 일반적으로 사용할 수 있으며, Adobe Workfront에서 사용자 정의 양식을 만들고 편집할 수 있는 기본 환경이 됩니다. 새 사용자 정의 양식을 만들거나 기존 양식을 열면 양식 디자이너의 캔버스 스타일 작업 영역이 표시됩니다.</p>
                        <p>이 릴리스 이후, 이전 양식 빌더로 되돌리는 옵션은 더 이상 사용할 수 없게 됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리 보기 릴리스: 2024년 6월 19일</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">환경 프로모션을 사용하여 Workfront 환경 간에 개체 이동</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>환경 프로모션을 사용하면 샌드박스 환경에서 프로덕션 환경으로 등 Workfront 환경 간에 개체를 이동할 수 있습니다. 조직의 데이터 및 레코드에 대한 위험 없이 개체를 구성하고 테스트할 수 있습니다. 그런 다음 재구성하지 않고도 이러한 객체를 프로덕션으로 이동하여 시간과 노력을 절약할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.6 릴리스 포함(2024년 6월 13일)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">사용자 지정 양식 디자이너에서 사용자 지정 양식 및 사용자 지정 필드 공유</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>이제 새 양식 디자이너에서 사용자 지정 양식과 사용자 지정 필드를 모두 공유할 수 있습니다. 이를 통해 사용자 지정 양식에서 사용자 간의 협업을 향상시킬 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리 보기 릴리스: 2024년 6월 6일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션 릴리스: 6월 13일</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">필드 영역에서 새 사용자 지정 필드 추가</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>이제 필드를 만들기 위한 사용자 지정 양식을 열지 않고도 Workfront의 필드 영역에서 직접 새 사용자 지정 필드 또는 위젯을 추가할 수 있습니다. 이렇게 하면 재사용 가능한 사용자 지정 필드를 빠르게 만들 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리 보기 릴리스: 2024년 6월 6일</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">양식 디자이너에서 사용할 수 있는 다중 선택 드롭다운 필드 형식</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>드롭다운 필드를 보다 쉽게 정의할 수 있도록 다중 선택 드롭다운 필드를 사용자 정의 양식 디자이너에 추가했습니다. 이 필드 유형을 사용하면 드롭다운 목록에서 두 개 이상의 옵션을 선택할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 6월 4일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2024년 6월 4일</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 향상된 Financial Management

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">프로젝트 및 작업에 사용할 수 있는 청구 가능 및 청구 불가능한 비용 필드</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>경비 유형을 보다 쉽게 볼 수 있도록 하기 위해, 경비는 프로젝트 및 태스크에서 청구 가능 경비와 청구 불가능 경비로 구분되었습니다. 보기 및 보고서에 추가할 수 있는 필드는 다음과 같습니다.</p>
                        <ul>
                            <li><p>계획된 청구 가능 경비 비용</p></li>
                            <li><p>청구 불가능한 계획된 경비</p></li>
                            <li><p>실제 청구 불가능한 비용 원가</p></li>
                            <li><p>실제 청구 불가능한 비용 원가</p></li>
                        </ul>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리 보기 릴리스: 2024년 5월 10일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2024년 5월 10일</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Experience Manager Assets 및 Assets Essentials 개선 사항용 Workfront</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Experience Manager Assets 및 Assets Essentials 통합을 위한 Workfront을 다음과 같이 개선했습니다.</p>
                        <ul>
                            <li><p>통합은 이제 클라우드 서비스 공급자로서 GCP를 지원합니다. 이전에 AWS 및 Azure이 지원되었습니다.</p></li>
                            <li><p>통합을 통해 Experience Manager으로 전송된 파일의 크기 제한이 30GB로 늘어났습니다. 이전에는 5GB로 제한되었습니다.</p></li>
                        </ul>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 6월 27일</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션: 24.7 릴리스 포함(2024년 7월 18일)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">헤더 또는 세부 정보 섹션에서 작업 및 문제 커밋 일자 및 조건을 편집합니다</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>이제 작업 및 문제를 보다 쉽게 업데이트할 수 있도록 레이아웃 템플릿의 작업 및 문제 헤더와 세부 정보 섹션에 추가할 수 있는 옵션으로 커밋 날짜 및 조건 필드를 추가했습니다. 이제 사용자는 수정된 레이아웃 템플릿에 할당될 때 페이지의 헤더 또는 세부 정보 섹션에서 이러한 필드를 업데이트할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 5월 30일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.6 릴리스 포함(2024년 6월 13일)</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">새 작업 워크플로우에 추가 관련 할당</a></p>
                        [!BADGE 빠른 릴리스를 위한 프로덕션 중 ]{type=Positive}
                        <p>프로젝트 및 프로젝트 태스크 목록에 태스크를 추가할 때 신규 태스크 상자의 지정 필드에 관련성이 높은 스마트 지정에 대해 동일한 기능을 추가했습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리 보기 릴리스: 2024년 2월 13일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.5 릴리스(2024년 5월 16일)</p>
                            </li>
                        </ul>
                    <p><i>이 기능은 미리 보기 및 빠른 릴리스 프로덕션에서 제거되었습니다.</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">더 관련성 있는 스마트 할당</a></p>
                        [!BADGE 빠른 릴리스를 위한 프로덕션 중 ]{type=Positive}
                        <p>Workfront에서 작업에 대한 스마트 할당을 계산하고 제안하는 데 사용하는 알고리즘을 변경했습니다. 새 알고리즘은 Workfront에서 작업을 할당하는 영역(작업 목록, 작업 헤더의 할당 영역, 홈 및 요약 패널)에 적용됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 21일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.5 릴리스(2024년 5월 16일)</p>
                            </li>
                        </ul>
                    <p><i>이 기능은 미리 보기 및 빠른 릴리스 프로덕션에서 제거되었습니다.</i></p>
                    </td>
                 </tr>
           </tbody>
        </table>

### 언어 교정 개선 사항

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">데스크톱 증명 뷰어에 대한 보안 업데이트</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Workfront Proof Desktop Proofing Viewer 2.1.35 보안 업데이트는 이전 릴리스에서 식별된 취약점에 대한 보안 버그 수정 사항을 제공합니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 7월 4일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2024년 7월 4일</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 향상된 리소스 관리 기능

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">휴무가 업무 균형자에 반영됨</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>작업 로드 밸런서는 작업의 1차 피할당자가 휴식 시간을 예약한 경우 작업을 원활하게 조정하기 위해 이제 프로젝트 타임라인이 다시 계산될 때 1차 사용자와 2차 사용자 모두에게 시간을 재할당합니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 6월 6일</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)</p>
                            </li>
                        </ul>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">제품 내 안내서에 대한 백엔드 변경</a></p>
                        <p>향후 몇 주 동안 제품 내 안내서에 대한 기술 변경을 구현하고 있습니다. 이 전환의 영향을 최소화하려고 노력했지만 일부 사용자는 이전에 본 안내서를 접할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>모든 고객을 위한 프로덕션: 2024년 8월 중순까지 점진적으로</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">이제 더 많은 Workfront 조직에서 Adobe 통합 경험을 사용할 수 있습니다.</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>조직이 Adobe 통합 경험의 이점을 이용할 수 있도록 기존 Workfront 고객이 사용할 수 있도록 하기 시작했습니다. </p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리 보기 릴리스: 2024년 6월 20일</p>
                            </li>
                            <li>
                                <p>지정된 고객을 위한 프로덕션: 24.7 릴리스(2024년 7월 18일)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Adobe 통합 셸을 단계적 롤아웃에서 사용할 수 있도록 하고 있습니다. 추가 조직은 24.10 및 25.1 릴리스와 함께 Adobe 통합 셸로 온보딩됩니다. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">도움말 단추가 기본 탐색 모음에서 제거되었습니다.</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>통합 셸에 없는 사용자의 경험을 통합하기 위해 기본 탐색 모음의 도움말 단추가 제거되었습니다. 통합 셸의 사용자에게 제공되지 않는 이 단추는 Workfront 설명서에 연결되어 있으며 기본 메뉴의 모든 사용자에게 사용할 수 있는 유사한 도움말 단추와 함께 이중화되었습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 6월 6일</p>
                            </li>
                            <li>
                                <p>모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">개체 액세스가 제한된 사용자를 위한 UI 환경 개선</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>사용자에게 오브젝트에 대한 액세스 권한이 없는 경우 Workfront에 해당 오브젝트 이름이 표시되는 모든 위치에 "액세스 권한 없음"이 표시됩니다. 이러한 향상된 경험은 Workfront API에도 적용됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 3월 27일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.5 릴리스 포함(2024년 5월 16일)</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 생산: 24.7 릴리스(2024년 7월 18일)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2024년 3분기 기간 동안의 룩앤필 업데이트</a></p>
                        <p>Adobe Workfront 애플리케이션의 다양한 영역에 대한 모양과 느낌에 대한 작은 업데이트는 2024년 3분기 내에 수행됩니다. 특정 릴리스 날짜에 대한 개별 릴리스 정보를 검토하십시오.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>릴리스 미리 보기: 2024년 3분기 릴리스 기간 동안</p>
                            </li>
                            <li>
                                <p><span class="preview">프로덕션 릴리스: 특정 날짜에 대한 릴리스 노트를 검토합니다.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## 공지

### Workfront Fusion 개선 사항

Workfront Fusion의 새로운 기능은 2024년 3분기 릴리스 일정 이외의 케이던스에서 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Fusion 릴리스 활동](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)을 참조하십시오.

### Workfront Scenario Planner 향상

이 릴리스에는 시나리오 계획자 업데이트가 없습니다. 이 영역은 업데이트를 사용할 수 있을 때 업데이트됩니다.

### Workfront Proof 개선 사항

이 릴리스에는 현재 Workfront Proof 업데이트가 없습니다. 이 영역은 업데이트를 사용할 수 있을 때 업데이트됩니다.

### Workfront 목표 개선 사항

현재 릴리스에는 Workfront 목표 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### API 버전 18

API 버전 18의 경우 일부 리소스 및 끝점을 수정했습니다. 일부 변경 사항은 새로운 기능을 지원하며, 다른 변경 사항을 통해 API를 통해 사용 가능한 정보를 보다 쉽게 사용할 수 있습니다.

새로운 기능 및 업데이트 내용은 [API 버전 18의 새로운 기능](/help/quicksilver/wf-api/api/new-api-version-18.md)을 참조하세요.

API 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 일정](/help/quicksilver/wf-api/api/api-version-support-schedule.md)을 참조하십시오.

### Workfront 유지 관리 업데이트

2024년 3분기 릴리스 동안 이루어진 유지 관리 업데이트에 대한 자세한 내용은 [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/ko/docs/workfront-known-issues/releases/current-updates)를 참조하십시오.

### 교육 업데이트

각 Adobe Workfront 제품 릴리스의 학습 프로그램, 학습 경로, 비디오 및 안내서에 대한 최신 업데이트를 살펴보십시오. 자세한 내용은 [Workfront 자습서 페이지](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/home)의 &quot;새로운 기능&quot; 섹션을 참조하십시오.
