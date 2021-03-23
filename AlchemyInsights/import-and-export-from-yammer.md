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
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="b1d69-102">Importação e exportação de Yammer</span><span class="sxs-lookup"><span data-stu-id="b1d69-102">Import and export from Yammer</span></span>

<span data-ttu-id="b1d69-103">**Importação**</span><span class="sxs-lookup"><span data-stu-id="b1d69-103">**Import**</span></span>

<span data-ttu-id="b1d69-104">As opções de importação de utilizadores variam consoante a sua rede Yammer esteja em [Modo Nativo para a Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), ou não.</span><span class="sxs-lookup"><span data-stu-id="b1d69-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="b1d69-105">**Modo Não Nativo**: Os utilizadores podem ser importados para grupos que usam [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limite para 100 utilizadores) dentro das definições do grupo, ou para a rede usando a [Atualização a granel](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) dentro do Administrador de Rede.</span><span class="sxs-lookup"><span data-stu-id="b1d69-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="b1d69-106">**Modo Nativo**: As operações de adesão ao grupo e de adesão à rede devem ser realizadas a partir do [portal de administração microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [portal AD Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), ou utilizando outra opção AD Azure.</span><span class="sxs-lookup"><span data-stu-id="b1d69-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="b1d69-107">As redes em Modo Nativo já não têm acesso a Bulk Update e outras funcionalidades antigas.</span><span class="sxs-lookup"><span data-stu-id="b1d69-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b1d69-108">A Yammer nunca apoiou a importação de conteúdos de dentro da Rede Administrador, mesmo quando a funcionalidade de Exportação de Dados foi utilizada noutra rede.</span><span class="sxs-lookup"><span data-stu-id="b1d69-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="b1d69-109">O conteúdo pode ser re-postado por soluções parceiras ou pelas APIs yammer REST.</span><span class="sxs-lookup"><span data-stu-id="b1d69-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="b1d69-110">**Exportação**</span><span class="sxs-lookup"><span data-stu-id="b1d69-110">**Export**</span></span>

<span data-ttu-id="b1d69-111">[Os dados da rede de exportação dentro da Rede Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permitem a exportação de conteúdos a partir de redes Yammer, incluindo mensagens e ficheiros.</span><span class="sxs-lookup"><span data-stu-id="b1d69-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="b1d69-112">Os anexos podem ser extremamente grandes e levarão as exportações a demorar um tempo significativo a concluir.</span><span class="sxs-lookup"><span data-stu-id="b1d69-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="b1d69-113">Recomendamos que as redes ativas sejam exportadas utilizando a [API de Exportação de Dados](https://developer.yammer.com/docs/data-export-api) em pedaços durante o dia ou a semana.</span><span class="sxs-lookup"><span data-stu-id="b1d69-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="b1d69-114">O Microsoft Support não fornece scripts personalizados para este fim.</span><span class="sxs-lookup"><span data-stu-id="b1d69-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="b1d69-115">Existe uma exportação separada [do RGPD](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) para exportar conteúdos para um utilizador individual.</span><span class="sxs-lookup"><span data-stu-id="b1d69-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>