---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 업데이트
ms.date: 05/20/2019
description: Microsoft 365 학습 경로 업데이트
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: cf058d0b8953f39a8243ffc91ab31fc5941c5674
ms.sourcegitcommit: 46caa9fa9d129bee107a8c9a7c5bc70a7f9af087
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2020
ms.locfileid: "44699131"
---
# <a name="update-microsoft-365-learning-pathways"></a>Microsoft 365 학습 경로 업데이트
기존 학습 경로 사이트가 있는 경우 다국어 지원을 위해 해당 사이트를 업데이트할 수 있습니다. 다국어 4.0 버전에 대 한 학습 경로를 업데이트 하려면 웹 파트 패키지, customlearning을 SharePoint 테 넌 트 앱 카탈로그에 업로드 합니다. 학습 경로를 업데이트할 때는 다음을 수행 합니다.  

- 이전에 만든 사용자 지정 재생 목록 및 자산은 모두 유지 관리 됩니다.
- 콘텐츠를 숨기 거 나 표시 하기 위한 설정이 유지 됩니다.
- 학습 경로 SharePoint 서식 파일이 변경 되지 않은 상태로 유지 됨
- 학습 경로 사이트 페이지는 번역 되지 않습니다. 이 작업을 수동으로 수행 해야 합니다.

## <a name="read-the-learning-pathways-multilingual-overview"></a>학습 경로 다국어 개요를 참조 하십시오.
다국어 지원이 경로 학습에 작동 하는 방식에 대 한 자세한 내용은 [학습 경로 다국어 개요](custom_overview_ml.md)를 참조 하세요. 

## <a name="prerequisites-to-update"></a>업데이트할 필수 구성 요소
학습 경로를 업데이트 하기 전에 다음 필수 구성 요소를 충족 해야 합니다.
- 학습 경로를 업데이트 하는 사람은 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다. 학습 경로를 프로 비전 하는 사람이 앱 카탈로그의 사이트 모음 소유자가 아닌 경우에는 [이러한 지침을 완료](addappadmin.md) 하 고 계속 진행 합니다. 

## <a name="set-language-settings"></a>언어 설정 설정 
학습 경로를 업데이트 하기 전에 사이트 언어 설정을 설정 합니다. 학습 경로 사이트에 다국어 지원을 사용 하도록 설정 하려면 **페이지 및 뉴스를 여러 언어로 번역할 수 있도록** 설정한 다음 해당 사이트에 대해 지원할 **언어를 추가**합니다.
1.  학습 경로 사이트의 오른쪽 위에서 **설정을** 선택한 다음 **사이트 정보**를 선택 합니다.
2.  사이트 정보 창 아래쪽에서 **모든 사이트 설정 보기**를 선택 합니다.
3.  **사이트 관리**에서 **언어 설정을**선택 합니다.
4.  **페이지 및 뉴스를 여러 언어로 번역할 수 있도록**설정 아래에서 toggle 스위치를 설정 합니다. 
- Multiligual 사이트의 경우 켜기/끄기를 설정 **으로 슬라이드**를 연 다음 언어 추가 섹션으로 이동 합니다. 
- 영어 전용 사이트의 경우이 기능을 **해제**로 슬라이드 전환 합니다.

### <a name="add-languages"></a>언어 추가
학습 경로에서는 9 개의 언어를 지원 하므로 필요한 언어만 추가 해야 합니다. 이 설명서에 사용 된 예에서는 이탈리아어가 추가 됩니다. 
- **사이트 언어 추가 또는 제거**에서 언어 이름 입력을 시작 **하거나 언어를 입력**하거나 드롭다운 목록에서 언어를 선택 합니다. 이 단계를 반복 하 여 여러 언어를 추가할 수 있습니다. 언제 든 지이 페이지로 다시 이동 하 여 사이트에서 언어를 추가 하거나 제거할 수 있습니다.
 
### <a name="assign-translators"></a>번역기 지정
학습 경로의 언어 설정을 정의할 때 번역기를 할당할 수 있습니다. 번역자에 게는 외국어 프로필이 설정 되어 있어야 합니다. 외국 언어 프로필에 대 한 자세한 내용은 [다국어 통신 사이트, 페이지 및 뉴스 만들기](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)를 참조 하세요.  
- 지원 되는 언어의 경우에는 **선택을 클릭 하거나 번역기를 입력** 한 다음 번역기를 선택 합니다. 

## <a name="update-the-learning-pathways-web-part-package"></a>학습 경로 웹 파트 패키지 업데이트
이 단계에서는 학습 경로 4.0 웹 파트를 SharePoint 앱 카탈로그에 업로드 한 다음, 학습 경로 관리 페이지로 이동 하 여 업데이트 프로세스를 시작 합니다.

### <a name="upload-the-web-part-package"></a>웹 파트 패키지 업로드
1.  팀의 다국어 공유 위치로 이동 하 고 PC의 로컬 드라이브에 **helloworld-webpart.sppkg** 를 다운로드 합니다. 
2.  아직 로그인 하지 않은 경우 테 넌 트 관리 또는 사이트 모음 관리자 계정을 사용 하 여 테 넌 트에 로그인 합니다. 
3.  **관리**  >  **모든**  >  **SharePoint**  >  **추가 기능**표시를 클릭 합니다. 
4.  **앱**에서 **열기**를 클릭 합니다. 
5.  **앱 카탈로그**  >  **배포 앱 for SharePoint를**클릭 합니다. 
6.  **Upload**  >  **파일 선택을**업로드 합니다 .를 클릭 합니다. 
7.  다운로드 한 **customlearning** 파일을 선택 하 고 **확인**  >  **배포**를 클릭 합니다. 

### <a name="complete-the-update"></a>업데이트 완료
1.  학습 경로 사이트의 **홈** 메뉴에서 **학습 경로 관리** 를 선택 합니다. 
2.  업데이트할 것인지 묻는 메시지가 표시 됩니다. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  **시작**을 클릭합니다. 
4. 업데이트가 완료 되 면 **닫기를**클릭 합니다. 

### <a name="next-steps"></a>다음 단계
- 사이트 및 웹 파트에서 제공 되는 [기본 콘텐츠](custom_exploresite.md) 를 살펴봅니다.
- 사이트 페이지 번역에 대 한 자세한 내용은 [번역 사이트 페이지](custom_translate_page_ml.md)를 참조 하십시오. 

