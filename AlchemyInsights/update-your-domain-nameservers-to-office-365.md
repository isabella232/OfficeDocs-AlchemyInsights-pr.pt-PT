---
title: Atualizar os servidores de nomes do seu domínio para apontar para a Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510295"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="bbd05-102">Atualizar os servidores de nomes do seu domínio para apontar para a Microsoft</span><span class="sxs-lookup"><span data-stu-id="bbd05-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="bbd05-103">Nota: as alterações aos servidores de nomes podem, por vezes, demorar até 48 horas a serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="bbd05-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="bbd05-104">Para configurar o seu domínio com a Microsoft, os conservadores de nomes do seu registo precisam de ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bbd05-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="bbd05-105">Crie ou edite os registos do seu servidor de nomes na sua entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="bbd05-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="bbd05-106">Aceda ao site da sua entidade de registo de domínios e procure a área onde pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="bbd05-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="bbd05-107">Crie ou edite dois registos de servidor de nomes de forma a que correspondam a estes valores:</span><span class="sxs-lookup"><span data-stu-id="bbd05-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="bbd05-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bbd05-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="bbd05-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bbd05-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="bbd05-110">Guarde as alterações.</span><span class="sxs-lookup"><span data-stu-id="bbd05-110">Save changes.</span></span>

<span data-ttu-id="bbd05-111">Também pode encontrar instruções detalhadas neste artigo: [Altere os serviçais para configurar o Microsoft 365 com qualquer registo de domínio](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="bbd05-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  