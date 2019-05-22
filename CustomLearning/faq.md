---
author: karuanag
ms.author: karuanag
title: Microsoft 365 학습 경로에 대 한 질문과 대답
ms.date: 02/10/2019
description: Microsoft 365 학습 경로에 대 한 질문과 대답 정보
ms.openlocfilehash: 26d6c7140b4d387e13b907033ea53b752f5e20ea
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334722"
---
# <a name="frequently-asked-questions"></a>질문과 대답

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>내 테 넌 트 환경에 Microsoft 365 학습 경로를 설치 하기 위한 요구 사항은 무엇 인가요?

- SharePoint Online 및 통신 사이트를 사용 하도록 설정 합니다.
- CLO365을 프로 비전 할 개인은 설치 대상 테 넌 트의 테 넌 트 관리자 여야 합니다.
- SharePoint 관리 센터의 ' 앱 ' 옵션 내에서 테 넌 트 ' 앱 카탈로그 '를 사용할 수 있어야 합니다.
- 새 앱 카탈로그를 만든 경우 앱 카탈로그를 완전히 프로 비전 하려면 대기 시간이 30 분 이상 이어야 합니다. 테 넌 트 앱 카탈로그를 만든 후 Microsoft 365 학습 경로를 직접 프로 비전 하려고 하면 학습 경로 솔루션의 프로 비전 오류가 발생 합니다. 
- CLO365을 프로 비전 할 개인은 설치를 위해 대상 테 넌 트의 앱 카탈로그에 대 한 사이트 모음 관리자 여야 합니다.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Microsoft 365 학습 경로를 설치할 때 Microsoft에서 테 넌 트 권한을 요구 하는 이유 

- SharePoint Online 프로 비전 서비스는 사용 권한을 사용 하 여 학습 경로 SharePoint 사이트를 프로 비전 하 고, 사이트의 페이지를 만들고, 테 넌 트 내에서 Microsoft 365 Learning 경로 응용 프로그램을 설치 합니다. 이는 사용 권한을 요청 하는 유일한 이유입니다. 요청 된 사용 권한이 없으면 SharePoint 프로 비전 서비스가 학습 경로 사이트 서식 파일 및 웹 파트를 자동으로 설치 하는 명령을 실행할 수 없습니다. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>베타 미리 보기에 있는 Microsoft 365 학습 경로의 의미는 무엇 인가요? 

Microsoft 365 학습 경로는 현재 베타 미리 보기 상태입니다. Microsoft 365 학습 경로를 평가, 계획 및 구현 하는 경우 다음 사항을 고려 하세요.

- 모든 베타 솔루션과 마찬가지로 서비스 관리 팀은 서비스 및 해당 구성 요소를 변경할 수 있는 권한을 보유 합니다. 버그 및 UX 문제를 적극적으로 해결할 때 웹 파트를 업데이트 해야 할 수 있습니다.
- 웹 파트를 업데이트 하려면 GitHub 리포지토리에서 다운로드 하 여 테 넌 트 앱 카탈로그에 업로드 해야 합니다. Microsoft 365 학습용 경로 [추가 정보](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) 파일의 "솔루션 업데이트" 섹션을 참조 하세요. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Microsoft 365 학습 경로는 어떤 언어로 제공 됩니까?

Microsoft 365 학습 경로는 현재 영어로만 제공 됩니다. 자동 종단 간 프로비저닝을 영어 테 넌 트와 함께 작동 합니다. CY19 Q3에서는 다음과 같은 9 가지 언어에 대 한 다국어 지원을 배포 하는 방법을 계획 하 고 있습니다. 

- 중국어(간체) 
- 네덜란드어(네덜란드) 
- 프랑스어  
- 독일어 
- 이탈리아어(이탈리아) 
- 일본어 (일본)  
- 포르투갈어 (브라질) 
- 러시아어 (러시아어)  
- 스페인어 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>테 넌 트 환경에 사이트를 설치 하는 데 소요 되는 시간이 얼마나 걸립니까?

설치 테스트를 기반으로 15 분 미만 시간이 소요 됩니다. 여기에는 요구 사항에 맞게 사이트를 사용자 지정 하는 데 필요한 시간이 포함 되지 않습니다.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 학습 경로는 오픈 소스 솔루션 이며 의미는 무엇 인가요?

Microsoft 365 학습 경로는 oss (Open Source Software) 솔루션이 며, 이러한 솔루션은 germane에 따라 혜택 및 고려 사항 집합을 제공 합니다.

#### <a name="benefits"></a>이점 
- **Microsoft 365 학습 경로는 무료 솔루션입니다.** 고객은 테 넌 트에서 솔루션을 설치 하 고, 사용자 지정 하 여 최종 사용자가 사용할 수 있도록 합니다.
- **OSS를 사용 하면 신속한 개발과 공동 작업을 수행할 수 있습니다.**  모든 오픈 소스 솔루션은 다양 한 참가자 커뮤니티에서 사용할 수 있습니다.  Microsoft는 혁신을 추진 하는이 방법에 최선을 다하고 있습니다.  고객의 가장 넓은 집합에 도움이 되는 환경을 제공 하기 위해 핵심 서비스 관리 팀은 공식 빌드로 병합 되는 기고 물을 결정 하기 위한 권한을 예약 합니다.  
- **OSS를 사용 하 여 파트너와 공동 작업을 수행할 수 있습니다.** Microsoft는 Microsoft 365 학습 경로에 대 한 향후 확장 및 기고를 지원 하기 위해 몇 가지 학습 파트너와 협력 하 고 있습니다. 이러한 요금제가 종료 될 때 추가 정보를 제공 합니다. 
    
#### <a name="implications"></a>상당한
- **OSS는 상업적으로 사용할 수 없는 제품입니다.** 상용 제품에는 업데이트 및 패치가 포함 되며 유료 지원 계약에 포함 됩니다. 현재 Microsoft에서 제공 하는 microsoft 365 학습 경로에 대 한 설명서, 업데이트 및 패치는 이러한 특정 비즈니스 시나리오를 개선 하기 위한 노력을 기반으로 합니다. 이 계획은 학습 경로에 계속 투자 하는 것 이지만 고객은 서비스 관리 팀이 향후 전략을 변경할 수 있다는 점을 염두에 두어야 합니다. 이후에 Microsoft 365 학습 경로에 대 한 변경 내용이 적용 되기 전에 전달 됩니다. 
- **OSS에서 microsoft 365 학습 경로는 GitHub의 온라인 문제 목록을 통해 지원 되며**microsoft 365 learning 경로는 기존 microsoft 지원 계약에 포함 되지 않습니다. 제출 된 문제는 Microsoft 365 learning 경로 서비스 소유자 및 커뮤니티에서 심사 됩니다. 문제 해결 서비스 수준은 유료 Microsoft 지원 계약과는 수준이 다릅니다.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Microsoft 365 학습 경로를 기본 SharePoint 사이트 모음의 하위 사이트를 만들 수 있나요?

아니요. 이 사이트는 항상 루트 사이트 모음으로 사용 되는 통신 사이트 서식 파일을 기반으로 합니다.

> [!NOTE]
> 최종 사용자가 사이트에 액세스 하는 데 필요한 사용 권한을 고려해 야 합니다. 대부분의 조직에서는 보안 또는 사용자 그룹을 정의 합니다. 직원 커뮤니티에 시작할 준비가 되 면 새 교육 포털에 적절 한 보안 그룹을 추가 해야 합니다.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>사이트를 다시 설치 해야 합니다. 제가 뭘 해야 하나요?

[여기](custom_provision.md)에 게시 된 설치 지침을 따릅니다.

> [!NOTE]
> 이전 설치에서 원격 분석을 사용 하지 않도록 설정 했으며 원격 분석을 계속 사용 하지 않도록 설정 하려면 여기에서 원격 분석을 사용 하지 않도록 설정 하기 위한 지침을 따라야 합니다.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Microsoft 365 학습 경로 구현에 대 한 업데이트를 수행 했습니다. 사이트를 다시 설치 하는 경우 이러한 업데이트 (사이트 서식 파일, 재생 목록)가 손실 됩니까?

현재 설치 된 사이트를 다시 설치 하면 개별 페이지 및 사용자 지정 재생 목록에 대 한 사용자 지정 내용이 손실 됩니다.  