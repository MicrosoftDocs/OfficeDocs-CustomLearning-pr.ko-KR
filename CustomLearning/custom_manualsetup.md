---
author: pkrebs
ms.author: pkrebs
title: 학습 경로 수동 설정
ms.date: 07/06/2020
description: Microsoft 365 학습 경로 수동 설정
ms.openlocfilehash: f980722fed48b5f92fb595cf8286604b3fa6d409
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043270"
---
# <a name="learning-pathways-manual-setup"></a>학습 경로 수동 설정

Microsoft 365 학습 경로는 다음 시나리오 중 하나를 지원 해야 하는 조직에 대 한 수동 설치를 제공 합니다. 

- 조직에 교육 전용의 설정 된 SharePoint Online 최신 통신 사이트가 있으며, 해당 사이트에 대해 학습 경로를 추가 하려는 경우 이 시나리오에서는 학습 경로 웹 파트가 사이트에 설정 되지 않았습니다.

- 조직의 SharePoint 통신 사이트 중 하나에서 다국어 지원에 대 한 학습 경로를 설치 하려고 합니다. 이 사이트는 영어가 아닌 기본 언어로 제공 되거나 학습 경로에서 지원 되는 언어 중 하나입니다. 다음은 학습 경로에서 지 원하는 언어입니다.

- English
- 중국어(간체)
- 프랑스어
- 독일어
- 이탈리아어(이탈리아)
- 일본어 (일본)
- 포르투갈어 (브라질)
- 러시아어 (러시아어)
- Spanish

학습 경로를 수동으로 설정 하려면 Windows PowerShell 및 SharePoint Online 관리 셸을 사용 하는 경험이 필요 합니다. 다음은 학습 경로의 수동 설정 단계에 대 한 개요입니다. 

- 모든 필수 구성 요소를 충족 했는지 확인 합니다.
- 사이트에 대 한 기본 언어 설정을 확인 합니다. 확인 되 면 수동 설치를 계속 합니다. 다른 기본 언어 설정이 필요한 경우에는 새 사이트를 만들어야 합니다. 
- SharePoint 테 넌 트 앱 카탈로그에 customlearning 파일을 설치 합니다.
- Microsoft 365 학습 경로 홈 사이트로 작동할 최신 커뮤니케이션 사이트를 프로 비전/식별 합니다.
- 경로 학습 경로가 종속 된 아티팩트를 사용 하 여 테 넌 트를 구성 하는 PowerShell 스크립트를 실행 합니다.
- CustomLearningAdmin 사이트 페이지로 이동 하 여 사용자 지정 콘텐츠 구성을 초기화 하기 위해 관리 웹 파트를 로드 합니다.

## <a name="prerequisites"></a>필수 구성 요소
학습용 경로 웹 파트를 수동으로 설치 하려면 다음 필수 구성 요소를 충족 해야 합니다. 

- 테 넌 트 전체 앱 카탈로그를 설정 하 고 구성 해야 합니다. [Office 365 테 넌 트 설정을](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 참조 하 고 "앱 카탈로그 만들기" 사이트 섹션을 따르세요. 
- 테 넌 트 전체 앱 카탈로그가 이미 프로 비전 된 경우 패키지를 업로드 하는 데 사용할 수 있는 권한이 있는 계정에 대 한 액세스가 필요 합니다. 일반적으로이 계정에는 SharePoint 관리자 역할이 있습니다. 
- 해당 역할이 있는 계정이 작동 하지 않으면 SharePoint 관리 센터로 이동 하 여 앱 카탈로그 사이트 모음에 대 한 사이트 모음 관리자를 찾고, 사이트 모음 관리자 중 한 명으로 로그인 하거나, 사이트 모음 관리자에 게 실패 한 SharePoint 관리자 계정을 추가 합니다. 
- 또한 SharePoint 테 넌 트 관리자 인 계정에도 액세스 해야 합니다.

## <a name="step-1---check-your-language-settings"></a>1 단계-언어 설정 확인
수동 설치 프로세스의 첫 단계에서 사이트 언어 설정을 확인 합니다. 사용할 수 있는 옵션은 다음과 같습니다.

### <a name="option-1---you-dont-want-multilingual-support"></a>옵션 1-다국어 지원 안 함
사이트에 대 한 다국어 지원을 사용 하지 않으려면 설정이 해제 되어 있는지 확인 합니다.
1.  SharePoint **communication 사이트에서**  >  **사이트 정보**  >  **보기 모든 사이트 설정**  >  **언어 설정을**선택 합니다. 
2.  **페이지 및 뉴스를 여러 언어로 번역 하도록 사용** **을 설정 합니다.**
3.  **저장**을 클릭합니다. 
4.  2 단계를 계속 진행 합니다.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>옵션 2-다국어 지원을 사용 하며 기본 언어로 확인
SharePoint communication site에는 기본 언어가 있습니다. 기본 언어는 학습 경로 관리 페이지를 포함 하 여 학습 경로를 보는 데 사용할 언어를 결정 합니다. 기본 언어 설정은 사이트를 처음 만들 때 설정 되며 나중에 변경할 수 없습니다. 수동 설치를 Continueing 전에 먼저 대상 사이트의 기본 언어를 사용 하는 것이 올바른지 확인 합니다.

1.  SharePoint **communication 사이트에서**  >  **사이트 정보**  >  **보기 모든 사이트 설정**  >  **언어 설정을**선택 합니다. 
2.  **페이지 및 뉴스를 여러 언어로 번역할 수 있도록** 설정 합니다를 **켜기**로 전환 합니다.
    - **언어**의 목록 맨 위에 표시 되는 언어를 확인 하는 경우에는 다른 언어를 추가한 다음 **저장**을 클릭할 수 있습니다. 2 단계를 계속 진행 합니다.
    - 사이트에 대해 선택한 것과 다른 기본 언어를 사용 하려면 원하는 언어로 새 SharePoint Communication 사이트를 만들어야 합니다. 옵션 3으로 이동 합니다. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>옵션 #3-다국어 지원을 사용 하지만 사이트에 대해 다른 기본 언어를 사용 하려고 합니다.
이 옵션을 사용 하면 기본 언어를 사용 하 여 SharePoint Online 통신 사이트를 새로 만든 다음 사이트에 대 한 언어 설정을 지정할 수 있습니다. 
1.  새 SharePoint communication site를 만들려면 [Sharepoint Online에서 커뮤니케이션 사이트 만들기](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)를 참조 하세요. 사이트를 만들 때이 언어를 학습용 경로에 사용할 기본 언어로 설정 해야 합니다. 
2. 만든 사이트에서 **설정**  >  **사이트 정보**  >  **보기 모든 사이트 설정**  >  **언어 설정을**선택 합니다. 
2.  **페이지 및 뉴스를 여러 언어로 번역할 수 있도록** 설정 합니다를 **켜기**로 전환 합니다.
3. 필요한 경우 다른 언어를 추가 하 고 **저장**을 클릭 합니다. 
4. 2 단계를 계속 진행 합니다. 

>! 참고 사이트에서 새로 만든 사이트로 사용자 지정 콘텐츠를 마이그레이션해야 하는 경우이 문서의 뒷부분에 나오는 "사용자 지정 콘텐츠 마이그레이션" 섹션을 참조 하십시오. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>2 단계-GitHub에서 웹 파트 패키지 및 설치 스크립트 가져오기
설치 프로세스의 일부로 Microsoft 365 learning 경로 웹 파트 패키지 및 PowerShell 설치 스크립트가 필요 합니다.

- [학습 경로 GitHub 리포지토리로](https://github.com/pnp/custom-learning-office-365)이동 합니다.
- **다운로드** 를 클릭 하 여 웹 파트 패키지와 스크립트를 로컬 드라이브에 저장 합니다. 이 프로세스의 이후 단계에서 스크립트 및 웹 파트 패키지를 사용 하 게 됩니다.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>2 단계-테 넌 트 앱 카탈로그에 웹 파트 업로드
Microsoft 365 학습 경로를 설정 하려면 helloworld-webpart.sppkg 파일을 테 넌 트 전체 앱 카탈로그에 업로드 하 고 배포 합니다. 앱 카탈로그에 앱을 추가 하는 방법에 대 한 자세한 내용은 [앱 카탈로그를 사용 하 여 SharePoint Online 환경에서 사용할 수 있는 사용자 지정 비즈니스 앱 만들기를](https://docs.microsoft.com/sharepoint/use-app-catalog) 참조 하세요.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>3 단계-최신 커뮤니케이션 사이트 프로 비전/식별
기존 SharePoint communication site를 식별 하거나 SharePoint Online 테 넌 트에서 새 사이트를 프로 비전 합니다. 통신 사이트를 구축 하는 방법에 대 한 자세한 내용은 [SharePoint Online에서 커뮤니케이션 사이트 만들기](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 및 단계에 따라 통신 사이트 만들기를 참조 하세요.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>4 단계-Microsoft 365 학습 경로 앱을 사이트에 추가

1. SharePoint 사이트에서 시스템 메뉴를 클릭 한 다음 **앱 추가**를 클릭 합니다. 
2. **앱**아래에서 **조직에서**를 클릭 한 다음 **Office 365에 대 한 학습 경로**를 클릭 합니다. 

## <a name="step-5---set-permissions-for-the-site"></a>5 단계-사이트에 대 한 사용 권한 설정
사이트에 대해 다음 권한이 설정 되어 있는지 확인 합니다.
- **사이트 모음 관리자 또는 소유자 그룹의 일부** -처음 사용을 위해 학습 경로를 설정 하는 customconfig 목록 항목을 초기화 하는 데 필요한 권한입니다. 
- **Members group** -콘텐츠 숨기기 및 표시, 사용자 지정 재생 목록 관리 등 학습 경로를 관리 하는 데 필요한 사용 권한
- **방문자 그룹** -사이트 콘텐츠를 보는 데 필요한 사용 권한 

## <a name="step-6--execute-powershell-configuration-script"></a>6 단계-PowerShell 구성 스크립트 실행
`CustomLearningConfiguration.ps1`솔루션에서 사용 하는 세 개의 [테 넌 트 속성](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties) 을 만들기 위해 실행 해야 하는 PowerShell 스크립트가 포함 됩니다. 또한이 스크립트는 사이트 페이지 라이브러리에 두 개의 [단일 파트 앱 페이지](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages) 를 만들어 관리자 및 사용자 웹 파트를 알려진 위치에 호스트 합니다.

1. SharePoint Online 관리 셸을 아직 다운로드 하지 않은 경우 지금 다운로드 하세요. [SharePoint Online 관리 셸 다운로드](https://go.microsoft.com/fwlink/p/?LinkId=255251)를 참조 하세요.
2. 스크립트를 실행 하려면 PowerShell 실행 정책을 설정 해야 할 수 있습니다. 자세한 내용은 [실행 정책 정보](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)를 참조 하세요.
3. 스크립트를 실행 `CustomLearningConfiguration.ps1` 합니다. 테 넌 트 관리자 자격 증명 외에도 스크립트는 테 넌 트 이름과 사이트 이름을 입력 하 라는 메시지를 표시 합니다. 사이트 URL에 대해 다음 예제를 고려할 때 `https://contoso.sharepoint.com/sites/O365CL` , `contoso` 은 테 넌 트 이름이 며 `O365CL` 사이트 이름입니다. 

### <a name="disabling-telemetry-collection"></a>원격 분석 컬렉션 사용 안 함
이 솔루션의 일부에는 기본적으로 설정 되어 있는 익명 원격 분석 추적 옵트인이 포함 되어 있습니다. 수동 설치를 수행 하는 경우 원격 분석 추적을 해제 하려면 스크립트를 변경 하 여 `CustomlearningConfiguration.ps1` $optInTelemetry 변수를 $false로 설정 하 고 스크립트를 실행 합니다.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>프로 비전 성공 유효성 검사 및 CustomConfig 목록 초기화

PowerShell 스크립트를 성공적으로 실행 한 후 사이트로 이동 하 고 처음 사용 하기 위해 학습 경로를 설정 하는 **Customconfig** 목록 항목을 초기화 한 다음 사이트가 작동 하는지 확인 합니다.

- `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`(으)로 이동합니다. **CustomLearningAdmin** 를 열면 처음 사용할 학습 경로를 설정 하는 **customconfig** 목록 항목이 초기화 됩니다. 다음과 같은 페이지가 표시 됩니다.

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테 넌 트 관리자는 사이트를 사용자 지정 하는 사용자가 될 가능성은 없으며, 사이트에 소수의 소유자를 할당 해야 합니다. 소유자는 사이트 페이지를 수정 하 고 사이트를 다시 브랜딩 할 수 있도록 사이트에 대 한 관리 권한을 가집니다. 또한 학습 경로 웹 파트를 통해 제공 되는 콘텐츠를 숨기 거 나 표시 하는 기능도 제공 됩니다. 또한 사용자 지정 재생 목록을 작성 하 고 사용자 지정 하위 범주에 할당할 수 있습니다.  

1. SharePoint **설정** 메뉴에서 **사이트 사용 권한을**클릭 합니다.
2. **고급 사용 권한 설정을**클릭 합니다.
3. **Office 365 소유자의 학습 경로를**클릭 합니다.
4. **새로 만들기**  >  **사용자를이 그룹에 추가**를 클릭 한 다음 소유자가 하려는 사용자를 추가 합니다. 
5. 링크를 추가 하 여 공유 메시지에서 [사이트를 탐색](https://docs.microsoft.com/Office365/CustomLearning/custom_explore) 하 고 **공유**를 클릭 합니다.

## <a name="migrate-custom-content"></a>사용자 지정 콘텐츠 마이그레이션
위의 단계를 수행 하 여 학습 경로 사이트를 다시 설정한 후에는 **Customplaylists** 목록 목록과 **customplaylists** 목록의 내용을 이동 해야 합니다. 선택적으로 사용자 지정 자산을 구성 하는 실제 사용자 지정 페이지를 기존 학습 경로 사이트에 두고 이동할 수도 있고,이를 삭제 하는 것도 의도입니다. **Customplaylists** 목록에 있는 모든 항목의 경우에는 **customplaylists** 목록에 있는 목록 항목의 ID가 각 재생 목록 항목의 JSONData 필드에 가려질 수 있기 때문에 작업을 어려울 수도 있습니다. 따라서 **Customplaylists** 목록 목록의 내용을 한 사이트에서 다른 사이트로 이동 하는 것 만으로는 충분 하지 않습니다. 또한 **Customassets** 목록에는 목록 항목의 JSONData 필드에 있는 사용자 지정 자산의 페이지에 대 한 절대 URL이 포함 됩니다. 자산을 이동 하지 않고 사이트의 이름을 바꾸지 않으면 (즉, 자산의 페이지에 대 한 절대 URL을 변경 하는 경우) **Customassets** 남아 있을 수 있습니다. 그러나 항목을 수동으로 수정 해야 합니다. 이러한 유형의 마이그레이션에 대 한 복잡성이 주어 지 면이 전환을 지원 하기 위해 학습 경로 파트너 중 하나를 등록 하는 것이 좋습니다. 

### <a name="next-steps"></a>다음 단계
- [사용자 지정 학습 경로](custom_overview.md)를 참조 하세요. 
- [사이트 번역 페이지](custom_translate_page_ml.md)를 참조 하세요.


