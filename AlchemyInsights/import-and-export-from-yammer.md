---
title: Importação e exportação de Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037262"
---
# <a name="import-and-export-from-yammer"></a>Importação e exportação de Yammer

**Importação**

As opções de importação de utilizadores variam consoante a sua rede Yammer esteja em [Modo Nativo para a Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), ou não.

- **Modo Não Nativo**: Os utilizadores podem ser importados para grupos que usam [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limite para 100 utilizadores) dentro das definições do grupo, ou para a rede usando a [Atualização a granel](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) dentro do Administrador de Rede.
- **Modo Nativo**: As operações de adesão ao grupo e de adesão à rede devem ser realizadas a partir do [portal de administração microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [portal AD Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), ou utilizando outra opção AD Azure. As redes em Modo Nativo já não têm acesso a Bulk Update e outras funcionalidades antigas.

> [!IMPORTANT]
> A Yammer nunca apoiou a importação de conteúdos de dentro da Rede Administrador, mesmo quando a funcionalidade de Exportação de Dados foi utilizada noutra rede. O conteúdo pode ser re-postado por soluções parceiras ou pelas APIs yammer REST.

**Exportação**

[Os dados da rede de exportação dentro da Rede Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permitem a exportação de conteúdos a partir de redes Yammer, incluindo mensagens e ficheiros. Os anexos podem ser extremamente grandes e levarão as exportações a demorar um tempo significativo a concluir. Recomendamos que as redes ativas sejam exportadas utilizando a [API de Exportação de Dados](https://developer.yammer.com/docs/data-export-api) em pedaços durante o dia ou a semana. O Microsoft Support não fornece scripts personalizados para este fim.

Existe uma exportação separada [do RGPD](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) para exportar conteúdos para um utilizador individual.