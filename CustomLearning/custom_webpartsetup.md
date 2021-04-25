---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 사이트 프로비전
ms.date: 02/10/2019
description: SharePoint 프로비전 엔진을 통해 Office 365용 사용자 지정 학습 사이트 프로비전
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: f930eba5815366bcefd2730c88a3c2df3f246dd4
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000324"
---
# <a name="provision-custom-learning"></a>사용자 지정 학습 프로비전

SharePoint Online 프로비저닝 서비스를 사용하여 Office 365 테넌트 관리자는 몇 번의 클릭으로 프로비저닝 프로세스를 시작할 수 있습니다. 프로비저닝 서비스는 사용자 지정 학습을 프로비전하는 권장 방법입니다. 빠르고 쉬우며 프로세스를 시작하는 데 몇 분 정도 걸립니다. 그러나 프로비저닝 서비스를 시작하기 전에 프로비전을 위한 선행 준비를 충족해야 합니다.

## <a name="prerequisites"></a>필수 구성 요소
 
프로비저닝 서비스 [SharePoint Online 프로비전](https://provisioning.sharepointpnp.com)서비스를 사용하여 사용자 지정 학습을 성공적으로 설정하려면 프로비저닝을 수행한 사람이 다음의 선행 요구 사항을 충족해야 합니다. 
 
- 사용자 지정 학습을 프로비전하는 사람은 사용자 지정 학습을 프로비전할 테넌트의 테넌트 관리자 되어야 합니다.  
- 테넌트 앱 카탈로그는 SharePoint 관리 센터의 앱 옵션 내에서 사용할 수 있어야 합니다. 조직에 SharePoint 테넌트 앱 카탈로그가 없는 경우 [SharePoint Online](/sharepoint/use-app-catalog) 설명서를 참조하여 만들 수 있습니다.  
- 사용자 지정 학습을 프로비저닝하는 사람은 테넌트 앱 카탈로그의 사이트 모음 소유자가 되어야 합니다. 사용자 지정 학습을 프로비저닝하는 사용자가 앱 카탈로그의 사이트 모음 소유자가 아닌 경우 [이러한 지침을 완료하고](addappadmin.md) 계속합니다. 

### <a name="to-provision-custom-learning"></a>사용자 지정 학습을 프로비전하기 위해

1. 으로 http://provisioning.sharepointpnp.com **이동하여 홈 페이지의** 오른쪽 위 모서리에서 로그인합니다.  사이트 서식 파일을 설치할 대상 테넌트의 자격 증명으로 로그인합니다.
![프로비저닝 서비스 기본 페이지.](media/inst_signin.png)

2. 조직을 대신하여 동의를 **지우고** 수락 을 **선택합니다.**
![동의 화면](media/inst_perms.png)

3. 솔루션 **갤러리에서 Office 365용** 사용자 지정 학습을 선택합니다.
![Office 365용 사용자 지정 학습을 선택하는 화면입니다.](media/inst_select.png)

4. 솔루션 홈 페이지에서 테넌트에 추가를 선택하는 테넌트 화면에  
 ![ 추가를 선택합니다.](media/inst_add.png)

5. 설치에 적합한 프로비저닝 정보 페이지의 필드 입력을 완료합니다. 최소한 프로비저닝 프로세스에 대한 알림을 받을 전자 메일 주소와 프로비전할 사이트의 대상 URL을 입력합니다.  
   > [!NOTE]
   > "/sites/MyTraining" 또는 "/teams/LearnOffice365" 등 직원에게 친숙한 사이트의 대상 URL을 만드세요.

   ![프로비저닝 세부 정보를 제공하는 화면입니다.](media/inst_options.png)

6. **테넌트** 환경에 사용자 지정 학습을 설치할 준비가 되면 프로비전을 선택합니다.  프로비저닝 프로세스는 최대 15분이 소요됩니다. 사이트에 액세스할 준비가 되면 이메일(프로비저닝 페이지에 입력한 알림 이메일 주소로)을 통해 알립니다.

> [!IMPORTANT]
> 사용자 지정 학습 사이트를 프로비전하는 테넌트 관리자는 사이트로 이동한 다음 CustomLearningAdmin.aspx를 열어 사용자 지정 학습 관리 속성을 초기화해야 합니다. 이때 테넌트 관리자는 소유자를 사이트에 할당해야 합니다. 

## <a name="validate-provisioning-success"></a>프로비저닝 성공 유효성 검사

프로비전이 완료되면 테넌트 관리자가 PnP 프로비전 서비스에서 전자 메일을 수신합니다. 관리자는 전자 메일에 제공된 사이트에 대한 링크를 복사한 다음 지침에 따라 사이트로 이동하면 됩니다. 또는 테넌트 관리자는 YOUR-SITE-COLLECTION-URL </SitePages/CustomLearningAdmin.aspx>탐색할 수 있습니다. 이렇게 하면 처음 사용할 때 사용자 지정 학습을 설정하는 CustomConfig 목록 항목이 초기화됩니다. 이 페이지를 처음 여는 사람은 테넌트 관리자, 사이트 모음 관리자 또는 사이트 소유자입니다. 다음과 같은 페이지가 표시됩니다. 

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테넌트 관리자는 사이트를 사용자 지정하는 사람이 될 가능성이 낮기 때문에 사이트에 소유자를 할당해야 합니다. 소유자는 사이트에 대한 관리 권한이 있으므로 사이트 페이지를 수정하고 사이트를 다시 브랜드할 수 있습니다. 또한 사용자 지정 학습 웹 파트를 통해 제공된 콘텐츠를 숨기고 표시하는 기능을 제공합니다. 또한 사용자 지정 재생 목록을 빌드하고 사용자 지정 하위 목록에 할당하는 기능을 사용할 수 있습니다.  

1. SharePoint **설정 메뉴에서** 사이트 **사용 권한 을 클릭합니다.**
2. 고급 **사용 권한 설정을 클릭합니다.**
3. **Office 365 소유자에** 대한 사용자 지정 학습을 클릭합니다.
4. 이 **그룹에 새** 사용자  >  **추가를 클릭하고** 소유자가 될 사용자를 추가한 다음 공유를 **클릭합니다.**

8. 페이지 오른쪽 **위** 모서리에서 다음 옵션을 클릭하여 사이트를 팔로우합니다.  
