---
author: pkrebs
ms.author: pkrebs
title: 수동 설치 학습 경로
ms.date: 02/18/2019
manager: bpardi
description: 수동 설치 학습 경로
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575973"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>사용자 지정 학습을 수동으로 설치하고 Office 365

Microsoft 사용자 지정 학습 웹 [](/sharepoint/dev/spfx/sharepoint-framework-overview) 파트는 SharePoint 프레임워크 버전 1.7.1을 사용하여 빌드됩니다.

웹 파트 및 사이트 모음을 수동으로 설치 및 구성하려면 다음 단계를 완료해야 합니다.

1. 모든 선행 요구를 충족하는지 검사합니다.
1. 테넌트 앱 카탈로그에 customlearning.sppkg Office 365 설치합니다.
1. 홈 사이트의 사용자 지정 학습 역할을 할 최신 Office 365 식별합니다.
1. 사용자 지정 학습이 사용하는 적절한 아티팩트로 테넌트를 구성하는 PowerShell 스크립트를 실행합니다.
1. CustomLearningAdmin.aspx 사이트 페이지로 이동하여 관리 웹 파트를 로드하여 사용자 지정 콘텐츠 구성을 초기화합니다.

## <a name="prerequisites"></a>필수 구성 요소

테넌트 전체 앱 카탈로그를 설정하고 구성해야 합니다. [테넌트 설정 Office 365](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 앱 카탈로그 사이트 만들기 섹션을 따르십시오. 테넌트 전체 앱 카탈로그가 이미 프로비전된 경우 이 설치 프로세스를 완료하기 위해 패키지를 업로드할 권한이 있는 계정에 액세스해야 합니다. 일반적으로 이 계정에는 관리자 역할이 SharePoint 있습니다. 해당 역할의 계정이 작동하지 않는 경우 SharePoint 관리 센터로 이동하여 앱 카탈로그 사이트 모음에 대한 사이트 모음 관리자를 찾아 사이트 모음 관리자 중 하나로 로그인하거나 사이트 모음 관리자에게 실패한 SharePoint 관리자 계정을 추가합니다. 또한 테넌트 관리자인 계정에 SharePoint 액세스해야 합니다.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>업로드 웹 파트를 테넌트 앱 카탈로그에 추가

사용자 지정 학습을 Office 365 사용자 지정 학습을 설정하려면 customlearning.sppkg 파일을 테넌트 전체 앱 카탈로그에 업로드하고 배포합니다. 앱 [카탈로그에](/sharepoint/use-app-catalog) 앱을 추가하는 방법에 대한 자세한 내용은 앱 카탈로그를 사용하여 SharePoint Online 환경에 사용자 지정 비즈니스 앱을 사용할 수 있도록 만들기를 참조하세요.

## <a name="provisionidentify-modern-communication-site"></a>최신 커뮤니케이션 사이트 프로비전/식별

기존 SharePoint 커뮤니케이션 사이트를 식별하거나 SharePoint 온라인 테넌트에서 새 사이트를 프로비전합니다. 커뮤니케이션 사이트를 프로비전하는 방법에 대한 자세한 내용은 [SharePoint Online에서](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 커뮤니케이션 사이트 만들기를 참조하고 단계에 따라 커뮤니케이션 사이트를 만드십시오.

## <a name="set-permissions-for-the-site"></a>사이트에 대한 사용 권한 설정

방문자 그룹에 콘텐츠를 볼 수 있는 모든 사용자와 사용자 지정 재생 목록을 관리할 수 있는 모든 사람을 구성원 그룹에 추가해야 합니다. 사용자가 처음 사이트 모음 관리자 또는 Owners 그룹의 일부가 되어야 하는 경우 사용자 지정 학습에 맞게 사이트를 구성하려면

사이트 모음에 Office 365 사용자 지정 학습을 추가합니다.

## <a name="execute-powershell-configuration-script"></a>PowerShell 구성 스크립트 실행

솔루션에서 사용하는 세 개의 테넌트 속성을 만들기 위해 실행해야 하는 PowerShell `CustomLearningConfiguration.ps1` 스크립트가 포함되어 [](/sharepoint/dev/spfx/tenant-properties) 있습니다. 또한 스크립트는 사이트 [](/sharepoint/dev/spfx/web-parts/single-part-app-pages) 페이지 라이브러리에 두 개의 단일 파트 앱 페이지를 만들어 알려진 위치에서 관리자 및 사용자 웹 파트를 호스팅합니다.

### <a name="disabling-telemetry-collection"></a>원격 분석 컬렉션을하지 않습니다.

이 솔루션의 일부에는 기본적으로 설정되어 있는, 비동기화된 원격 분석 추적 옵트인이 포함되어 있습니다. 수동 설치를 수행하고 원격 분석 추적을 해제하려면 스크립트를 변경하여 $optInTelemetry 변수를 `CustomlearningConfiguration.ps1` $false.

수동 설치를 수행하지 않는 경우 원격 분석 추적을 해제하려면 실행 시 원격 분석 추적을 사용하지 않도록 설정하는 별도의 `TelemetryOptOut.ps1` 스크립트가 포함되어 있습니다.

## <a name="initialize-web-part-custom-configuration"></a>웹 파트 사용자 지정 구성 초기화

PowerShell 스크립트가 성공적으로 실행된 후 로 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 이동합니다. 이렇게 하면 처음 사용할 사용자 지정 학습을 설정하는 CustomConfig 목록 항목이 초기화됩니다.

이제 구성이 완료되어 사용자 지정 학습을 사용하여 구성을 진행할 수 Office 365. 자세한 내용은 사용자 설명서를 참조하십시오.
