---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 업데이트
ms.date: 07/06/2020
description: Microsoft 365 학습 경로 업데이트
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 324bf41df1a6eec8d4646f3affdd48bedbbe3252
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000344"
---
# <a name="update-learning-pathways"></a>학습 경로 업데이트
기존 학습 경로 사이트가 있는 경우 다국어 지원을 위해 업데이트할 수 있습니다. 다국어 4.0 버전으로 학습 경로를 업데이트하려면 웹 파트 패키지 customlearning.sppkg를 SharePoint 테넌트 앱 카탈로그에 업로드합니다. 학습 경로를 업데이트하는 경우:  

- 이전에 만든 모든 사용자 지정 재생 목록 및 자산은 유지 관리됩니다.
- 콘텐츠를 숨기거나 표시하는 설정이 유지 관리됩니다.
- 학습 경로 SharePoint 서식 파일은 변경되지 않은 것으로 남아 있습니다.
- 학습 경로 사이트 페이지는 번역되지 않습니다. 이 작업을 수동으로 완료해야 합니다.

## <a name="read-the-learning-pathways-multilingual-overview"></a>학습 경로 다국어 개요 읽기
학습 경로에 다국어 지원이 작동하는 방식에 대한 자세한 내용은 학습 경로 다국어 [개요 를 참조하세요.](custom_overview.md) 

## <a name="prerequisites-to-update"></a>업데이트할 선행 준비
학습 경로를 업데이트하기 전에 다음 선행 준비를 충족해야 합니다.
- 학습 경로를 업데이트하는 사람은 테넌트 앱 카탈로그의 사이트 모음 소유자가 되어야 합니다. 학습 경로를 프로비저닝하는 사용자가 앱 카탈로그의 사이트 모음 소유자가 아닌 경우 이러한 [지침을 완료하고](addappadmin.md) 계속합니다. 

## <a name="set-language-settings"></a>언어 설정 설정 
학습 경로를 업데이트하기 전에 사이트 언어 설정을 설정하십시오. 학습 경로 사이트에 대한 다국어 지원을 사용하도록 설정하려면  페이지 및 뉴스를 여러 언어로 번역할 수 있도록 설정을 **으로** 설정한 다음 사이트에 대해 지원할 언어를 추가할 수 있습니다.
1.  학습 경로 사이트에서 오른쪽 상단의 설정을 선택한 다음 사이트 **정보를 선택합니다.** 
2.  사이트 정보 창의 아래쪽에서 모든 사이트 설정 보기 **를 선택합니다.**
3.  사이트 **관리에서** 언어 **설정을 선택합니다.**
4.  페이지 **및 뉴스를 여러** 언어로 번역할 수 있도록 설정에서 토글 스위치를 설정하십시오. 
- 다국어 사이트의 경우 토글을 **으로** 밀고 언어 추가 섹션으로 진행합니다. 
- 영어 전용 사이트의 경우 해제로 **토글합니다.**

### <a name="add-languages"></a>언어 추가
학습 경로는 9개 언어를 지원하고 필요한 언어만 추가해야 합니다. 이 설명서에 사용된 예제에서 이탈리아어가 추가됩니다. 
- 사이트 언어 추가 **또는 제거에서** 언어 선택 또는 입력에 언어 이름을 입력하거나 **드롭다운에서** 언어를 선택합니다. 이 단계를 반복하여 여러 언어를 추가할 수 있습니다. 이 페이지로 돌아가서 사이트에서 언어를 추가하거나 제거할 수 있습니다.
 
### <a name="assign-translators"></a>번역자 할당
학습 경로에 대한 언어 설정을 정의할 때 번역자를 할당할 수 있습니다. 번역자는 외래 언어 프로필을 설정해야 합니다. 외국어 프로필에 대한 자세한 내용은 다국어 통신 사이트, 페이지 및 뉴스 만들기를 [참조하세요.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)  
- 지원되는 언어의  경우 선택을 클릭하거나 번역을 입력한 다음 번역을 선택합니다. 

## <a name="update-the-learning-pathways-web-part-package"></a>학습 경로 웹 파트 패키지 업데이트
이 단계에서는 학습 경로 4.0 웹 파트를 SharePoint 앱 카탈로그에 업로드한 다음 학습 경로 관리 페이지로 이동하여 업데이트 프로세스를 시작합니다.

### <a name="upload-the-web-part-package"></a>웹 파트 패키지 업로드
1.  [GitHub](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)사용자 지정 학습 리포지토리로 이동하여 **customlearning.sppkg를** 선택한 다음 PC의 로컬 드라이브에 다운로드합니다.
2.  아직 로그인하지 않은 경우 테넌트 관리자 또는 사이트 모음 관리자 계정으로 테넌트에 로그인합니다. 
3.  관리자 **모든**  >  SharePoint **추가** 기능  >  **표시**  >  **를 클릭합니다.** 
4.  앱에서  **열기 를 클릭합니다.** 
5.    >  **SharePoint용 앱 카탈로그 배포를 클릭합니다.** 
6.  파일 **선택**  >  **업로드를 클릭합니다.** 
7.  다운로드한 **customlearning.sppkg** 파일을 선택하고 확인 **배포를**  >  **클릭합니다.** 

### <a name="complete-the-update"></a>업데이트 완료
1.  학습 경로 사이트에서 홈 메뉴에서 학습 **경로** 관리 **를** 선택합니다. 
2.  업데이트할지 묻는 메시지가 표시될 것입니다. 
![업데이트를 시작하라는 메시지가 표시됩니다.](media/custom_update_adminprompt_ml.png)
3.  **시작** 을 클릭합니다. 
4. 업데이트가 완료되면 닫기 **를 클릭합니다.** 

### <a name="next-steps"></a>다음 단계
- 사이트 [및 웹 파트에](custom_exploresite.md) 제공된 기본 콘텐츠를 살펴보겠습니다.
- 사이트 페이지 번역에 대한 자세한 내용은 사이트 페이지 [번역을 참조하세요.](custom_translate_page_ml.md) 

