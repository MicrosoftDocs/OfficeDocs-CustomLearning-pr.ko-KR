---
author: pkrebs
ms.author: pkrebs
title: 학습 경로 수동 설정
ms.date: 07/06/2020
description: Microsoft 365 경로 수동 설정
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 05df35787399cfb2445fa3ea4193e7f7f64848c5
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310442"
---
# <a name="learning-pathways-manual-setup"></a>학습 경로 수동 설정

Microsoft 365 학습 경로는 다음 시나리오 중 하나에 대한 지원이 필요한 조직을 위한 수동 설정을 제공합니다. 

- 조직에 교육 전용으로 SharePoint 온라인 최신 커뮤니케이션 사이트가 설정되어 있으며 해당 사이트에 학습 경로를 추가하려는 경우 이 시나리오에서는 학습 경로 웹 파트가 사이트에 설정되지 않은 경우

- 조직의 커뮤니케이션 사이트 중 하나에 다국어 지원을 위한 학습 SharePoint 합니다. 사이트에 영어가 아닌 기본 언어가 있으며 학습 경로에서 지원되는 언어 중 하나인 기본 언어가 있습니다. 학습 경로에서 지원하는 언어는 다음과 같습니다.

- 영어
- 중국어(간체)
- 프랑스어
- 독일어
- 이탈리아어(이탈리아)
- 일본어(일본)
- 포르투갈어(브라질)
- 러시아어(러시아어)
- 스페인어

학습 경로를 수동으로 설정하려면 온라인 관리 셸 및 Windows PowerShell 작업하는 SharePoint 필요합니다. 다음은 학습 경로의 수동 설정 단계에 대한 개요입니다. 

- 모든 선행 요구를 충족하는지 검사합니다.
- 사이트의 기본 언어 설정을 확인합니다. 확인이면 수동 설치를 계속 진행합니다. 다른 기본 언어 설정이 필요한 경우 새 사이트를 만들어야 합니다. 
- 테넌트 앱 카탈로그에 customlearning.sppkg SharePoint 설치합니다.
- 학습 경로 홈 사이트로 사용할 최신 커뮤니케이션 Microsoft 365 식별합니다.
- 학습 경로에 따라 달라지는 아티팩트로 테넌트를 구성하는 PowerShell 스크립트를 실행합니다.
- CustomLearningAdmin.aspx 사이트 페이지로 이동하여 관리 웹 파트를 로드하여 사용자 지정 콘텐츠 구성을 초기화합니다.

## <a name="prerequisites"></a>필수 구성 요소
학습 경로 웹 파트를 수동으로 설정하려면 다음의 선행 구성을 충족해야 합니다. 

- 테넌트 전체 앱 카탈로그를 설정하고 구성해야 합니다. [테넌트 설정 Office 365](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) "앱 카탈로그 만들기" 사이트 섹션을 따르십시오. 
- 테넌트 전체 앱 카탈로그가 이미 프로비전된 경우 패키지를 업로드할 권한이 있는 계정에 액세스해야 합니다. 일반적으로 이 계정에는 관리자 역할이 SharePoint 있습니다. 
- 해당 역할의 계정이 작동하지 않는 경우 SharePoint 관리 센터로 이동하여 앱 카탈로그 사이트 모음의 사이트 모음 관리자를 찾아 사이트 모음 관리자 중 한명으로 로그인하거나 사이트 모음 관리자에게 실패한 SharePoint 관리자 계정을 추가합니다. 
- 또한 테넌트 관리자인 계정에 SharePoint 필요합니다.

## <a name="step-1---check-your-language-settings"></a>1단계 - 언어 설정 확인
수동 설치 프로세스의 첫 번째 단계로 사이트 언어 설정을 확인합니다. 가능한 옵션은 다음과 같습니다.

### <a name="option-1---you-dont-want-multilingual-support"></a>옵션 1 - 다국어 지원을 원하지 않습니다.
사이트에 대해 다국어 지원을 원하지 않는 경우 해당 사이트가 꺼져 있는지 확인하세요.
1.  SharePoint 커뮤니케이션 사이트에서 사이트 **설정** 모든 사이트 설정 언어 설정  >    >    >  **보기를 선택합니다.** 
2.  페이지 및 **뉴스를 여러** 언어로 번역할 수 있도록 설정 스위치를 끄기 로 **설정하세요.**
3.  **저장** 을 클릭합니다. 
4.  2단계를 계속 진행합니다.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>옵션 2 - 다국어 지원을 원하고 기본 언어로 확인
SharePoint 통신 사이트에는 기본 언어가 있습니다. 기본 언어는 학습 경로 관리 페이지를 포함하여 학습 경로를 볼 언어를 지정합니다. 기본 언어 설정은 사이트를 처음 만들 때 설정하며 이후에 변경할 수 없습니다. 수동 설치를 계속하기 전에 대상 사이트의 기본 언어로 확인을 합니다.

1.  SharePoint 커뮤니케이션 사이트에서 사이트 **설정** 모든 사이트 설정 언어 설정  >    >    >  **보기를 선택합니다.** 
2.  페이지 및 **뉴스를 여러** 언어로 번역할 수 있도록 설정 스위치를 **켜기 로 설정**
    - 언어 아래의 목록 맨 위에 나타나는 언어를 확인하려면 언어를 더 추가한 다음 저장을 **클릭합니다.** 2단계를 계속 진행합니다.
    - 사이트에 대해 선택한 언어와 다른 기본 언어를 사용하려면 원하는 언어로 새 SharePoint 통신 사이트를 만들어야 합니다. 옵션 3으로 계속합니다. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>옵션 #3 - 다국어 지원을 원하지만 사이트에 대해 다른 기본 언어를 사용하려는 경우
이 옵션을 사용하면 원하는 기본 언어로 SharePoint 온라인 통신 사이트를 새로 만든 다음 사이트의 언어 설정을 지정합니다. 
1.  새 사이트 SharePoint 만들 자세한 내용은 [Create a communication site in SharePoint Online를 참조하세요.](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 사이트를 만들 때 언어를 학습 경로에 필요한 기본 언어로 설정해야 합니다. 
2. 만든 사이트에서 사이트 **설정** 모든 사이트 설정 언어 설정  >    >    >  **보기를 선택합니다.** 
2.  페이지 및 **뉴스를 여러** 언어로 번역할 수 있도록 설정 스위치를 **켜기 로 설정**
3. 필요한 경우 언어를 추가하고 저장을 **클릭합니다.** 
4. 2단계를 계속 진행합니다. 

>! [참고] 사이트에서 새로 만든 사이트로 사용자 지정 콘텐츠를 마이그레이션해야 하는 경우 이 문서 부분의 "사용자 지정 콘텐츠 마이그레이션" 섹션을 참조하십시오. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>2단계 - 웹 파트 패키지 및 설정 스크립트를 GitHub
설치 프로세스의 일부로 학습 경로 웹 파트 Microsoft 365 PowerShell 설치 스크립트가 필요합니다.

- [리포지토리에서 학습 GitHub 이동](https://github.com/pnp/custom-learning-office-365)
- **다운로드를** 클릭하여 웹 파트 패키지 및 스크립트를 로컬 드라이브에 저장합니다. 이 프로세스의 이후 단계에서 스크립트 및 웹 파트 패키지를 사용하게 됩니다.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>2단계 - 업로드 웹 파트를 테넌트 앱 카탈로그에 추가
학습 Microsoft 365 설정하려면 customlearning.sppkg 파일을 테넌트 전체 앱 카탈로그에 업로드하고 배포합니다. 앱 [카탈로그에](/sharepoint/use-app-catalog) 앱을 추가하는 방법에 대한 자세한 내용은 앱 카탈로그를 사용하여 SharePoint Online 환경에 사용자 지정 비즈니스 앱을 사용할 수 있도록 만들기를 참조하세요.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>3단계 - 최신 커뮤니케이션 사이트 프로비전/식별
기존 SharePoint 커뮤니케이션 사이트를 식별하거나 SharePoint 온라인 테넌트에서 새 사이트를 프로비전합니다. 커뮤니케이션 사이트를 프로비전하는 방법에 대한 자세한 내용은 [SharePoint Online에서](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 커뮤니케이션 사이트 만들기를 참조하고 단계에 따라 커뮤니케이션 사이트를 만드십시오.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>4단계 - 사이트에 Microsoft 365 경로 앱 추가

1. SharePoint 사이트에서 시스템 메뉴를 클릭한 다음 앱 **추가를 클릭합니다.** 
2. 앱에서 **조직에서** 를 클릭한 다음 에 대한 학습 경로를 **Office 365.** 

## <a name="step-5---set-permissions-for-the-site"></a>5단계 - 사이트에 대한 사용 권한 설정
사이트에 대해 다음 사용 권한을 설정해야 합니다.
- **사이트 모음 관리자** 또는 Owners 그룹의 일부 - 처음 사용할 학습 경로를 설정하는 CustomConfig 목록 항목을 초기화하는 데 필요한 권한입니다. 
- **구성원 그룹** - 콘텐츠 숨기기 및 표시, 사용자 지정 재생 목록 관리 등 학습 경로 관리에 필요한 권한
- **방문자 그룹** - 사이트 콘텐츠를 보는 데 필요한 권한입니다. 

## <a name="step-6--execute-powershell-configuration-script"></a>6단계- PowerShell 구성 스크립트 실행
솔루션에서 사용하는 세 개의 테넌트 속성을 만들기 위해 실행해야 하는 PowerShell `CustomLearningConfiguration.ps1` 스크립트가 포함되어 [](/sharepoint/dev/spfx/tenant-properties) 있습니다. 또한 스크립트는 사이트 [](/sharepoint/dev/spfx/web-parts/single-part-app-pages) 페이지 라이브러리에 두 개의 단일 파트 앱 페이지를 만들어 알려진 위치에서 관리자 및 사용자 웹 파트를 호스팅합니다.

1. 온라인 관리 셸을 아직 다운로드하지 않은 SharePoint 지금 다운로드하세요. 온라인 [SharePoint 셸 다운로드를 참조하세요.](https://go.microsoft.com/fwlink/p/?LinkId=255251)
2. 스크립트를 실행하려면 PowerShell 실행 정책을 설정해야 할 수 있습니다. 자세한 내용은 실행 정책 [정보를 참조하세요.](/powershell/module/microsoft.powershell.core/about/about_execution_policies)
3. 스크립트를 `CustomLearningConfiguration.ps1` 실행합니다. 테넌트 관리자 자격 증명 외에도 스크립트에서 테넌트 이름 및 사이트 이름을 묻는 메시지가 표시됩니다. 사이트 URL의 다음 예인 는 테넌트 이름이고 `https://contoso.sharepoint.com/sites/O365CL` `contoso` 사이트 `O365CL` 이름입니다. 

### <a name="disabling-telemetry-collection"></a>원격 분석 컬렉션을하지 않습니다.
이 솔루션의 일부에는 기본적으로 설정되어 있는, 비동기화된 원격 분석 추적 옵트인이 포함되어 있습니다. 수동 설치를 수행하고 있으며 원격 분석 추적을 해제하려면 스크립트를 변경하여 $optInTelemetry 변수를 $false `CustomlearningConfiguration.ps1` 실행합니다.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>프로비전 성공의 유효성 검사 및 CustomConfig 목록 초기화

PowerShell 스크립트가 성공적으로 실행된 후 사이트로 이동하고, 처음 사용할 학습 경로를 설정하는 **CustomConfig** 목록 항목을 초기화하고, 사이트가 작동하고 있는지 확인할 수 있습니다.

- `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`으로 이동합니다. **CustomLearningAdmin.aspx** 를 열면 처음 사용할 학습 경로를 설정하는 **CustomConfig** 목록 항목이 초기화됩니다. 다음과 같은 페이지가 표시됩니다.

![샘플 구성 페이지.](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테넌트 관리자는 사이트를 사용자 지정하는 사람이 될 가능성이 낮기 때문에 사이트에 몇 개의 소유자를 할당해야 합니다. 소유자는 사이트에 대한 관리 권한이 있으므로 사이트 페이지를 수정하고 사이트를 다시 브랜드할 수 있습니다. 또한 학습 경로 웹 파트를 통해 전달되는 콘텐츠를 숨기고 표시하는 기능을 제공합니다. 또한 사용자 지정 재생 목록을 빌드하고 사용자 지정 하위 목록에 할당하는 기능을 사용할 수 있습니다.  

1. 사이트 SharePoint **설정** 사이트 사용 권한 **을 클릭합니다.**
2. 고급 **사용 권한 설정** 클릭합니다.
3. 소유자에 대한 학습 **Office 365 클릭합니다.**
4. 이 **그룹에 새** 사용자  >  **추가를 클릭한** 다음 소유자가 될 사용자를 추가합니다. 
5. 공유 메시지에서 [사이트 탐색에](custom_exploresite.md) 대한 링크를 추가하고 공유를 **클릭합니다.**

## <a name="migrate-custom-content"></a>사용자 지정 콘텐츠 마이그레이션
위의 단계를 수행하여 학습 경로 사이트를 다시 설정한 후 **CustomPlaylists** 목록 및 **CustomAssets** 목록의 내용을 이동해야 합니다. 선택적으로 기존 학습 경로 사이트에 있는 경우 사용자 지정 자산을 구성하는 실제 사용자 지정 페이지를 이동할 수 있으며 원하는 경우 해당 페이지를 삭제합니다. **CustomPlaylists** 목록의 모든 항목에 대해 **CustomAssets** 목록의 목록 항목 ID는 각 재생 목록 목록 항목의 JSONData 필드에 묻기 때문에 작업이 어려울 수 있습니다. 따라서 **CustomPlaylists** 목록의 내용을 한 사이트에서 다른 사이트로 이동하는 것만으로는 충분하지 않습니다. 또한 **CustomAssets** 목록에는 목록 항목의 JSONData 필드에 있는 사용자 지정 자산 페이지의 절대 URL이 포함되어 있습니다. 자산이 이동되지 않는 경우 사이트 이름을 바꾸지 않은 경우(따라서 자산의 페이지에 대한 절대 URL을 변경) **CustomAssets는** 그대로 유지될 수 있습니다. 그러나 항목을 수동으로 수정해야 합니다. 이러한 유형의 마이그레이션이 복잡할 경우 학습 경로 파트너 중 하나를 추가하여 이러한 전환을 지원할 것을 제안합니다. 

### <a name="next-steps"></a>다음 단계
- 학습 [경로 사용자 지정을 참조합니다.](custom_overview.md) 
- 사이트 [페이지 번역을 참조하세요.](custom_translate_page_ml.md)