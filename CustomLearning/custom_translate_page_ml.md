---
author: pkrebs
ms.author: pkrebs
title: 사이트 페이지 번역
ms.date: 07/06/2020
description: 사이트 페이지 번역
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: baa46deda7d7e10f3a7655fc6da076d37607e29f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000294"
---
# <a name="translate-site-pages"></a>사이트 페이지 번역
학습 경로 사이트 번역을 시작하기 전에 다국어 기능이 학습 경로에서 작동하는 방식에 대한 몇 가지 주요 개념을 이해하는 것이 중요합니다. 
- 사이트 정보 - 탐색, 로고 및 사이트 이름 번역을 사용하려면 사용자의 언어 프로필에서 사이트를 보고 번역해야 합니다.  
- 학습 경로 웹 파트가 영어가 아닌 언어로 표시하려면 사용자의 언어 프로필을 사용하여 웹 파트를 보아야 합니다. 웹 파트 및 Microsoft 제공 콘텐츠가 이미 번역되어 있습니다. 언어 프로필에 대한 자세한 내용은 개인 언어 및 국가별 설정 [변경을 참조하세요.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)
- 학습 경로를 설정하는 방식에 따라 번역된 페이지를 사용할 수 있는지 여부가 결정됩니다. Microsoft 365 룩북 서비스를 통해 프로비전된 새 사이트에는 9개 언어로 번역된 페이지가 제공됩니다. 만든 사이트 또는 사이트가 업데이트된 경우 수동으로 번역해야 합니다. [다국어 학습 경로에 대한 설정 옵션을 참조하세요.](custom_setupoptions_ml.md)
- 커뮤니케이션 사이트에 대한 SharePoint Online 다국어 기능을 통해 학습 경로에 대한 다국어 지원을 사용할 수 있습니다. SharePoint Online 다국어 기능에 대한 자세한 내용은 다국어 통신 사이트, 페이지 및 뉴스 [만들기를 참조하세요.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c) 

## <a name="working-with-a-newly-provisioned-site"></a>새로 프로비전된 사이트 작업
Microsoft 365 룩북 서비스에서 새 학습 경로 사이트를 프로비전한 경우 번역된 페이지를 이미 사용할 수 있습니다. 기본적으로 사이트에서 제공하는 페이지는 다음과 같습니다.

- Home.aspx
- Start-with-Six-Simple-Steps.aspx
- Get-started-with-Microsoft-365.aspx
- Get-started-with-Microsoft-Teams.aspx
- Get-started-with-SharePoint.aspx
- Get-started-with-OneDriive.aspx
- Ask-questions-and-get-help.aspx
- 교육 이벤트 calendar.aspx
- Become-a-Champion.aspx
- Recommended-Playlists.aspx
- 학습 경로 관리 성공 센터

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>새로 프로비전된 사이트에서 번역된 페이지 보기
번역된 학습 경로 사이트에 익숙해지기 위해 몇 가지 번역된 페이지를 살펴보자.

### <a name="view-the-translated-home-page"></a>번역된 홈 페이지 보기
학습 경로 홈 페이지에서 다음 예제와 같이 언어 드롭다운에서 언어를 선택합니다. 이 예제에서는 오른쪽 위 모서리에 이탈리아어가 선택되어 있으며 모든 페이지 요소가 변환됩니다.

![사진 학습 경로의 수](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>번역된 Microsoft 365 교육 페이지 보기
이제 Microsoft 365 교육 페이지를 살펴보십시오. 

1. 학습 경로 사이트 **홈 페이지에서** **Microsoft 365 교육 을 클릭합니다.**
2. 페이지의 오른쪽 위 모서리에서 언어를 선택합니다. 이 예제에서는 이탈리아어가 선택되어 있습니다.

![이탈리아어 샘플 학습 경로 페이지](media/custom_ml_pages_training.png)

언어를 선택하면 표시되는 번역은 무엇입니까?
- SharePoint 페이지는 위의 그래픽에 표시된 대로 변환됩니다. 페이지 배너의 텍스트가 이제 이탈리아어로 표시됩니다.

What's translations aren'tvisible?
- 사이트 이름이 영어로 제공됩니다.
- 사이트 탐색이 영어로 제공됩니다.
- 학습 경로 웹 파트가 영어로 제공됩니다.

## <a name="view-the-fully-translated-site"></a>완전히 번역된 사이트 보기 
사이트 페이지, 탐색 및 웹 파트를 비롯한 특정 언어로 완전히 번역된 사이트를 표시하려면 해당 언어에 대해 사용자의 개인 언어 및 국가별 설정을 지정해야 합니다. 언어 및 국가별 설정에 대한 자세한 내용은 개인 언어 및 국가별 설정 [변경을 참조하세요.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) 별도의 계정을 사용하거나 다른 언어 설정이 있는 다른 사용자가 번역된 페이지를 보게 하는 것이 좋습니다.  

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>업데이트되거나 수동으로 설치된 학습 경로 사이트 작업
기존 학습 경로 사이트를 업데이트하거나 웹 파트를 기존 사이트에 수동으로 설치한 경우 사이트 페이지를 수동으로 번역해야 합니다. 학습 경로 웹 파트 및 콘텐츠가 이미 번역되어 사용자의 기본 설정 언어로 표시됩니다. 페이지를 번역하려는 경우 다음 지침 "원하는 언어에 대한 페이지 만들기"를 참조하세요. 

## <a name="create-pages-for-the-languages-you-want"></a>원하는 언어에 대한 페이지 만들기
사이트를 다국어 기능을 사용하도록 설정하고 사용할 수 있도록 할 언어를 선택한 후 원하는 번역 페이지를 만들 수 있습니다. 

1. 다른 언어로 사용할 수 있도록 할 기본 언어 페이지로 이동합니다.
2. 위쪽 표시줄에서 번역 을 **선택합니다.**
3. 원하는 **언어에** 대해 만들기를 선택합니다.

> [!IMPORTANT]
> 번역 페이지를 만든 후 다음을 보장하기 위해 기본 언어 페이지를 게시(또는 다시 게시)해야 합니다.
>- 번역 페이지는 해당 언어 사이트에 표시됩니다.
>- 번역 페이지가 뉴스 웹 파트 및 강조 표시된 콘텐츠 웹 파트에 올바르게 표시됩니다.
>- 사이트 맨 위에 있는 언어 드롭다운에는 사용하도록 설정한 모든 언어가 포함됩니다.
>- 번역자는 번역 요청을 통보합니다.

페이지를 만든 후 페이지 상태(초안 저장, 게시 등)가 각 언어 옆에 있는 번역 창에 표시됩니다. 또한 할당한 번역자는 번역이 요청된 전자 메일로 통보됩니다.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>특정 언어로 완전히 번역된 사이트 보기
사이트 페이지, 탐색 및 웹 파트를 비롯한 특정 언어로 완전히 번역된 사이트를 표시하려면 해당 언어에 대해 사용자의 개인 언어 및 국가별 설정을 지정해야 합니다. 언어 및 국가별 설정에 대한 자세한 내용은 개인 언어 및 국가별 설정 [변경을 참조하세요.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) 별도의 계정을 사용하거나 다른 언어 설정이 있는 다른 사용자가 번역된 페이지를 보게 하는 것이 좋습니다.

## <a name="what-does-a-translator-do"></a>번역기는 어떤 역할을 하나요?
 사이트를 영어로 설정한 후 스페인어를 원하는 개인 언어로 사용하는 사용자는 제목, 탐색 및 발자국 콘텐츠를 수동으로 편집하고 스페인어로 번역합니다. 독일어를 기본 설정 개인 언어로 사용하는 사용자는 독일어로 동일하게 작업을 수행합니다. 콘텐츠가 번역되면 해당 기본 설정 언어를 사용하는 모든 사용자에게 콘텐츠가 표시됩니다. 웹 파트는 사용자의 기본 설정 언어를 선택하고 해당 언어로 번역된 콘텐츠를 보여줍니다. 

번역자는 기본 언어 페이지의 복사본을 지정된 언어로 수동으로 번역합니다. 페이지 복사본이 만들어지면 번역가 지정되면 번역자는 전자 메일로 알림을 하게 됩니다. 전자 메일에는 기본 언어 페이지와 새로 만든 번역 페이지에 대한 링크가 포함되어 있습니다. 번역자는 다음을 합니다.
1. 전자 **메일에서** 번역 시작 단추를 선택합니다.
2. 페이지 **오른쪽** 상단에서 편집을 선택하고 콘텐츠를 번역합니다.
3. 완료되면 초안으로 저장(독자에게 표시될 준비가 되지 않은 경우)을 선택하거나 사이트에서 해당 언어를 사용하는 모든 사용자가 페이지를 볼 준비가  된 경우 게시 또는 뉴스 게시를 **선택합니다.** 

번역 프로세스에 대한 자세한 내용은 다국어 통신 사이트, 페이지 및 뉴스 만들기를 [참조하세요.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c) 

## <a name="updating-the-default-language-page"></a>기본 언어 페이지 업데이트
기본 언어 페이지가 업데이트될 때 페이지를 다시 게시해야 합니다. 그런 다음 번역 페이지의 번역자는 개별 번역 페이지를 업데이트할 수 있도록 업데이트가 이행된 것으로 전자 메일에 통보됩니다.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>다국어 사이트 이름, 탐색 및 발자국 설정
사용 가능한 다른 언어로 사이트의 사이트 이름, 탐색 및 바닥글을 표시하려면 각 언어를 직접 번역해야 합니다.

예를 들어 영어를 기본 언어로 사용하여 커뮤니케이션 사이트를 만든 후 해당 사이트에 스페인어 및 독일어를 사용하도록 설정했다고 가정해 보겠습니다. 사이트를 만들 때 기본 언어(이 경우에는 영어)로 사이트 이름 및 설명을 설정합니다. 사이트를 만든 후에도 사이트 이름 및 설명을 업데이트할 수 있습니다. 그 다음 영어로 탐색 노드와 바닥글 콘텐츠를 만들 수 있습니다.

사이트를 영어로 설정한 후 스페인어를 기본 설정 개인 언어로 사용하는 사용자는 직접 제목, 설명, 탐색 및 바닥글 콘텐츠를 스페인어로 편집하고 번역합니다. 독일어를 기본 설정 개인 언어로 사용하는 사용자는 독일어로 동일하게 작업을 수행합니다. 콘텐츠가 번역되면 해당 기본 설정 언어를 사용하는 모든 사용자에게 콘텐츠가 표시됩니다. 

> [! NOTES]
>- 원하는 언어로 사이트 콘텐츠를 번역하는 사용자는 해당 사이트의 Owners 그룹의 구성원이거나 동일한 사이트 권한이 있는 사용자입니다.
>- 사이트 이름, 탐색 또는 발자국어를 기본 언어로 변경하면 기존 사이트 번역을 덮어들이지 않는 한 다른 언어로 번역된 해당 항목이 자동으로 업데이트되지 않습니다. 이렇게 하는 경우 번역된 항목이 기본 언어의 업데이트로 대체되어 수동으로 다시 번역해야 합니다. 번역을 덮어 사용하려면 기본 언어의 사이트 언어 페이지로 이동한 다음 고급 설정 표시를 선택합니다. 그런 다음 번역 덮어 사용에 대한 토글을 으로 으로 끄습니다. 이 옵션은 페이지 또는 뉴스 콘텐츠에는 적용되지 않습니다.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>완전히 번역된 사이트를 특정 언어로 보기
사이트 페이지, 탐색 및 웹 파트를 비롯한 특정 언어로 완전히 번역된 사이트를 표시하려면 해당 언어에 대해 사용자의 개인 언어 및 국가별 설정을 지정해야 합니다. 언어 및 국가별 설정에 대한 자세한 내용은 개인 언어 및 국가별 설정 [변경을 참조하세요.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) 별도의 계정을 사용하거나 다른 언어 설정이 있는 다른 사용자가 번역된 페이지를 보게 하는 것이 좋습니다.

## <a name="for-more-information"></a>자세한 내용
- SharePoint 커뮤니케이션 사이트 페이지 번역에 대한 자세한 내용은 다국어 통신 사이트, 페이지 및 뉴스 [만들기를 참조하세요.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)
- 학습 경로를 사용자 지정하는 데 대한 자세한 내용은 사용자 지정 [학습 경로 를 참조하세요.](custom_overview.md)  
