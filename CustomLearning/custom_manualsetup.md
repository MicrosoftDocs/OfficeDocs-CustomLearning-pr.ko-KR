---
author: pkrebs
ms.author: pkrebs
title: 독립 실행형 웹 파트 설정
ms.date: 02/10/2019
description: Office 365 수동 웹 파트 설정에 대 한 사용자 지정 학습
ms.openlocfilehash: f5d94d673f491d5b5778ef73d518914dbd4cdbb9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523062"
---
# <a name="stand-alone-web-part-setup"></a>독립 실행형 웹 파트 설정

사용자 지정 학습은 교육 전용으로 설정 된 SharePoint Online 최신 통신 사이트가 이미 있는 조직에 대해 수동, 독립 실행형 웹 파트 설치를 제공 하거나 사용자 지정 학습 웹 파트를 직접 설정 하려는 경우에만 사용할 수 있습니다. 통신 사이트 수동 설정에는 Windows PowerShell 및 SharePoint Online 관리 셸에서 작업 하는 경험이 필요 합니다. 사용자 지정 학습 웹 파트를 수동으로 설정 하는 단계는 다음과 같습니다.

- 모든 필수 구성 요소를 충족 했는지 확인 합니다.
- Office 365 테 넌 트 앱 카탈로그에 customlearning 파일을 설치 합니다.
- Office 365 홈 사이트에 대 한 사용자 지정 학습 역할을 하는 최신 커뮤니케이션 사이트를 구축/식별 합니다.
- 사용자 지정 학습에 따라 적절 한 아티팩트를 사용 하 여 테 넌 트를 구성 하는 PowerShell 스크립트를 실행 합니다.
- CustomLearningAdmin 사이트 페이지로 이동 하 여 사용자 지정 콘텐츠 구성을 초기화 하기 위해 관리 웹 파트를 로드 합니다.

> [!NOTE]
> 사용자 지정 학습을 빠르고 쉽게 설정할 수 있는 방법은 [구축 사용자 지정 학습](installsitepackage.md)을 참조 하십시오.

## <a name="prerequisites"></a>필수 구성 요소
사용자 지정 학습 웹 파트를 수동으로 설치 하기 위해서는 다음 필수 구성 요소를 충족 해야 합니다. 

- 테 넌 트 전체 앱 카탈로그를 설정 하 고 구성 해야 합니다. [Office 365 테 넌 트 설정을](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 참조 하 고 앱 카탈로그 사이트 만들기 섹션을 따르세요. 
- 테 넌 트 전체 앱 카탈로그가 이미 프로 비전 된 경우에는이 설치 프로세스를 완료 하기 위해 패키지를 업로드 하는 권한이 있는 계정에 대 한 액세스 권한을 받아야 합니다. 일반적으로 SharePoint 관리자 역할이 있는 계정입니다. 
- 해당 역할이 있는 계정이 작동 하지 않으면 SharePoint 관리 센터로 이동 하 여 앱 카탈로그 사이트 모음에 대 한 사이트 모음 관리자를 찾고 사이트 모음 관리자 중 한 명으로 로그인 하거나 SharePoint 관리자 계정을 추가 합니다. 사이트 모음 관리자에 게 실패 한 것입니다. 
- 또한 SharePoint 테 넌 트 관리자 인 계정에도 액세스 해야 합니다.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>1 단계-GitHub에서 웹 파트 패키지 및 설치 스크립트 가져오기
설치 프로세스의 일부로 사용자 지정 학습 웹 파트 패키지 및 PowerShell 설치 스크립트가 필요 합니다.

- [사용자 지정 학습 GitHub 리포지토리](https://github.com/pnp/custom-learning-office-365)를 방문 합니다.
- **다운로드** 를 클릭 하 여 웹 파트 패키지와 스크립트를 로컬 드라이브에 저장 합니다. 이 프로세스의 이후 단계에서 스크립트 및 웹 파트 패키지를 사용 하 게 됩니다.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>2 단계-테 넌 트 앱 카탈로그에 웹 파트 업로드
Office 365에 대 한 사용자 지정 학습을 설정 하려면 테 넌 트 전체 앱 카탈로그에 customlearning 파일을 업로드 하 고 배포 합니다. 앱 카탈로그에 앱을 추가 하는 방법에 대 한 자세한 내용은 [앱 카탈로그를 사용 하 여 SharePoint Online 환경에서 사용할 수 있는 사용자 지정 비즈니스 앱 만들기를](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) 참조 하세요.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>3 단계-최신 커뮤니케이션 사이트 프로 비전/식별
기존 sharepoint communication site를 식별 하거나 sharepoint Online 테 넌 트에서 새 사이트를 프로 비전 합니다. 통신 사이트를 구축 하는 방법에 대 한 자세한 내용은 [SharePoint Online에서 커뮤니케이션 사이트 만들기](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 및 단계에 따라 통신 사이트 만들기를 참조 하세요.

## <a name="step-4---set-permissions-for-the-site"></a>4 단계-사이트에 대 한 사용 권한 설정
사이트에 대해 다음 권한이 설정 되어 있는지 확인 합니다.
- **사이트 모음 관리자 또는 소유자 그룹의 일부** -처음 사용을 위해 사용자 지정 학습을 설정 하는 customconfig 목록 항목을 초기화 하는 데 필요한 사용 권한입니다. 
- **구성원 그룹** -콘텐츠 숨기기 및 표시, 사용자 지정 재생 목록 관리 등 사용자 지정 학습을 관리 하는 데 필요한 permissons
- **방문자 그룹** -사이트 콘텐츠를 보는 데 필요한 사용 권한 

## <a name="step-5--execute-powershell-configuration-script"></a>5 단계-PowerShell 구성 스크립트 실행
솔루션에서 사용 `CustomLearningConfiguration.ps1` 하는 세 개의 [테 넌 트 속성](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) 을 만들기 위해 실행 해야 하는 PowerShell 스크립트가 포함 됩니다. 또한 스크립트는 사이트 페이지 라이브러리에 두 개의 [단일 파트 앱 페이지](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) 를 만들어 관리자 및 사용자 웹 파트를 알려진 위치에 호스트 합니다.

### <a name="disabling-telemetry-collection"></a>원격 분석 컬렉션 사용 안 함
이 솔루션의 일부에는 기본적으로 설정 되어 있는 익명 원격 분석 추적 옵트인이 포함 되어 있습니다. 수동 설치를 수행 하는 경우 원격 분석 추적을 해제 하려면 `CustomlearningConfiguration.ps1` 스크립트를 변경 하 여 $optInTelemetry 변수를 $false로 설정 하십시오.

수동 설치를 수행 하지 않고 원격 분석 추적을 해제 하려는 경우에는 실행 시 원격 분석 추적 `TelemetryOptOut.ps1` 을 사용 하지 않도록 설정 하는 별도의 스크립트가 포함 되었습니다.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>프로 비전 성공 유효성 검사 및 customconfig 목록 초기화

PowerShell 스크립트가 성공적으로 실행 되 면 사이트로 이동 하 여 처음 사용할 사용자 지정 학습을 설정 하는 **customconfig** 목록 항목을 초기화 하 고 사이트가 작동 하는지 확인 합니다.

1. `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`으로 이동합니다. **CustomLearningAdmin** 를 열면 처음 사용할 사용자 지정 학습을 설정 하는 **customconfig** 목록 항목이 초기화 됩니다. 다음과 같은 페이지가 표시 됩니다.

![cg-adminapppage-.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테 넌 트 관리자는 사이트를 사용자 지정 하는 사용자가 될 가능성은 없으며, 사이트에 소수의 소유자를 할당 해야 합니다. 소유자는 사이트 페이지를 수정 하 고 사이트를 다시 브랜딩 할 수 있도록 사이트에 대 한 관리 권한을 가집니다. 또한 사용자 지정 학습 웹 파트를 통해 제공 되는 콘텐츠를 숨기 거 나 표시 하는 기능도 제공 됩니다. 또한 사용자 지정 재생 목록을 작성 하 고 사용자 지정 하위 범주에 할당할 수 있습니다.  

1. SharePoint **설정** 메뉴에서 **사이트 사용 권한을**클릭 합니다.
2. **고급 사용 권한 설정을**클릭 합니다.
3. **Office 365 소유자에 대 한 사용자 지정 학습을**클릭 합니다.
4. **새로 만들기** > **사용자를이 그룹에 추가**를 클릭 한 다음 소유자가 하려는 사용자를 추가 합니다. 
5. 링크를 추가 하 여 공유 메시지에서 [사이트를 탐색](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore) 하 고 **공유**를 클릭 합니다.

### <a name="next-steps"></a>다음 단계
- 조직의 교육 환경 [사용자 지정](custom_overview.md)

