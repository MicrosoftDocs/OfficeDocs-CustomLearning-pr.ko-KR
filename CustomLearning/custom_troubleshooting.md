---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 문제 해결
ms.date: 02/10/2019
description: 사용자 지정 학습 문제를 해결 하는 방법 알아보기
ms.openlocfilehash: 7cbd049d4794d14f9e8cc26fd0db5f444812d688
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055102"
---
# <a name="troubleshoot-custom-learning"></a>사용자 지정 학습 문제 해결

다음은 Office 365 또는 SharePoint Online 프로 비전 서비스에 대 한 사용자 지정 학습에서 발생할 수 있는 문제에 대 한 문제 해결 팁입니다.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>테 넌 트 관리 권한이 있는지 확인 하는 방법

SharePoint Online 프로 비전 서비스에 로그인 하 고 사용자 지정 학습용 프로 비전에는 테 넌 트 관리자 권한이 필요 합니다. SharePoint Online 프로 비전 서비스에 로그인 하는 동안 문제가 발생 하는 경우 전역 관리자 역할이 할당 되었는지 확인 합니다. 사용자 지정 학습 솔루션에는 테 넌 트 관리 권한 (Office 365 전역 관리자 역할 이라고 함)이 필요 합니다. 전역 관리자 역할이 할당 되었는지 확인 하는 방법은 다음과 같습니다.

1.  Office.com에 로그인 합니다.
2.  **관리** 클릭
3.  **사용자**에서 **활성 사용자** 를 선택 합니다.
4.  사용자 이름 검색
5.  검색 결과에서 사용자의 이름을 클릭 합니다. 전역 관리자가 역할에 대 한 것을 볼 수 있습니다.

![cg-globaladminrole-.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>전역 관리자 역할이 없는 경우
- 조직에서 전역 관리자를 찾아서 해당 사용자가 서비스에 로그인 하거나 전역 관리자 역할을 할당 하도록 합니다.

## <a name="tenant-app-catalog-troubleshooting"></a>테 넌 트 앱 카탈로그 문제 해결
사용자 지정 학습을 수행 하려면 대상 테 넌 트에서 앱 카탈로그를 프로 비전 해야 합니다. 앱 카탈로그를 만들려면 전역 관리자 권한이 필요 합니다. 다음은 일반적인 앱 카탈로그 문제에 대 한 문제 해결 단계입니다.

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>테 넌 트 앱 카탈로그가 있는지 여부를 확인 하는 방법 
초보자에 게 전역 관리자 권한이 있는지 확인 합니다. 위의 테 넌 트 관리 권한 단계를 참조 하세요.

1. Office 365에서 **관리**, 확장 화살표 >를 차례로 클릭 하 고 **모든** > **관리 센터** > **SharePoint**표시를 클릭 합니다.
2. **클래식 관리 SharePoint Center** > **apps** > **앱 카탈로그**를 클릭 합니다.
3. **앱**에는 **SharePoint 용 앱 배포**라는 타일이 표시 됩니다. 타일이 표시 되 면 테 넌 트 앱 카탈로그가 있습니다. 아래에서 **사이트 Colllection를 확인 하는 방법을** 참조 하십시오. 타일이 표시 되지 않는 경우 테 넌 트에 대 한 테 넌 트 앱 카탈로그를 만들어야 합니다. 아래에서 **테 넌 트 앱 카탈로그를 만드는 방법** 섹션을 참조 하세요.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>사용자가 테 넌 트 앱 카탈로그의 사이트 모음 소유자 인지 확인 하는 방법 
Office 365에 대 한 사용자 지정 학습을 프로 비전 하려면 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다. 소유자 인 경우에는 다음과 같은 방법으로 determin.

1. Office 365에서 **관리**, 확장 화살표 >를 차례로 클릭 하 고 **모든** > **관리 센터** > **SharePoint**표시를 클릭 합니다.
2. **클래식 관리 SharePoint 센터**를 클릭 하 고 **앱 카탈로그**를 선택 합니다.
3. **소유자**를 선택 하 고 사용자가 사이트 모음 소유자 인지 확인 합니다. 다음과 같이 표시 됩니다.
 
![cg-sitecollectionowner-.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>테 넌 트 앱 카탈로그가 없는 경우 만드는 방법 
1. SharePoint Online 관리자 계정을 사용 하 여 Office 365에 로그인 합니다.
2. **관리자**를 클릭합니다.
3. **관리 센터**에서 **SharePoint**를 클릭 합니다. 
4. **앱** > **앱 카탈로그**를 클릭 합니다.
5. **새 앱 카탈로그 사이트 만들기**를 클릭 한 다음 **확인**을 클릭 합니다. 
6.  앱 카탈로그에 대 한 정보를 입력 합니다. 관리자를 두 명 이상 포함할 수 있습니다. 다음은 예제를 보여 줍니다.  

![cg-appcatalogfinish-.png](media/cg-appcatalogfinish.png)

7.  그거에요. 완료 되었습니다. 하지만 사용자 지정 학습 프로 비전으로 이동 하기 전에 30 분 이상 기다려야 앱 카탈로그 만들기가 완료 되었는지 확인 해야 합니다. 

> [!IMPORTANT]
> 사용자 지정 학습을 프로 비전 하기 전에 테 넌 트 앱 카탈로그를 만든 후 30 분 이상 기다립니다. 이렇게 하면 SharePoint 내에서 앱 카탈로그 프로 비전 프로세스가 완료 됩니다. 