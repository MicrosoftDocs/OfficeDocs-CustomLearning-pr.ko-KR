---
author: karuanag
ms.author: karuanag
manager: alexb
title: 재생 목록 사용자 지정 및 공유
ms.date: 02/10/2019
description: 기존 콘텐츠 또는 새 SharePoint 페이지에서 사용자 지정 재생 목록 만들기
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000214"
---
# <a name="customize-and-share-playlists"></a>재생 목록 사용자 지정 및 공유

## <a name="create-a-playlist"></a>재생 목록 만들기

재생 목록은 "자산"을 보완하는 것입니다. "자산"은 Microsoft 교육 콘텐츠의 SharePoint 페이지 또는 기존 항목입니다. 재생 목록을 만들 때 함께 이동하여 사용자에 대한 학습 경로를 만드는 자산을 선택합니다.  

SharePoint 페이지를 추가하면 조직에서 호스팅되는 YouTube 비디오 또는 비디오를 사용하여 SharePoint 페이지를 만들 수 있습니다. Forms 또는 기타 Office 365 콘텐츠를 사용하여 페이지를 만들 수도 있습니다.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>1단계: 재생 목록에 대한 SharePoint 페이지 만들기
이 예제에서는 먼저 재생 목록에 추가할 SharePoint 페이지를 만들어 보겠습니다. YouTube 비디오 웹 파트 및 텍스트 웹 파트가 있는 페이지를 만들 것입니다.  이 지침에서는 SharePoint Online 서비스를 사용 중이라 가정합니다. 

#### <a name="create-a-new-page"></a>새 페이지 만들기
1.  새 사이트 페이지 > 사이트 > 콘텐츠 > > 선택합니다.
2.  제목 영역에 Teams 명령 상자를 입력합니다.
3.  새 추가 섹션을 선택한 다음 두 열을 선택합니다.

![두 열 추가](media/clo365addtwocolumn.png)

4.  왼쪽 상자에서 새 웹 파트 추가를 선택한 다음 Embed를 선택합니다. 
5.  웹 브라우저에서 이 URL로 이동하여 비디오에 대한 https://youtu.be/wYrRCRphrp0 코드를 다운로드합니다. 
6.  SharePoint 웹 파트에서 Embed 코드 추가를 선택한 다음 임박 상자에 붙여 넣습니다. 
7.  오른쪽 상자에서 새 웹 파트 추가를 선택한 다음 텍스트를 선택합니다. 
8.  웹 브라우저에서 이 URL로 이동하여 https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 시도해 보세요! 페이지의 지침에 따라 텍스트 웹 파트에 붙여 넣습니다. 페이지는 다음과 같이 표시됩니다. 
![Embed page](media/clo365teamscommandbox.png)
9.  **게시를** 클릭한 다음 페이지의 URL을 복사하여 메모장에 붙여 넣습니다.

#### <a name="step-2-create-the-playlist"></a>2단계: 재생 목록 만들기

1. 사이트 **환경의 사용자 지정 학습 관리** 페이지로 이동합니다.
![사용자 지정 학습 관리 선택 화면.](media/custom_admin.png)
1. 범주가  선택되어 있는지 확인 
1. 새 재생 목록을 표시하려면 범주를 클릭합니다.
1. 범주 이름 옆에 있는 더하기 기호 범주 옵션과 더하기 기호가 강조 표시된 ![ 창을 클릭합니다.](media/custom_addplay.png)

1. 아래 예제와 같이 값을 입력하고 만들기를 **선택합니다.** 
![재생 목록 세부 정보를 입력하는 페이지입니다.](media/custom_details.png)
- **제목** - 재생 목록의 표시 이름
- **Description** - 학습할 내용에 대한 정보
- **범주** - 초기 선택에 따라 미리 선택
- **하위 범주** - 사용자 선택에 따라 미리 선택
- **기술** - 적용 가능한 선택
- **수준** - 초보자, 상호 연결 또는 고급
- **대상** - 이를 통해 Microsoft에서 제공하는 미리 정의된 역할 목록을 기반으로 콘텐츠를 대상으로 할 수 있습니다.

6. 자세히 **저장을 클릭합니다.**

> [!TIP]
> 재생 목록의 아이콘 이미지를 사용자 지정할 수 있습니다.  이미지 아이콘을 클릭하고 이전에 업로드한 이미지의 URL을 삽입합니다.  이미지가 사용자 지정 학습 사이트 모음 또는 모든 사용자가 파일에 액세스할 수 있는 다른 위치에 있는지 확인  
![이미지 창을 선택합니다.](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>3단계: 재생 목록에 자산 추가
이 단계에서는 Microsoft의 기존 자산과 만든 SharePoint 페이지를 재생 목록에 추가합니다. 

1. 재생 목록에 대한 세부 정보를 저장한 후 기존 자산 검색을 사용할 수 있습니다.
1. **검색 용어에** 입력하여 다른 재생 목록에서 사용할 수 있는 미리 정의한 자산 목록을 볼 수 있습니다. **자산의 이름을** 클릭하여 새 재생 목록에 포함합니다.<br/>
![재생 목록 자산 페이지](media/custom_slist.png)

앞에서 만든 SharePoint 페이지를 추가하거나 환경의 처음부터 만들 수도 있습니다.

1. 재생 목록 **자산 대화 상자에서** 새 자산 옵션을 클릭합니다.
1. 자산에 제목을 **제공 합니다.** 입력하면 추가 옵션이 표시됩니다.
![제목 및 추가 세부 정보를 입력하는 양식입니다.](media/custom_newpage.png)
1. 이제 SharePoint Online에서 새 자산 페이지를 만들거나 기존 페이지의 URL을 입력하여 사용자 지정 재생 목록에 추가할 수 있습니다. 
1. **범주,** 하위  **범주** 및 기술 필드는 이 재생 목록의 이전 선택에 따라 미리 채워지게 됩니다.
1. 이 개별 자산에 대한 Level 및 Audience에 대해 적절한 선택을 합니다.  
1. 자산 **저장을 클릭하여** 사용자 지정 재생 목록에 추가
1. 재생 목록이 완료될 때까지 개별 페이지를 검색하거나 추가하는 단계를 반복합니다. 
1. 재생 **목록 닫기 를 클릭하여** 저장

이 콘텐츠가 포함된 재생 목록은 이제 사용자 지정 학습 웹 사이트를 설치/포함한 모든 곳에서 사용할 수 있습니다. 

> [!NOTE]
> 재생 목록을 닫은 후 실수를 한 경우 재생 목록 이름 옆에 있는 X를 클릭하여 범주에서 삭제할 수 있습니다.  

#### <a name="things-to-think-about"></a>생각할 것

사용자 지정 재생 목록을 사용하여 최종 사용자가 다양한 작업을 수행할 수 있습니다.  시간제 요청 양식이 있나요?  하드웨어 장비를 요청하는 양식인가요?  기존 교육 자산을 경험에 프로그래밍할 수 있습니다.  

## <a name="share-playlists"></a>재생 목록 공유

1. 웹파트 또는 사이트 환경 내의 재생 목록으로 이동
1. 왼쪽 위 모서리에 세 개의 아이콘이 표시됩니다.
1. 링크를 나타내는 아이콘 클릭
1. URL 옆에 있는 복사를 클릭하는 재생 목록 화면에 ![ URL을 복사합니다.](media/share.png)
이제 이 URL을 사이트 탐색에 삽입하거나 다른 통신에 활용하여 직원을 해당 재생 목록으로 바로 이동하는 데 사용할 수 있습니다. 

### <a name="next-steps---drive-adoption"></a>다음 단계 - [채택 주도](driveadoption.md)
