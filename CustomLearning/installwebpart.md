---
author: karuanag
ms.author: karuanag
title: 사용자 지정 학습 솔루션 웹 파트 설치
ms.date: 02/10/2019
description: 사용자 지정 학습 솔루션 웹 파트에 대 한 설치 지침
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989689"
---
# <a name="installing-the-custom-learning-solution-webpart"></a>사용자 지정 학습 솔루션 웹 파트 설치

## <a name="prerequisites-for-a-tenant-wide-installation"></a>테 넌 트 전체 설치를 위한 필수 구성 요소

- 전체 테 넌 트에 대 한 사용자 지정 학습 웹 파트를 설치 하려면 Office 365 관리 권한이 있어야 합니다.  이러한 사용 권한이 없는 경우 Office 365 관리자에 게 작업 하거나 개별 사이트 모음에 대 한 웹 파트를 설치할 수 있습니다.
- 사용자 또는 Office 365 관리자에 게 설치 및 구성 된 테 넌 트 전체 [앱 카탈로그](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) 또는 웹 파트를 수신 하는 [사이트 모음 앱 카탈로그](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)를 설정 해야 합니다.]
- SharePoint Online만 지원 됩니다. 웹 파트는 온-프레미스 버전의 SharePoint에 설치 하는 것을 지원 하지 않습니다.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>테 넌 트에 사용자 지정 학습 웹 파트 추가 

1. 사용자 지정 학습 웹 파트를 다운로드 하 여 로컬 드라이브에 저장 합니다.  이 파일의 이름은 "helloworld-webpart.sppkg"입니다.  파일의 이름이 나 접미사를 변경 하지 마십시오. 
2. 테 넌 트에 대 한 [Office 365 관리 포털로](https://admin.microsoft.com/AdminPortal/Home#/homepage) 이동 합니다.
3. 왼쪽 탐색 창에서 관리 센터, SharePoint를 선택 합니다. 이 페이지는 새 탭에서 열립니다., sharepoint 관리 센터에서 앱, 앱 카탈로그, sharepoint 용 앱을 선택 합니다. 
4. 웹 파트 업로드를 선택 하 고 사용자가 다운로드 한 "helloworld-webpart.sppkg" 파일을 선택 합니다.
5. 이 테 넌 트 전체 설치의 경우 "이 솔루션을 조직의 모든 위치에서 사용할 수 있도록 설정" 옆의 상자를 선택 합니다.  
 
> [!NOTE]
> webpart를 설치한 후에는 SharePoint Online의 웹 파트 갤러리에 해당 웹 파트를 찾을 수 있습니다.  **웹 파트의 이름은 "Microsoft Learning"입니다** .

![솔루션 배포](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a>SharePoint Online 페이지에 Microsoft Learning 웹 파트 추가

사용자 지정 학습을 테 넌 트에서 설치한 후 SharePoint 페이지에 웹 파트를 추가할 수 있습니다. Office 365 및 사이트에서 Windows 10 학습을 사용할 수 있습니다.

1. 전체 너비 열 레이아웃에 사용자 지정 학습 웹 파트를 추가 합니다.

![SharePoint 페이지 레이아웃](media/clo365fullcolumnwidth.png)

2. SharePoint 페이지에서 섹션 추가를 선택한 다음 전체 너비 열을 선택 합니다.  다음과 같은 메시지가 표시 됩니다.

![addwebpart](media/clo365addfullwidthwebpart.png)

3. Microsoft Learning을 선택 합니다.  그러면 다음이 표시 됩니다. 

![사용자 지정 학습 웹 파트](media/clo365addwebpart.png)

 이제 타일을 클릭 하 여 솔루션에 포함 된 기본 콘텐츠를 탐색할 수 있습니다.  

### <a name="next-steps"></a>다음 단계
- 웹 파트에 포함 된 [기본 콘텐츠](webpartcontent.md) 를 살펴봅니다.
- 조직의 교육 환경 [사용자 지정](customization.md)
- 교육 솔루션 [도입을 추진](driveadoption.md) 합니다.

