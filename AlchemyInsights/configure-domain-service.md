---
title: Configure o serviço de domínio
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885691"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="d5107-102">Não é possível ativar a AAD-DS ou a implantação está a falhar</span><span class="sxs-lookup"><span data-stu-id="d5107-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="d5107-103">Para resolver a questão do serviço de domínio AD AD (AAD-DS) não estar ativado ou não ser implementado, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="d5107-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="d5107-104">Se estiver a utilizar uma rede virtual já existente, verifique se o NSG tem regras que bloqueiam as portas necessárias para sincronizar em AAD-DS no portal https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="d5107-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="d5107-105">Verifique se a sua mensagem de erro é respondida neste guia de resolução de problemas que está disponível em  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="d5107-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="d5107-106">Tente implementar os Serviços de Domínio AZure numa nova rede virtual.</span><span class="sxs-lookup"><span data-stu-id="d5107-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="d5107-107">Siga o guia 'Iniciar a partida' sobre como implementar a AAD-DS: [Criar e Configurar serviços de domínio AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="d5107-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="d5107-108">Se estiver a ter problemas com a Implementação de Serviços de Domínio Azure AD, consulte [os Serviços de Domínio Ad Ad de resolução](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) de problemas para resolver erros comuns para o ajudar a pôr as coisas a funcionar novamente.</span><span class="sxs-lookup"><span data-stu-id="d5107-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="d5107-109">**Incapaz de desativar a AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="d5107-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="d5107-110">AAD-DS não pode ser pausada.</span><span class="sxs-lookup"><span data-stu-id="d5107-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="d5107-111">Se desejar parar de utilizar o seu domínio gerido, este deve ser eliminado.</span><span class="sxs-lookup"><span data-stu-id="d5107-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="d5107-112">Para eliminar o seu domínio Gerido, consulte [eliminar o Serviço de Domínio AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="d5107-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



