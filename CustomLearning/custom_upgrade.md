---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 업그레이드
ms.date: 02/10/2019
description: Office 365 수동 웹 파트 설정에 대 한 사용자 지정 학습
ms.openlocfilehash: 72ac6f7a135697b816f2decbf010ec439562598f
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523073"
---
# <a name="manual-upgrade-for-custom-learning"></a>사용자 지정 학습을 위한 수동 업그레이드

Office 365에 대 한 사용자 지정 학습은 이전 파일럿에 참여 한 조직에 대해 수동 업그레이드 프로세스를 제공 합니다. 업그레이드 프로세스를 통해 조직은 새로운 향상 된 사용자 지정 학습 웹 파트를 SharePoint 앱 카탈로그에 추가한 다음 PowerShell 스크립트를 실행 하 여 현재 사용자 지정 학습 사이트와 업그레이드를 계속 사용할 수 있습니다. 다음은 업그레이드 프로세스에 대 한 간략 한 설명입니다. 

- 새 웹 파트를 업로드 하 고 Powershell 스크립트를 실행 하는 사용자에 게 필요한 권한이 있는지 확인 합니다.
- 웹 파트, customlearning 파일을 Office 365 테 넌 트 앱 카탈로그에 업로드 합니다.
- 사용자 지정 학습에 필요한 적절 한 아티팩트를 사용 하 여 테 넌 트를 구성 하는 PowerShell 스크립트를 실행 합니다.
- 사용자 지정 학습 사이트의 CustomLearningAdmin 페이지로 이동 하 여 사용자 지정 ccontent 구성을 초기화 합니다.

## <a name="prerequisites"></a>필수 구성 요소
사용자 지정 학습을 성공적으로 업그레이드 하려면 다음 필수 구성 요소를 충족 해야 합니다. 

- 테 넌 트 전체 앱 카탈로그를 설정 해야 합니다. 테 넌 트 앱 카탈로그가 없는 경우 [Office 365 테 넌 트 설정을](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 참조 하 고 앱 카탈로그 사이트 만들기 섹션을 따르세요. 
- 테 넌 트 전체 앱 카탈로그가 이미 프로 비전 된 경우 패키지를 업로드 하는 데 필요한 권한을 가진 계정에 대 한 액세스 권한이 있어야 합니다. 일반적으로 SharePoint 관리자 역할이 있는 계정입니다. 
- sharepoint 관리자 역할이 있는 계정이 작동 하지 않는 경우 sharepoint 관리 센터로 이동 하 여 앱 카탈로그를 선택 하 고, 소유자를 클릭 하 고, 사이트 모음 관리자 중 한 명에 게 로그인 하거나, 사이트에 오류가 발생 한 SharePoint 관리자 계정을 추가 합니다. 모음 관리자 목록 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>1 단계-GitHub에서 웹 파트 패키지 및 설치 스크립트 가져오기
설치 프로세스의 일부로 사용자 지정 학습 웹 파트 패키지 및 PowerShell 설치 스크립트가 필요 합니다.

1. [사용자 지정 학습 GitHub 리포지토리](https://github.com/pnp/custom-learning-office-365)를 방문 합니다.
2. **복제 또는 다운로드**를 클릭 한 다음 **ZIP을 다운로드**합니다.   
3. 로컬 드라이브의 위치에 **ZIP** 파일을 저장 합니다.
4. 로컬 드라이브에서 **ZIP** 파일을 추출 합니다.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>2 단계-테 넌 트 앱 카탈로그에 웹 파트 업로드
Office 365에 대 한 사용자 지정 학습을 설정 하려면 테 넌 트 전체 앱 카탈로그에 customlearning 파일을 업로드 하 고 배포 합니다. 앱 카탈로그에 앱을 추가 하는 방법에 대 한 자세한 내용은 [앱 카탈로그를 사용 하 여 SharePoint Online 환경에서 사용할 수 있는 사용자 지정 비즈니스 앱 만들기를](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) 참조 하세요.

1. Office 365에서 **관리자**를 클릭 합니다.
2. **관리 센터**에서 **SharePoint**를 클릭 합니다.
3. **apps** > **앱 카탈로그** > **배포 앱 SharePoint를 클릭 합니다.**
4. **파일 선택을** **업로드** > 합니다 .를 클릭 합니다.
5. ZIP 파일을 저장 한 폴더에서 **webpart** 폴더를 선택 하 고 **customlearning** 을 선택 합니다.
6. **배포**를 클릭합니다.

## <a name="step-5--execute-powershell-configuration-script"></a>5 단계-PowerShell 구성 스크립트 실행
PowerShell 스크립트 `CustomLearningConfiguration.ps1` 는 GitHub에서의 ZIP 다운로드에 포함 됩니다. 솔루션에서 사용 하는 세 개의 [테 넌 트 속성](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) 을 만들려면 스크립트를 실행 해야 합니다. 또한이 스크립트는 사이트 페이지 라이브러리에 두 개의 [단일 파트 앱 페이지](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) 를 만들어 관리자 및 사용자 웹 파트를 알려진 위치에 호스트 합니다. 이러한 앱 페이지는 다음과 같습니다.

- customadministration .aspx
- customviewer .aspx

### <a name="to-run-the-powershell-script"></a>Powershell 스크립트를 실행 하려면
- PowerShell을 사용 하 여 `CustomLearningConfiguration.ps1` GitHub ZIP에서 webpart 폴더에 있는 스크립트를 실행 합니다. 성공 하면 명령 창에 세 개의 키/값 쌍과 **사용자 지정 학습 관리자** 가 표시 됩니다.

### <a name="disabling-telemetry-collection"></a>원격 분석 컬렉션 사용 안 함
사용자 지정 학습에는 익명 원격 분석 추적 옵트인 (기본적으로 설정 됨)이 포함 됩니다. 원격 분석 추적을 해제 하려면 `CustomlearningConfiguration.ps1` `$optInTelemetry` 변수를로 `$false`설정 하도록 스크립트를 변경 하십시오.

## <a name="step-6---initialize-web-part-custom-configuration"></a>6 단계-웹 파트 사용자 지정 구성 초기화
PowerShell 스크립트를 성공적으로 실행 한 후로 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`이동 합니다. **CustomLearningAdmin** 를 열면 처음 사용할 사용자 지정 학습을 설정 하는 **customconfig** 목록 항목이 초기화 됩니다. 다음과 같은 페이지가 표시 됩니다.

![cg-adminapppage-.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테 넌 트 관리자는 사이트를 사용자 지정 하는 사용자가 될 가능성은 없으며, 사이트에 소수의 소유자를 할당 해야 합니다. 소유자는 사이트 페이지를 수정 하 고 사이트를 다시 브랜딩 할 수 있도록 사이트에 대 한 관리 권한을 가집니다. 또한 사용자 지정 학습 웹 파트를 통해 제공 되는 콘텐츠를 숨기 거 나 표시 하는 기능도 제공 됩니다. 또한 사용자 지정 재생 목록을 작성 하 고 사용자 지정 하위 범주에 할당할 수 있습니다.  

1. SharePoint **설정** 메뉴에서 **사이트 사용 권한을**클릭 합니다.
2. **고급 사용 권한 설정을**클릭 합니다.
3. **Office 365 소유자에 대 한 사용자 지정 학습을**클릭 합니다.
4. **새로 만들기** > **사용자를이 그룹에 추가**를 클릭 하 고 소유자를 부여할 사용자를 추가한 다음 **공유**를 클릭 합니다.

이제 업그레이드가 완료 되었습니다. 환경에 맞게 사용자 지정 학습 사이트 및 웹 파트를 조정 하는 방법에 대 한 자세한 내용은 [교육 환경 사용자 지정](custom_overview.md)을 참조 하십시오.

## <a name="upgrade-instructions-for-site-owners"></a>사이트 소유자에 대 한 업그레이드 지침
office 365에 대 한 사용자 지정 학습은 웹 파트에 대 한 다양 한 향상 된 기능을 소개 합니다. 웹 파트에 대 한 작업은 [학습 환경 사용자 지정](custom_overview.md) 섹션에 자세히 설명 되어 있습니다. 이제 사이트 소유자는 다음을 수행 해야 합니다.  

- Office 365 웹 파트에 대 한 사용자 지정 학습을 사용할 수 있는지 확인 합니다. 
- 페이지의 기존 웹 파트를 새 웹 파트로 바꾸기
- 이전 웹 파트를 가리키는 링크 바꾸기

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>Office 365 웹 파트에 대 한 사용자 지정 학습을 사용할 수 있는지 확인
1.  사용자 지정 학습 사이트에서 **설정을**클릭 한 다음 ***페이지 추가를**클릭 합니다.
2.  페이지에서 **+** 아이콘을 클릭 하 여 웹 파트를 추가한 다음 Office 365 웹 파트 **에 대 한 사용자 지정 학습** 을 선택 합니다. 페이지는 이제 다음과 같은 그래픽과 같습니다.

[cg-adminapppage-.png](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>이전 웹 파트를 새 웹 파트로 바꾸기
사용자 지정 학습 웹 파트를 교체 하거나 사이트를 변경 하기 전에 새 웹 파트를 사용 하는 방법에 대해 설명 하는 것 처럼 [학습 환경 사용자 지정](custom_overview.md) 문서를 읽는 것이 좋습니다. 

사용자 지정 학습 사이트를 업그레이드 하려면 웹 파트의 기존 인스턴스를 새 웹 파트로 바꿉니다. 웹 파트가 추가 된 위치를 확인할 수는 없지만 이전 파일럿에 대 한 지침은 다음 페이지에 웹 파트를 추가 했기 때문에이 페이지에서 웹 파트를 바꿉니다.

- Get-started-with-Office-365 .aspx
- Get-started-with-Microsoft-Teams .aspx
- Get-started-with-OneDrive .aspx
- Get-started-with-SharePoint .aspx

### <a name="replace-existing-links-to-the-web-part"></a>웹 파트에 대 한 기존 링크 바꾸기
새 웹 파트에 대 한 향상 된 기능을 통해 재생 목록에 연결 하는 방식이 변경 되었습니다. 업그레이드의 일환으로 웹 파트에 대 한 링크를 메뉴 항목, 홈 페이지의 링크 등으로 바꿔야 합니다. 사용자 지정 학습 웹 파트를 교체 하거나 사이트를 변경 하기 전에 새 웹 파트를 사용 하는 방법에 대해 설명 하는 것 처럼 [학습 환경 사용자 지정](custom_overview.md) 문서를 읽는 것이 좋습니다. 

## <a name="recreate-existing-playlists"></a>기존 재생 목록 다시 만들기 
재생 목록이 제대로 작동 하도록 하기 위해 이전 버전의 웹 파트를 사용 하 여 만든 재생 목록을 다시 만들어야 합니다. 재생 목록을 삭제 하기 전에 새 사용자 지정 학습 웹 파트를 사용 하 여 쉽게 다시 만들 수 있도록 사용자 지정 재생 목록 및 관련 자산의 목록을 만듭니다. 재생 목록의 복사본을 만든 다음 삭제 합니다. 삭제 하기 전에 JSONData 필드를 사용 하 여 재생 목록 내용의 복사본을 만들 수 있습니다. 이를 통해 나중에 쉽게 만들 수 있습니다.


1. 사용자 지정 학습 사이트에서**사이트 콘텐츠** **설정을** > 클릭 합니다. 
2. 재생 목록을 선택 하 고 줄임표를 선택한 다음 **편집**을 선택 하 고 **JSONData** 필드의 내용을 복사한 다음 나중에 참조 하기 위해 메모장 이나 별도의 문서에 저장 합니다. **취소**를 선택 합니다.
3. 재생 목록을 선택 하 고 줄임표를 선택한 다음 **삭제**를 선택 합니다.
4. 이제 새 웹 파트로 재생 목록을 다시 만들 준비가 되었습니다.
Office 365 웹 파트에 대 한 사용자 지정 학습을 사용 하는 방법에 대 한 자세한 내용은 [학습 환경 사용자 지정 (custom_overview)을 참조 하십시오.

### <a name="next-steps"></a>다음 단계
- 조직의 교육 환경 [사용자 지정](custom_overview.md)

