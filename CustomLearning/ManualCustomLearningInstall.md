---
author: pkrebs
ms.author: pkrebs
title: 수동 설치 학습 경로
ms.date: 02/18/2019
description: 수동 설치 학습 경로
ms.service: sharepoint online
ms.openlocfilehash: a9ae97bbafcc82c54251cae9a0ad658b7a0c16f4
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234670"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Office 365에 대 한 사용자 지정 학습을 수동으로 설치 및 구성

Microsoft 사용자 지정 학습 웹 파트는 [SharePoint Framework](https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview) 버전 1.7.1을 사용 하 여 작성 됩니다.

웹 파트 및 사이트 모음을 수동으로 설치 및 구성 하려면 다음 단계를 완료 해야 합니다.

1. 모든 필수 구성 요소를 충족 했는지 확인 합니다.
1. Office 365 테 넌 트 앱 카탈로그에 customlearning 파일을 설치 합니다.
1. Office 365 홈 사이트에 대 한 사용자 지정 학습 역할을 하는 최신 커뮤니케이션 사이트를 구축/식별 합니다.
1. 사용자 지정 학습에 따라 적절 한 아티팩트를 사용 하 여 테 넌 트를 구성 하는 PowerShell 스크립트를 실행 합니다.
1. CustomLearningAdmin 사이트 페이지로 이동 하 여 사용자 지정 콘텐츠 구성을 초기화 하기 위해 관리 웹 파트를 로드 합니다.

## <a name="prerequisites"></a>필수 구성 요소

테 넌 트 전체 앱 카탈로그를 설정 하 고 구성 해야 합니다. [Office 365 테 넌 트 설정을](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 참조 하 고 앱 카탈로그 사이트 만들기 섹션을 따르세요. 테 넌 트 전체 앱 카탈로그가 이미 프로 비전 된 경우에는이 설치 프로세스를 완료 하기 위해 패키지를 업로드 하는 권한이 있는 계정에 대 한 액세스 권한을 받아야 합니다. 일반적으로 SharePoint 관리자 역할이 있는 계정입니다. 해당 역할이 있는 계정이 작동 하지 않으면 SharePoint 관리 센터로 이동 하 여 앱 카탈로그 사이트 모음에 대 한 사이트 모음 관리자를 찾은 다음 사이트 모음 관리자 중 한 명으로 로그인 하거나 사이트 모음 관리자에 게 실패 한 SharePoint 관리자 계정을 추가 합니다. 또한 SharePoint 테 넌 트 관리자 인 계정에도 액세스 해야 합니다.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>테 넌 트 앱 카탈로그에 웹 파트 업로드

Office 365에 대 한 사용자 지정 학습을 설정 하려면 테 넌 트 전체 앱 카탈로그에 customlearning 파일을 업로드 하 고 배포 합니다. 앱 카탈로그에 앱을 추가 하는 방법에 대 한 자세한 내용은 [앱 카탈로그를 사용 하 여 SharePoint Online 환경에서 사용할 수 있는 사용자 지정 비즈니스 앱 만들기를](https://docs.microsoft.com/sharepoint/use-app-catalog) 참조 하세요.

## <a name="provisionidentify-modern-communication-site"></a>최신 통신 사이트 프로 비전/식별

기존 SharePoint communication site를 식별 하거나 SharePoint Online 테 넌 트에서 새 사이트를 프로 비전 합니다. 통신 사이트를 구축 하는 방법에 대 한 자세한 내용은 [SharePoint Online에서 커뮤니케이션 사이트 만들기](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 및 단계에 따라 통신 사이트 만들기를 참조 하세요.

## <a name="set-permissions-for-the-site"></a>사이트에 대 한 사용 권한 설정

방문자 그룹에 콘텐츠를 볼 수 있어야 하는 사람과 사용자 지정 재생 목록을 구성원 그룹으로 관리할 수 있는 모든 사용자를 추가 해야 합니다. 사용자가 처음으로 사이트 모음 관리자 또는 소유자 그룹의 일부일 때 사용자 지정 학습을 사용 하도록 사이트를 구성 합니다.

Office 365 앱에 대 한 사용자 지정 학습을 사이트 모음에 추가 합니다.

## <a name="execute-powershell-configuration-script"></a>PowerShell 구성 스크립트 실행

`CustomLearningConfiguration.ps1`솔루션에서 사용 하는 세 개의 [테 넌 트 속성](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties) 을 만들기 위해 실행 해야 하는 PowerShell 스크립트가 포함 됩니다. 또한 스크립트는 사이트 페이지 라이브러리에 두 개의 [단일 파트 앱 페이지](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages) 를 만들어 관리자 및 사용자 웹 파트를 알려진 위치에 호스트 합니다.

### <a name="disabling-telemetry-collection"></a>원격 분석 컬렉션 사용 안 함

이 솔루션의 일부에는 기본적으로 설정 되어 있는 익명 원격 분석 추적 옵트인이 포함 되어 있습니다. 수동 설치를 수행 하는 경우 원격 분석 추적을 해제 하려면 스크립트를 변경 `CustomlearningConfiguration.ps1` 하 여 $optInTelemetry 변수를 $false로 설정 하십시오.

수동 설치를 수행 하지 않고 원격 분석 추적을 해제 하려는 경우에는 `TelemetryOptOut.ps1` 실행 시 원격 분석 추적을 사용 하지 않도록 설정 하는 별도의 스크립트가 포함 되었습니다.

## <a name="initialize-web-part-custom-configuration"></a>웹 파트 사용자 지정 구성 초기화

PowerShell 스크립트를 성공적으로 실행 한 후로 이동 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 합니다. 이 명령은 처음 사용을 위해 사용자 지정 학습을 설정 하는 CustomConfig 목록 항목을 초기화 합니다.

이제 구성이 완료 되며 Office 365에 대 한 사용자 지정 학습을 사용 하 여 앞으로 이동할 수 있습니다. 자세한 내용은 사용자 설명서를 참조 하세요.