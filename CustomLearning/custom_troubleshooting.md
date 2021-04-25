---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 문제 해결
ms.date: 02/10/2019
description: Microsoft 365 학습 경로 문제 해결 방법 학습
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000304"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Microsoft 365 학습 경로 문제 해결

다음은 Microsoft 365 학습 경로 또는 SharePoint Online 프로비전 서비스에서 발생할 수 있는 문제에 대한 문제 해결 팁입니다.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>테넌트 관리자 권한이 있는 경우를 아는 방법

SharePoint Online 프로비저닝 서비스에 로그인하고 사용자 지정 학습을 프로비저닝하려면 테넌트 관리자 권한이 필요합니다. SharePoint Online 프로비저닝 서비스에 로그인 문제가 발생하는 경우 전역 관리자 역할이 할당되어 있는지 확인 합니다. 사용자 지정 학습 솔루션에는 테넌트 관리자 권한이 필요합니다(그렇지 않으면 Office 365 전역 관리자 역할). 전역 관리자 역할이 할당되어 있는지 확인하는 방법에는 다음이 있습니다.

1.  로그인하여 Office.com.
2.  관리자를 **클릭합니다.**
3.  사용자 **아래에서** 활성 **사용자를 선택합니다.**
4.  이름 검색
5.  검색 결과에서 이름을 클릭합니다. 역할에 대한 전역 관리자가 표시 됩니다.
![라이선스, 그룹 구성원 자격 및 기타 정보와 함께 역할을 나열하는 샘플 페이지입니다.](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>전역 관리자 역할이 없는 경우
- 조직에서 전역 관리자를 찾아 해당 사용자가 서비스에 로그인하게 하거나 사용자에게 전역 관리자 역할을 할당하게 합니다.

## <a name="tenant-app-catalog-troubleshooting"></a>테넌트 앱 카탈로그 문제 해결
사용자 지정 학습을 사용하려면 대상 테넌트에 앱 카탈로그를 프로비전해야 합니다. 앱 카탈로그를 만들려면 전역 관리자 권한이 필요합니다. 다음은 일반적인 앱 카탈로그 문제에 대한 문제 해결 단계입니다.

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>테넌트 앱 카탈로그가 있는지 아는 방법 
먼저 전역 관리자 권한이 있는지 확인 합니다. 위의 테넌트 관리자 권한에 대한 단계를 참조하세요.

1. Office 365에서 **관리자,** 확장 화살표 > 클릭하고 모든 관리 센터  >    >  **SharePoint 표시를 클릭합니다.**
2. 클래식 **관리자 SharePoint 센터 앱**  >  **앱** 카탈로그  >  **를 클릭합니다.**
3. 앱 **아래에** SharePoint용 앱 배포 제목의 **타일이 표시됩니다.** 타일이 표시되어 있는 경우 테넌트 앱 카탈로그가 있습니다. 아래 **사이트 구성...** 섹션을 참조하세요. 타일이 없는 경우 테넌트에 대한 테넌트 앱 카탈로그를 만들어야 합니다. 아래 테넌트 앱 **카탈로그를 만드는** 방법 섹션을 참조하세요.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>테넌트 앱 카탈로그에서 사이트 모음 소유자가 되도록 하는 방법 
Microsoft 365 학습 경로를 프로비저닝하려면 테넌트 앱 카탈로그의 사이트 모음 소유자가 해야 합니다. 소유자인지 확인하는 방법에는 다음이 있습니다.

1. Office 365에서 **관리자,** 확장 화살표 > 클릭하고 모든 관리 센터  >    >  **SharePoint 표시를 클릭합니다.**
2. 클래식 **관리 SharePoint 센터를 클릭한** 다음 앱 카탈로그 **를 선택합니다.**
3. 소유자 **를** 선택한 다음 사이트 모음 소유자가 되도록 합니다. 모양은 다음과 같아야 합니다.
![관리자 관리 페이지.](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>없는 경우 테넌트 앱 카탈로그를 만드는 방법 
1. SharePoint Online 관리자 계정으로 Office 365에 로그인합니다.
2. **관리자** 를 클릭합니다.
3. 관리 **센터에서** **SharePoint 를 클릭합니다.** 
4. 앱 **앱 카탈로그**  >  **를 클릭합니다.**
5. 새 **앱 카탈로그 사이트 만들기를 클릭한** 다음 확인 을 **클릭합니다.** 
6.  앱 카탈로그에 대한 정보를 입력합니다. 관리자를 두 개 이상 포함할 수 있습니다. 다음은 예를 보여 주는 예제입니다.  
![새 앱 카탈로그에 대한 정보를 입력할 양식입니다.](media/cg-appcatalogfinish.png)

7.  그거에요. 완료한 것입니다. 그러나 프로비저닝 사용자 지정 학습으로 이동하기 전에 앱 카탈로그 만들기가 완료될 때까지 30분 이상 기다려야 합니다. 

> [!IMPORTANT]
> 사용자 지정 학습을 프로비저닝하기 전에 테넌트 앱 카탈로그를 만들고 30분 이상 기다립니다. 이렇게 하면 SharePoint 내에서 앱 카탈로그 프로비저닝 프로세스가 완료됩니다. 