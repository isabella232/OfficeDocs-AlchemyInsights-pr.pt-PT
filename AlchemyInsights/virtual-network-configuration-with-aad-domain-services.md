---
title: Configuração virtual com serviços de domínio AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885646"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Configuração virtual com serviços de domínio AAD

A configuração virtual com os serviços de domínio AAD envolve os seguintes passos: 

1. Verificar a saúde do seu domínio no portal Azure https://aka.ms/aadds-health
2. Verificando o seu NSG por regras que bloqueiam portas necessárias para sincronizar em Azure AD Domain Services no portal https://aka.ms/aadds-networking
3. Certificando-se de que a sua rede virtual é implantada na mesma Região Azure que o seu domínio gerido pelos Serviços de Domínio AZure AD.
4. Garantindo que não tem um domínio existente com o mesmo nome de domínio disponível na rede virtual.

Para obter mais detalhes sobre a consideração de design na Rede Virtual Azure para apoiar os serviços de domínio AAD, consulte [Adyssed de Rede Virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

