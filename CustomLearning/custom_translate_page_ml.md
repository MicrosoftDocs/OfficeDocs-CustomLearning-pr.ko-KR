---
author: pkrebs
ms.author: pkrebs
title: 사이트 페이지 번역
ms.date: 02/10/2019
description: 사이트 페이지 번역
ms.openlocfilehash: cf397250ceab826efb8b82522c0560c2109d24bb
ms.sourcegitcommit: f355885fb93d66abf61df535fa704ccdb8df9b64
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/05/2020
ms.locfileid: "45038988"
---
# <a name="translate-site-pages"></a>사이트 페이지 번역
학습 경로 사이트 번역을 시작 하기 전에 다국어 기능이 학습 경로에서 작동 하는 방식에 대 한 몇 가지 주요 개념을 이해 하는 것이 중요 합니다. 
- 사이트 정보-탐색, 로고 및 사이트 이름 번역을 사용 하려면 사용자의 언어 프로필에서 사이트를 보고 번역 해야 합니다.  
- 사용자의 언어 프로필로 학습 경로 웹 파트를 확인 하 여 영어가 아닌 언어로 표시 해야 합니다. 웹 파트 및 Microsoft 제공 콘텐츠가 이미 번역 되었습니다. 언어 프로필에 대 한 자세한 내용은 [개인 언어 및 국가별 설정 변경을](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)참조 하세요.
- 학습 경로를 설정 하는 방법에 따라 번역 된 페이지를 사용할 수 있는지 여부가 결정 됩니다. SharePoint 프로 비전 서비스를 사용 하 여 프로 비전 된 새 사이트는 사용 가능한 9 개 언어의 페이지를 번역 합니다. 사용자가 만든 사이트 또는 사이트를 업데이트 하면 수동 번역을 수행 해야 합니다. [다국어 학습 경로의 설치 옵션을](custom_setupoptions_ml.md)참조 하세요.
- 정보 교환 경로에 대 한 다국어 지원은 통신 사이트용 SharePoint Online 다국어 기능을 통해 사용 하도록 설정 됩니다. SharePoint Online 다국어 기능에 대 한 자세한 내용은 [다국어 통신 사이트, 페이지 및 뉴스 만들기](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)를 참조 하세요. 

## <a name="working-with-a-newly-provisioned-site"></a>새로 프로 비전 된 사이트 사용
SharePoint 프로 비전 서비스에서 새 학습 경로 사이트를 프로 비전 한 경우 번역 된 페이지를 이미 사용할 수 있습니다. 기본적으로 사이트에서는 다음과 같은 페이지를 제공 합니다.

- Home.aspx
- Start-with-Six-Simple-Steps .aspx
- Get-started-with-Microsoft-365 .aspx
- Get-started-with-Microsoft-Teams .aspx
- Get-started-with-SharePoint .aspx
- Get-started-with-OneDriive .aspx
- Ask-questions-and-get-help .aspx
- 교육 이벤트 일정 .aspx
- Become-a-Champion .aspx
- Recommended-Playlists .aspx
- 학습 경로 관리 성공 센터

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>새로 프로 비전 한 사이트에서 번역 된 페이지 보기
번역 된 학습 경로 사이트를 익힐 수 있도록 몇 가지 번역 된 페이지를 확인 하세요.

### <a name="view-the-translated-home-page"></a>번역 된 홈 페이지 보기
학습 경로 홈 페이지의 다음 예와 같이 언어 드롭다운에서 언어를 선택 합니다. 이 예제에서는 오른쪽 위 모서리에 선택 된 이탈리아어를 표시 하 고 모든 페이지 요소를 변환 합니다.

![custom_ml_pages_home.png](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>번역 된 Microsoft 365 교육 페이지 보기
이제 Microsoft 365 교육 페이지를 살펴보겠습니다. 

1. 학습 경로 사이트 **홈** 페이지에서 **Microsoft 365 교육**을 클릭 합니다.
2. 페이지의 오른쪽 위 모서리에서 언어를 선택 합니다. 이 예에서는 이탈리아어가 선택 되어 있습니다.

![custom_ml_pages_training.png](media/custom_ml_pages_training.png)

언어를 선택 하면 표시 되는 번역은 무엇입니까?
- 위 그림에 표시 된 대로 SharePoint 페이지가 번역 됩니다. 페이지 배너의 텍스트가 현재 이탈리아어로 표시 되어 있습니다.

번역이 표시 되지 않는 경우
- 사이트 이름이 영어로 되어 있습니다.
- 사이트 탐색이 영어로 되어 있습니다.
- 학습 경로 웹 파트가 영어로 되어 있습니다.

## <a name="view-the-fully-translated-site"></a>완전히 번역 된 사이트 보기 
사이트 페이지, 탐색, 웹 파트 등의 특정 언어로 전체 변환 된 사이트를 보려면 해당 언어에 대해 사용자의 개인 언어 및 국가별 설정을 지정 해야 합니다. 언어 및 국가별 설정 설정에 대 한 자세한 내용은 [개인 언어 및 국가별 설정 변경을](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)참조 하십시오. 별도의 계정을 사용 하거나 다른 언어 설정을 사용 하는 다른 사용자에 게 번역 된 페이지를 표시 하는 것이 좋습니다.  

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>업데이트 되거나 수동으로 설치 된 학습 경로 사이트를 사용 하 여 작업
기존 학습 경로 사이트를 업데이트 하거나 기존 사이트에 웹 파트를 수동으로 설치한 경우 사이트 페이지를 수동으로 번역 해야 합니다. 학습 경로 웹 파트 및 콘텐츠는 이미 번역 되어 사용자의 기본 설정 언어로 표시 됩니다. 페이지를 변환 하려면 "원하는 언어에 대 한 페이지 만들기" 지침을 참조 하십시오. 

## <a name="create-pages-for-the-languages-you-want"></a>원하는 언어에 대 한 페이지 만들기
다국어 기능에 대 한 사이트를 사용 하도록 설정 하 고 사용 가능 하도록 설정할 언어를 선택한 후에는 원하는 번역 페이지를 만들 수 있습니다. 

1. 다른 언어로 사용할 수 있도록 설정할 기본 언어 페이지로 이동 합니다.
2. 위쪽 막대에서 **번역**을 선택 합니다.
3. 원하는 언어에 대해 **만들기** 를 선택 합니다.

> [!IMPORTANT]
> 번역 페이지를 만든 후에는 기본 언어 페이지를 게시 하거나 다시 게시 해야 다음을 확인할 수 있습니다.
>- 번역 페이지는 해당 언어 사이트에 표시 됩니다.
>- 번역 페이지는 뉴스 웹 파트 및 강조 표시 된 콘텐츠 웹 파트에서 올바르게 표시 됩니다.
>- 사이트 위쪽의 언어 드롭다운에서 사용 하도록 설정한 모든 언어를 포함 합니다.
>- 번역자는 번역 요청에 대 한 알림을 받습니다.

페이지를 만든 후에는 번역 창에서 각 언어 옆에 페이지 상태 (임시 저장, 게시 됨 등)가 표시 됩니다. 또한 할당 한 번역자에 게 번역이 요청 됨을 알리는 전자 메일 알림이 표시 됩니다.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>특정 언어로 전체 변환 된 사이트 보기
사이트 페이지, 탐색, 웹 파트 등의 특정 언어로 전체 변환 된 사이트를 보려면 해당 언어에 대해 사용자의 개인 언어 및 국가별 설정을 지정 해야 합니다. 언어 및 국가별 설정 설정에 대 한 자세한 내용은 [개인 언어 및 국가별 설정 변경을](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)참조 하십시오. 별도의 계정을 사용 하거나 다른 언어 설정을 사용 하는 다른 사용자에 게 번역 된 페이지를 표시 하는 것이 가장 좋습니다.

## <a name="what-does-a-translator-do"></a>번역기는 어떤 역할을 하나요?
 사이트가 영어로 설정 된 후에는 스페인어를 기본 설정 된 개인 언어로 사용 하는 사용자는 수동으로 제목, 탐색, 바닥글 콘텐츠를 스페인어로 편집 하 고 변환 합니다. 독일어로 표시 되는 사용자는 독일어와 동일한 방식으로 사용 됩니다. 콘텐츠를 번역 하면 해당 기본 언어의 모든 사용자에 대해 표시 됩니다. 웹 파트는 사용자의 기본 설정 언어를 선택 하 고 해당 언어로 번역 된 콘텐츠를 표시 합니다. 

번역자는 기본 언어 페이지의 복사본을 지정 된 언어로 수동으로 번역 합니다. 페이지의 복사본을 만들 때 번역기가 지정 된 경우 번역자에 게 전자 메일을 보냅니다. 이 전자 메일에는 기본 언어 페이지와 새로 만든 번역 페이지에 대 한 링크가 포함 되어 있습니다. 변환기는 다음과 같은 작업을 수행 합니다.
1. 전자 메일에서 **번역 시작** 단추를 선택 합니다.
2. 페이지 오른쪽 위에서 **편집** 을 선택 하 고 콘텐츠를 번역 합니다.
3. 작업이 완료 되 면 **초안으로 저장** (독자에 게 공개할 준비가 되지 않은 경우)을 선택 하 고, 사이트에서 해당 언어를 사용 하는 모든 사용자가 페이지를 볼 준비가 되 면 **게시** 또는 **뉴스 게시**를 선택 합니다.

변환 프로세스에 대 한 자세한 내용은 [다국어 통신 사이트, 페이지 및 뉴스 만들기](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)를 참조 하세요. 

## <a name="updating-the-default-language-page"></a>기본 언어 페이지 업데이트
기본 언어 페이지가 업데이트 되 면 페이지를 다시 게시 해야 합니다. 그러면 번역 페이지의 변환기에 게 업데이트를 적용 하 여 개별 번역 페이지에 대 한 업데이트를 수행할 수 있는 전자 메일 알림이 제공 됩니다.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>다국어 사이트 이름, 탐색 및 바닥글 설정
사이트의 사이트 이름, 탐색 및 바닥글을 사용 가능 하도록 설정한 다른 언어로 표시 하려면 각 언어를 수동으로 번역 해야 합니다.

예를 들어 영어 기본 언어로 커뮤니케이션 사이트를 만들었고 스페인어 및 독일어로 사이트를 사용 하도록 설정 했다고 가정해 보겠습니다. 사이트를 만들 때 기본 언어 (이 경우 영어)에서 사이트 이름 및 설명을 설정 합니다. 사이트를 만든 후에도 사이트 이름 및 설명을 업데이트할 수 있습니다. 그런 다음 영어로 탐색 노드와 바닥글 콘텐츠를 만듭니다.

사이트가 영어로 설정 된 후에는 스페인어를 선호 하는 개인 언어로 사용 하는 사용자는 제목, 설명, 탐색 및 바닥글 내용을 스페인어로 다시 편집 하 고 변환 합니다. 독일어로 표시 되는 사용자는 독일어와 동일한 방식으로 사용 됩니다. 콘텐츠를 번역 하면 해당 기본 언어의 모든 사용자에 대해 표시 됩니다. 

> [! NOTES
>- 원하는 언어의 사이트 콘텐츠를 번역 하는 사용자는 해당 사이트에 대 한 소유자 그룹의 구성원 이거나 사이트 사용 권한이 동일 해야 합니다.
>- 기본 언어로 사이트 이름, 탐색 또는 바닥글이 변경 되는 경우에는 기존 사이트 번역을 덮어쓰도록 선택 하지 않으면 다른 언어에서 해당 하는 번역 된 항목이 자동으로 업데이트 되지 않습니다. 이렇게 하면 번역 된 항목이 기본 언어로 업데이트 된 것으로 바뀌고 다시 수동으로 번역 해야 합니다. 번역을 덮어쓰려면 기본 언어에 대 한 사이트 언어 페이지로 이동 하 여 고급 설정 표시를 선택 합니다. 그런 다음 번역 덮어쓰기에 대해 전환 기능을 설정으로 밉니다. 이 옵션은 페이지 또는 뉴스 콘텐츠에는 적용 되지 않습니다.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>특정 언어로 전체 변환 된 사이트를 보려면
사이트 페이지, 탐색, 웹 파트 등의 특정 언어로 전체 변환 된 사이트를 보려면 해당 언어에 대해 사용자의 개인 언어 및 국가별 설정을 지정 해야 합니다. 언어 및 국가별 설정 설정에 대 한 자세한 내용은 [개인 언어 및 국가별 설정 변경을](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)참조 하십시오. 별도의 계정을 사용 하거나 다른 언어 설정을 사용 하는 다른 사용자에 게 번역 된 페이지를 표시 하는 것이 좋습니다.

## <a name="for-more-information"></a>자세한 내용
- SharePoint communication 사이트 페이지 변환에 대 한 자세한 내용은 [다국어 통신 사이트, 페이지 및 뉴스 만들기](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)를 참조 하세요.
- 학습 경로를 사용자 지정 하는 방법에 대 한 자세한 내용은 [Customize Learning 경로](custom_overview.md)를 참조 하십시오.  
