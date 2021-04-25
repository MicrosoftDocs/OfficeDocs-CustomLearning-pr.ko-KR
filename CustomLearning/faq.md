---
title: Microsoft 365 학습 경로 FAQ
author: karuanag
ms.author: karuanag
ms.date: 02/10/2019
description: Microsoft 365 학습 경로에 대한 질문과 대답 정보
ms.service: sharepoint-online
ms.openlocfilehash: d91c2710315b393eb8be3645c4fa94b32d353aa7
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000084"
---
# <a name="frequently-asked-questions"></a>자주 묻는 질문

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>최근에 Office 365용 사용자 지정 학습이 Microsoft 365 학습 경로로 이름을 지정하는 블로그 게시물을 보했습니다. 이름 변경의 일환으로 솔루션에 추가되는 다른 변경 사항이 있나요? 조직에서 솔루션을 업데이트해야 하나요?

Microsoft 365 학습 경로 릴리스는 Microsoft 365 브랜디드에 맞게 솔루션 이름을 변경하는 데 전념하는 브랜드 변경입니다. 현재 조직에서 Office 365용 사용자 지정 학습이 성공적으로 실행되고 있는 경우 현재 솔루션을 업데이트할 필요가 없습니다.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>테넌트 환경에 Microsoft 365 학습 경로를 설치하기 위한 요구 사항은 무엇입니까?

- SharePoint Online 및 커뮤니케이션 사이트를 사용할 수 있습니다.
- CLO365를 프로비전할 개인은 설치할 대상 테넌트의 테넌트 관리자 되어야 합니다.
- '앱 카탈로그' 테넌트는 SharePoint 관리 센터의 '앱' 옵션 내에서 사용할 수 있어야 합니다.
- 새 앱 카탈로그를 만들 경우 앱 카탈로그를 완전히 프로비전하려면 30분 이상의 대기 시간이 필요합니다. 테넌트 앱 카탈로그를 만드는 직후 Microsoft 365 학습 경로를 프로비전하려고 하면 학습 경로 솔루션의 프로비전 오류가 발생합니다. 
- CLO365를 프로비전할 개인은 설치할 대상 테넌트에서 앱 카탈로그의 사이트 모음 관리자 되어야 합니다.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Microsoft가 Microsoft 365 학습 경로를 설치할 때 테넌트 권한을 요청하는 이유 

- SharePoint Online 프로비저닝 서비스는 사용 권한을 사용하여 학습 경로 SharePoint 사이트를 프로비전하고, 사이트의 페이지를 만들고, 테넌트 내에 Microsoft 365 학습 경로 응용 프로그램을 설치합니다. 그 이유는 사용 권한을 요청하는 유일한 이유입니다. 요청된 사용 권한이 없는 경우 SharePoint 프로비전 서비스는 학습 경로 사이트 서식 파일 및 웹 파트를 자동으로 설치하는 명령을 실행할 수 없습니다. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>베타 미리 보기에서 Microsoft 365 학습 경로의 의미는 무엇입니까? 

Microsoft 365 학습 경로는 현재 베타 미리 보기에 있습니다. Microsoft 365 학습 경로를 평가, 계획 및 구현할 때 다음을 고려합니다.

- 모든 베타 솔루션과 함께 서비스 관리 팀은 서비스 및 해당 구성 요소를 변경할 수 있는 권리가 있습니다. 버그 및 UX 문제를 적극적으로 해결하고 있는 경우 WebPart를 업데이트해야 할 수 있습니다.
- 웹 파트를 업데이트하려면 GitHub 리포지토리에서 웹 파트를 다운로드하여 테넌트 앱 카탈로그에 업로드해야 합니다. Microsoft 365 학습 경로 읽기 파일의 "솔루션 업데이트" [섹션을 참조하세요.](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Microsoft 365 학습 경로를 사용할 수 있는 언어는 무엇입니까?

Microsoft 365 학습 경로는 현재 영어로만 제공됩니다. 자동 종단-종단 프로비전은 영어 테넌트에서만 작동합니다. 2020년 2분기에는 다음 언어에 대한 다국어 지원을 롤아웃할 계획입니다. 

- 중국어(간체) 
- 프랑스어  
- 독일어 
- 이탈리아어(이탈리아) 
- 일본어(일본)  
- 포르투갈어(브라질) 
- 러시아어(러시아어)  
- 스페인어 

> 다가오는 학습 경로에 대한 다국어 지원 릴리스에는 네덜란드어 지원이 포함되지 않습니다. 향후에도 새로운 언어 옵션을 평가할 예정입니다.

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>테넌트 환경에 사이트를 설치하는 데 시간이 얼마나 걸릴까요?

설치 테스트에 따라 15분 미만이 걸립니다. 여기에는 요구 사항에 맞게 사이트를 사용자 지정하는 데 필요한 시간은 포함되지 않습니다.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 학습 경로가 오픈 소스 솔루션인가요? 그 의미는 무엇입니까?

Microsoft 365 학습 경로는 OSS(오픈 소스 소프트웨어) 솔루션으로, OSS에 다양한 이점과 고려 사항을 제공합니다.

#### <a name="benefits"></a>이점 
- **Microsoft 365 학습 경로는 무료 솔루션입니다.** 고객은 테넌트에 솔루션을 설치하고, 솔루션을 사용자 지정하고, 최종 사용자가 사용할 수 있도록 할 수 있습니다.
- **OSS를 사용하면 신속한 개발 및 공동 작업을 가능하게 합니다.**  모든 오픈 소스 솔루션은 광범위한 참가자 커뮤니티에서 사용할 수 있습니다.  Microsoft는 이러한 혁신을 추진하기 위해 최선을 다하고 있습니다.  핵심 서비스 관리 팀은 가장 광범위한 고객에게 혜택을 제공하는 환경을 제공하도록 보장하기 위해 공식 빌드에 병합되는 기여를 결정할 수 있는 권리가 있습니다.  
- **OSS를 사용하면 파트너와 공동 작업을 할 수 있습니다.** Microsoft는 여러 학습 파트너와 협력하여 향후 Microsoft 365 학습 경로에 대한 노력과 기여를 지원하고 있습니다. 이러한 계획이 마무리될 때 추가 정보를 제공할 것입니다. 
    
#### <a name="implications"></a>의미
- **OSS는 상업용 제품이 아니며,** 상업용 제품에는 업데이트 및 패치가 포함되고 유료 지원 계약에 포함됩니다. Microsoft는 현재 Microsoft 365 학습 경로에 대한 설명서, 업데이트 및 패치를 제공하면서 이러한 특정 비즈니스 시나리오를 개선하기 위한 노력의 기반이 됩니다. 당사의 계획은 학습 경로에 계속 투자할 계획입니다. 서비스 관리 팀은 향후 전략을 변경할 수 있습니다. Microsoft 365 학습 경로에 대한 향후 변경 사항은 적용에 앞서 전달됩니다. 
- **OSS로 Microsoft 365** 학습 경로는 GitHub의 온라인 문제 목록을 통해 지원됩니다. Microsoft 365 학습 경로는 기존 Microsoft 지원 계약에 적용되지 않습니다. 제출된 문제는 Microsoft 365 학습 경로 서비스 소유자 및 커뮤니티에서 검토합니다. 문제 해결 서비스 수준은 유료 Microsoft 지원 계약과 수준이 동일하지 않습니다.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Microsoft 365 학습 경로를 기본 SharePoint 사이트 모음의 하위 사이트로 만들 수 있나요?

아니요. 이 사이트는 항상 루트 사이트 모음인 커뮤니케이션 사이트 서식 파일을 기반으로 합니다.

> [!NOTE]
> 최종 사용자가 사이트에 액세스하는 데 필요한 사용 권한을 고려해야 합니다. 대부분의 조직에서는 보안 또는 사용자 그룹을 정의했습니다. 직원 커뮤니티에 시작할 준비가 된 후 새 교육 포털에 적절한 보안 그룹을 추가해야 합니다.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>사이트를 다시 설치해야 합니다. 제가 뭘 해야 하나요?

여기에 게시된 설치 지침을 [따릅니다.](custom_provision.md)

> [!NOTE]
> 이전 설치에서 원격 분석 기능을 사용하지 않도록 설정한 경우 원격 분석 사용 안 을 계속하려면 여기에서 원격 분석 비활성화 지침을 따라야 합니다.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Microsoft 365 학습 경로 구현을 업데이트했습니다. 사이트를 다시 설치하면 이러한 업데이트(사이트 서식 파일, 재생 목록에 적용)가 손실될 수 있나요?

현재 설치를 통해 사이트를 다시 설치하면 개별 페이지 및 사용자 지정 재생 목록의 사용자 지정이 손실됩니다.  
