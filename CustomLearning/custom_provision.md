---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 사이트 구축
ms.date: 02/10/2019
description: SharePoint 프로 비전 엔진을 통해 Office 365 사이트에 대 한 사용자 지정 학습 프로 비전
ms.openlocfilehash: 868708f9f096c84d5ebc5f9bc4e21e558da84d2b
ms.sourcegitcommit: 5ea8d7fdc255ef7de06f41b3c794bc40551cf5bb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30577864"
---
# <a name="provision-custom-learning"></a>사용자 지정 학습 프로 비전 

SharePoint Online 프로 비전 서비스를 사용 하 여 Office 365 테 넌 트 관리자는 몇 번의 간단한 클릭으로 프로 비전 프로세스를 시작할 수 있습니다. 구축 서비스는 사용자 지정 학습을 프로 비전 하는 데 권장 되는 방법입니다. 프로세스를 시작 하는 데 몇 분 정도 더 빠르고 간편 하 게 작업을 수행 합니다. 프로 비전 서비스를 시작 하기 전에 먼저 프로 비전을 위한 필수 구성 요소를 충족 했는지 확인 합니다.

## <a name="prerequisites"></a>필수 구성 요소
 
프로 비전 서비스를 사용 하 여 사용자 지정 학습을 성공적으로 설정 하려면 프로 비전을 수행 하는 사람이 다음 사전 요구 사항을 충족 해야 합니다. 
 
- 사용자 지정 학습을 프로 비전 하는 사람은 사용자 지정 학습을 구축할 테 넌 트의 테 넌 트 관리자 여야 합니다.  
- SharePoint 관리 센터의 앱 옵션 내에서 테 넌 트 앱 카탈로그를 사용할 수 있어야 합니다. 조직에 sharepoint 테 넌 트 앱 카탈로그가 없는 경우 [sharepoint Online 문서](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) 를 참조 하 여 만듭니다.  
- 사용자 지정 학습은 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다. 사용자 지정 학습을 프로 비전 하는 사람이 앱 카탈로그의 사이트 모음 소유자가 아닌 경우에는 [이러한 지침을 완료](addappadmin.md) 하 고 계속 진행 합니다. 

### <a name="to-provision-custom-learning"></a>사용자 지정 학습을 프로 비전 하려면

1. http://provisioning.sharepointpnp.com 홈 페이지의 오른쪽 위 모서리에서 이동 하 여 **로그인** 합니다.  사이트 서식 파일을 설치 하려는 대상 테 넌 트에 대 한 자격 증명으로 로그인 합니다.

![pnphome-.png](media/inst_signin.png)

2. **조직 대신 동의** 를 지우고 **수락**을 선택 합니다.

![내](media/inst_perms.png)

3. 페이지를 아래로 스크롤하여 **솔루션** 탭을 선택한 다음 **Office 365에 대 한 사용자 지정 학습**을 선택 합니다. 

![내](media/inst_select.png)

4. **테 넌 트에 추가를 선택 합니다** .

![inst_select-.png](media/inst_add.png)

5. 설치에 적합 하도록 프로 비전 정보 페이지의 필드를 완성 합니다. 적어도 프로 비전 프로세스에 대 한 알림을 받을 전자 메일 주소와 사이트를 프로 비전 할 대상 URL을 입력 합니다.  
> [!NOTE]
> "/sites/MyTraining" 또는 "/teams/LearnOffice365"과 같은 직원에 게 친숙 한 사이트의 대상 URL을 만듭니다.

![inst_options-.png](media/inst_options.png)

6. 사용자 지정 학습을 테 넌 트 환경에 설치할 준비가 되 면 **프로 비전** 을 선택 합니다.  구축 프로세스는 최대 15 분까지 소요 됩니다. 사이트에 액세스할 준비가 되 면 프로 비전 페이지에서 입력 한 알림 전자 메일 주소로 전자 메일을 통해 알림 메시지가 표시 됩니다. 

> [!IMPORTANT]
> 사용자 지정 학습 사이트를 프로 비전 하는 테 넌 트 관리자는 해당 사이트로 이동한 다음 **CustomLearningAdmin** 를 열어 사용자 지정 학습 관리 속성을 초기화 해야 합니다. 현재, 테 넌 트 관리자는 소유자를 사이트에도 할당 해야 합니다. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>프로 비전 성공 유효성 검사 및 customconfig 목록 초기화

프로비저닝이 완료 되 면 사이트를 프로 비전 한 테 넌 트 관리자가 PnP 프로 비전 서비스에서 전자 메일을 받습니다. 전자 메일에 사이트에 대 한 링크가 포함 되어 있습니다. 이때 테 넌 트 관리자는 전자 메일에 제공 된 링크를 사용 하 여 사이트에 방문 하 고 처음 사용할 수 있도록 사이트를 설정 해야 합니다.

- `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`으로 이동합니다. **CustomLearningAdmin** 를 열면 처음 사용할 사용자 지정 학습을 설정 하는 **customconfig** 목록 항목이 초기화 됩니다. 다음과 같은 페이지가 표시 됩니다.

![cg-adminapppage-.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>사이트에 소유자 추가
테 넌 트 관리자는 사이트를 사용자 지정 하는 사용자가 될 가능성은 없으며, 사이트에 소수의 소유자를 할당 해야 합니다. 소유자는 사이트 페이지를 수정 하 고 사이트를 다시 브랜딩 할 수 있도록 사이트에 대 한 관리 권한을 가집니다. 또한 사용자 지정 학습 웹 파트를 통해 제공 되는 콘텐츠를 숨기 거 나 표시 하는 기능도 제공 됩니다. 또한 사용자 지정 재생 목록을 작성 하 고 사용자 지정 하위 범주에 할당할 수 있습니다.  

1. SharePoint **설정** 메뉴에서 **사이트 사용 권한을**클릭 합니다.
2. **고급 사용 권한 설정을**클릭 합니다.
3. **Office 365 소유자에 대 한 사용자 지정 학습을**클릭 합니다.
4. **새로 만들기** > **사용자를이 그룹에 추가**를 클릭 한 다음 소유자가 하려는 사용자를 추가 합니다. 
5. 링크를 추가 하 여 공유 메시지에서 [사이트를 탐색](custom_exploresite.md) 하 고 **공유**를 클릭 합니다.

### <a name="next-steps"></a>다음 단계
- 사이트 및 웹 파트에서 제공 되는 [기본 콘텐츠](custom_exploresite.md) 를 살펴봅니다.
