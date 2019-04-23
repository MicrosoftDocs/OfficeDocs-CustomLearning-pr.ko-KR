---
author: karuanag
ms.author: karuanag
title: Office 365 솔루션에 대 한 사용자 지정 학습에 대 한 질문과 대답
ms.date: 02/10/2019
description: Office 365에 대 한 사용자 지정 학습에 대 한 질문과 대답 정보
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056012"
---
# <a name="frequently-asked-questions"></a>질문과 대답

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. Office 365에 대 한 사용자 지정 학습을 내 테 넌 트 환경에 설치 하기 위한 요구 사항은 무엇 인가요?

- SharePoint Online 및 통신 사이트를 사용 하도록 설정 합니다.
- CLO365을 프로 비전 할 개인은 설치 대상 테 넌 트의 테 넌 트 관리자 여야 합니다.
- SharePoint 관리 센터의 ' 앱 ' 옵션 내에서 테 넌 트 ' 앱 카탈로그 '를 사용할 수 있어야 합니다.
- CLO365을 프로 비전 할 개인은 설치를 위해 대상 테 넌 트의 앱 카탈로그에 대 한 사이트 모음 관리자 여야 합니다.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2 .에서 사용할 수 있는 Office 365에 대 한 사용자 지정 학습 언어는 무엇입니까?

Office 365에 대 한 사용자 지정 학습은 현재 영어로만 제공 됩니다. 자동 종단 간 프로비저닝을 영어 테 넌 트와 함께 작동 합니다. 향후 릴리스에서 추가 언어를 추가할 수 있습니다.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. 테 넌 트 환경에 사이트를 설치 하는 데 얼마나 걸립니까?

설치 테스트를 기반으로 15 분 미만 시간이 소요 됩니다. 여기에는 요구 사항에 맞게 사이트를 사용자 지정 하는 데 필요한 시간이 포함 되지 않습니다.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. Office 365에 대 한 사용자 지정 학습을 기본 SharePoint 사이트 모음의 하위 사이트를 만들 수 있나요?

아니요. 이 사이트는 항상 루트 사이트 모음으로 사용 되는 통신 사이트 서식 파일을 기반으로 합니다.

> [!NOTE]
> 최종 사용자가 사이트에 액세스 하는 데 필요한 사용 권한을 고려해 야 합니다. 대부분의 조직에서는 보안 또는 사용자 그룹을 정의 합니다. 직원 커뮤니티에 시작할 준비가 되 면 새 교육 포털에 적절 한 보안 그룹을 추가 해야 합니다.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. 사이트를 다시 설치 해야 합니다. 제가 뭘 해야 하나요?

[여기](custom_provision.md)에 게시 된 설치 지침을 따릅니다.

> [!NOTE]
> 이전 설치에서 원격 분석을 사용 하지 않도록 설정 했으며 원격 분석을 계속 사용 하지 않도록 설정 하려면 여기에서 원격 분석을 사용 하지 않도록 설정 하기 위한 지침을 따라야 합니다.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. Office 365에 대 한 사용자 지정 학습 구현을 업데이트 했습니다. 사이트를 다시 설치 하는 경우 이러한 업데이트 (사이트 서식 파일, 재생 목록)가 손실 됩니까?

현재 설치 된 사이트를 다시 설치 하면 개별 페이지 및 사용자 지정 재생 목록에 대 한 사용자 지정 내용이 손실 됩니다.  