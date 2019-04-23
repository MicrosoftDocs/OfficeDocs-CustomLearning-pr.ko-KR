---
author: karuanag
ms.author: karuanag
title: 재생 목록 사용자 지정 및 공유
ms.date: 02/10/2019
description: 기존 콘텐츠 또는 새 SharePoint 페이지에서 사용자 지정 재생 목록 만들기
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056428"
---
# <a name="customize-and-share-playlists"></a>재생 목록 사용자 지정 및 공유

## <a name="create-a-playlist"></a>재생 목록 만들기

재생 목록은 "자산"의 compliation. "자산"은 SharePoint 페이지 또는 Microsoft 교육 콘텐츠의 기존 항목입니다. 재생 목록을 만들 때 함께 이동 하는 자산을 선택 하 여 사용자에 대 한 학습 경로를 만듭니다.  

sharepoint 페이지를 추가할 때의 이점은 조직에서 호스트 되는 YouTube 비디오 또는 비디오를 사용 하 여 sharepoint 페이지를 만들 수 있다는 것입니다. 양식 또는 기타 Office 365 콘텐츠가 포함 된 페이지를 만들 수도 있습니다.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>1 단계: 재생 목록에 대 한 SharePoint 페이지 만들기
이 예제에서는 먼저 재생 목록에 추가할 SharePoint 페이지를 만듭니다. YouTube 비디오 웹 파트 및 텍스트 웹 파트가 포함 된 페이지를 만듭니다.  이 지침에서는 SharePoint Online 서비스를 사용 하 고 있다고 가정 합니다. 

#### <a name="create-a-new-page"></a>새 페이지 만들기
1.  설정 메뉴 > 사이트 콘텐츠 > 사이트 페이지 > 새 > Site 페이지를 선택 합니다.
2.  제목 영역에 팀 명령 사용 상자를 입력 합니다.
3.  새 섹션 추가를 선택 하 고 두 개의 열을 선택 합니다.

![2 열 추가](media/clo365addtwocolumn.png)

4.  왼쪽 상자에서 새 웹 파트 추가를 선택 하 고 포함을 선택 합니다. 
5.  웹 브라우저에서이 URL https://youtu.be/wYrRCRphrp0 로 이동 하 여 비디오에 대 한 embed 태그를 가져옵니다. 
6.  SharePoint 웹 파트에서 embed 태그 추가를 선택 하 여 포함 상자에 붙여 넣습니다. 
7.  오른쪽 상자에서 새 웹 파트 추가를 선택한 다음 텍스트를 선택 합니다. 
8.  웹 브라우저에서 다음 https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b URL로 이동 하 여 Try! 지침을 선택한 다음 텍스트 웹 파트에 붙여 넣습니다. 페이지 모양은 다음과 같습니다. 

![페이지 포함](media/clo365teamscommandbox.png)

9.  **게시**를 클릭 한 다음 페이지의 URL을 복사 하 여 메모장에 붙여넣기

#### <a name="step-2-create-the-playlist"></a>2 단계: 재생 목록 만들기

1. 사이트 환경에서 **사용자 지정 학습 관리** 페이지로 이동 합니다.
![custom_admin-.png](media/custom_admin.png)
1. **범주가** 선택 되어 있는지 확인 
1. 새 재생 목록을 표시할 범주를 클릭 합니다.
1. 범주 이름 옆에 있는 더하기 기호 ![(custom_addplay)를 클릭 합니다.](media/custom_addplay.png)

1. 아래 예제와 같이 값을 입력 하 고 **만들기**를 선택 합니다. 
![custom_details-.png](media/custom_details.png)
- **제목** -재생 목록의 표시 이름입니다.
- **Description** -배우게 되는 사항에 대 한 정보입니다.
- **범주** -초기 선택을 기준으로 미리 선택 됩니다.
- **하위 범주** -초기 선택을 기준으로 미리 선택
- **기술** -해당 되는 경우 선택
- **만추** -초급, intermidate 또는 Advanced
- **대상 그룹** -Microsoft에서 제공 하는 미리 정의 된 역할 목록을 기반으로 콘텐츠를 대상으로 지정할 수 있습니다.

6. **세부 정보 저장** 을 클릭 합니다.

> [!TIP]
> 재생 목록의 아이콘 이미지를 사용자 지정할 수 있습니다.  이미지 아이콘을 클릭 하 고 이전에 업로드 한 이미지의 URL을 삽입 합니다.  이미지가 사용자 지정 학습 사이트 모음에 위치 하거나 모든 사용자가 해당 파일에 액세스할 수 있는 다른 위치에 있는지 확인 합니다.  
![custom_image-.png](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>3 단계: 재생 목록에 에셋 추가
이 단계에서는 Microsoft 및 만든 SharePoint 페이지의 기존 자산을 재생 목록에 추가 합니다. 

1. 재생 목록에 대 한 세부 정보를 저장 한 후에는 기존 자산 검색을 사용할 수 있습니다.
1. **검색 용어를 입력** 하 여 다른 재생 목록에서 사용할 수 있는 미리 정의 된 자산의 목록을 확인 합니다. 자산 **이름을 클릭** 하 여 새 재생 목록에 포함 합니다.
![custom_slist-.png](media/custom_slist.png)

이전에 만든 SharePoint 페이지를 추가 하거나 환경에서 처음부터 새로 만들 수도 있습니다.

1. 재생 목록 자산 대화 상자에서 **새 자산** 옵션을 클릭 합니다.
1. 자산에 **제목을**지정 합니다. 입력 된 추가 옵션에는 custom_newpage ![가 표시 됩니다.](media/custom_newpage.png)
1. 이제 SharePoint Online에서 새 자산 페이지를 만들거나 기존 페이지의 URL을 입력 하 여 사용자 지정 재생 목록에 추가할 수 있습니다. 
1. **범주**, **하위 범주** 및 **기술** 필드는이 재생 목록에 대 한 이전 선택 항목에 따라 미리 채워집니다.
1. 이 개별 자산의 수준 및 대상 그룹을 적절 하 게 선택 합니다.  
1. **자산 저장** 을 클릭 하 여 사용자 지정 재생 목록에 추가 합니다.
1. 재생 목록이 완료 될 때까지 개별 페이지를 검색 하거나 추가 하 여이 단계를 반복 합니다. 
1. **재생 목록 닫기** 를 클릭 하 여 저장

이 콘텐츠를 포함 하는 재생 목록은 사용자 지정 학습 웹 파트를 설치/포함 한 모든 위치에서 사용할 수 있게 됩니다. 

> [!NOTE]
> 재생 목록을 닫은 후 실수를 한 경우 재생 목록 이름 옆에 있는 X를 클릭 하 여 범주에서 삭제할 수 있습니다.  

#### <a name="things-to-think-about"></a>고려해 야 할 사항

사용자 지정 재생 목록을 사용 하 여 최종 사용자가 다양 한 작업을 지원할 수 있습니다.  휴가 요청 양식이 있습니까?  하드웨어 장비를 요청 하는 양식  모든 기존 교육 자산이 환경에 프로그래밍 될 수 있습니다.  

## <a name="share-playlists"></a>재생 목록 공유

1. 웹 파트 또는 사이트 환경 내의 재생 목록으로 이동
1. 왼쪽 위 모서리에 세 개의 아이콘이 표시 됩니다.
1. 링크를 나타내는 아이콘을 클릭 합니다.
1. 재생 목록에 URL 복사

![.png](media/share.png) 이 URL은 이제 사이트 탐색에 삽입 하거나 다른 통신에서 사용 하 여 직원을 해당 재생 목록으로 바로 이동할 수 있습니다. 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a>다음 단계- [드라이브 도입](driveadoption.md)
