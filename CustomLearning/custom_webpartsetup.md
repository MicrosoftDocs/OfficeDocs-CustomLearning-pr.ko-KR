---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 사이트 구축
ms.date: 02/10/2019
description: SharePoint 프로 비전 엔진을 통해 Office 365 사이트에 대 한 사용자 지정 학습 프로 비전
ms.service: sharepoint online
ms.openlocfilehash: feebef7f351aab4cd1efe7f87596dad98dba7536
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233760"
---
# <a name="provision-custom-learning"></a>사용자 지정 학습 프로 비전

SharePoint Online 프로 비전 서비스를 사용 하 여 Office 365 테 넌 트 관리자는 몇 번의 간단한 클릭으로 프로 비전 프로세스를 시작할 수 있습니다. 구축 서비스는 사용자 지정 학습을 프로 비전 하는 데 권장 되는 방법입니다. 프로세스를 시작 하는 데 몇 분 정도 더 빠르고 간편 하 게 작업을 수행 합니다. 프로 비전 서비스를 시작 하기 전에 먼저 프로 비전을 위한 필수 구성 요소를 충족 했는지 확인 합니다.

## <a name="prerequisites"></a>필수 구성 요소
 
프로 비전 서비스 [SharePoint Online 프로 비전 서비스](https://provisioning.sharepointpnp.com)를 사용 하 여 사용자 지정 학습을 성공적으로 설정 하려면 프로 비전을 수행 하는 사람이 다음 사전 요구 사항을 충족 해야 합니다. 
 
- 사용자 지정 학습은 프로 비전 하는 테 넌 트의 테 넌 트 관리자 여야 합니다.  
- SharePoint 관리 센터의 앱 옵션 내에서 테 넌 트 앱 카탈로그를 사용할 수 있어야 합니다. 조직에 SharePoint 테 넌 트 앱 카탈로그가 없는 경우 [Sharepoint Online 문서](https://docs.microsoft.com/sharepoint/use-app-catalog) 를 참조 하 여 만듭니다.  
- 사용자 지정 학습은 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다. 사용자 지정 학습을 프로 비전 하는 사람이 앱 카탈로그의 사이트 모음 소유자가 아닌 경우에는 [이러한 지침을 완료](addappadmin.md) 하 고 계속 진행 합니다. 

### <a name="to-provision-custom-learning"></a>사용자 지정 학습을 프로 비전 하려면

1. http://provisioning.sharepointpnp.com홈 페이지의 오른쪽 위 모서리에서 이동 하 여 **로그인** 합니다.  사이트 서식 파일을 설치 하려는 대상 테 넌 트에 대 한 자격 증명으로 로그인 합니다.

![pnphome.png](media/inst_signin.png)

2. **조직 대신 동의** 를 지우고 **수락**을 선택 합니다.

![내](media/inst_perms.png)

3. 솔루션 갤러리에서 **Office 365에 대 한 사용자 지정 학습** 을 선택 합니다.

![내](media/inst_select.png)

4. 솔루션 홈 페이지에서 **테 넌 트에 추가를** 선택 합니다.

![inst_select.png](media/inst_add.png)

5. 설치에 적합한 프로비저닝 정보 페이지의 필드 입력을 완료합니다. 적어도 프로 비전 프로세스에 대 한 알림을 받을 전자 메일 주소와 사이트를 프로 비전 할 대상 URL을 입력 합니다.  
> [!NOTE]
> "/Sites/MyTraining" 또는 "/teams/LearnOffice365"과 같은 직원에 게 친숙 한 사이트의 대상 URL을 만듭니다.

![inst_options.png](media/inst_options.png)

6. 사용자 지정 학습을 테 넌 트 환경에 설치할 준비가 되 면 **프로 비전** 을 선택 합니다.  프로비저닝 프로세스는 최대 15분이 소요됩니다. 사이트에 액세스할 준비가 되면 이메일(프로비저닝 페이지에 입력한 알림 이메일 주소로)을 통해 알립니다.

> [!IMPORTANT]
> 사용자 지정 학습 사이트를 프로 비전 하는 테 넌 트 관리자는 해당 사이트로 이동한 다음 CustomLearningAdmin를 열어 사용자 지정 학습 관리 속성을 초기화 해야 합니다. 현재, 테 넌 트 관리자는 소유자를 사이트에도 할당 해야 합니다. 

## <a name="validate-provisioning-success"></a>구축 성공 유효성 검사

프로비저닝이 완료 되 면 테 넌 트 관리자가 PnP 프로 비전 서비스에서 전자 메일을 받습니다. 관리자는 전자 메일에 제공 된 사이트에 대 한 링크를 복사한 다음 지침에 따라 사이트로 이동할 수 있습니다. 또는 테 넌 트 관리자가/SitePages/CustomLearningAdmin.aspx.> 사이트 모음 URL <탐색할 수 있습니다. 이 명령은 처음 사용을 위해 사용자 지정 학습을 설정 하는 CustomConfig 목록 항목을 초기화 합니다. 이 페이지를 처음 여는 사용자가 테 넌 트 관리자, 사이트 모음 관리자 또는 사이트 소유자 여야 합니다. 다음과 같은 페이지가 표시 됩니다. 

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테 넌 트 관리자는 사이트를 사용자 지정 하는 사용자가 될 가능성은 없으며, 사이트에 소유자를 할당 해야 합니다. 소유자는 사이트 페이지를 수정 하 고 사이트를 다시 브랜딩 할 수 있도록 사이트에 대 한 관리 권한을 가집니다. 또한 사용자 지정 학습 웹 파트를 통해 제공 되는 콘텐츠를 숨기 거 나 표시 하는 기능도 제공 됩니다. 또한 사용자 지정 재생 목록을 작성 하 고 사용자 지정 하위 범주에 할당할 수 있습니다.  

1. SharePoint **설정** 메뉴에서 **사이트 사용 권한을**클릭 합니다.
2. **고급 사용 권한 설정을**클릭 합니다.
3. **Office 365 소유자에 대 한 사용자 지정 학습을**클릭 합니다.
4. **새로 만들기**  >  **사용자를이 그룹에 추가**를 클릭 하 고 소유자를 부여할 사용자를 추가한 다음 **공유**를 클릭 합니다.

8. 페이지 오른쪽 위 모서리에서 **다음** 옵션을 클릭 하 여 사이트를 따르세요.  

### <a name="next-steps"></a>다음 단계
- 웹 파트에 포함 된 [기본 콘텐츠](sitecontent.md) 를 살펴봅니다.
