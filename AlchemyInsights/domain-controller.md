---
title: Controlador de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901310"
---
# <a name="domain-controller"></a><span data-ttu-id="5a131-102">Controlador de domínio</span><span class="sxs-lookup"><span data-stu-id="5a131-102">Domain controller</span></span>

<span data-ttu-id="5a131-103">**Não é possível ativar a AAD-DS ou a implantação está a falhar**</span><span class="sxs-lookup"><span data-stu-id="5a131-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="5a131-104">Para resolver a questão do serviço de domínio AD AD (AAD-DS) não estar ativado ou não ser implementado, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="5a131-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="5a131-105">Se estiver a utilizar uma rede virtual já existente, verifique se o NSG tem regras que bloqueiam as portas necessárias para sincronizar em AAD-DS no portal https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="5a131-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="5a131-106">Verifique se a sua mensagem de erro é respondida neste guia de resolução de problemas que está disponível em  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="5a131-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="5a131-107">Tente implementar os Serviços de Domínio AZure numa nova rede virtual.</span><span class="sxs-lookup"><span data-stu-id="5a131-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="5a131-108">Siga o guia 'Iniciar a ção' sobre como implementar o AAD-DS, que está disponível no [Tutorial para criar serviços de domínio AD AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="5a131-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="5a131-109">Se estiver a ter problemas com a Implementação de Serviços de Domínio Azure AD, consulte [os Serviços de Domínio Ad Ad de resolução](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) de problemas para resolver erros comuns para o ajudar a pôr as coisas a funcionar novamente.</span><span class="sxs-lookup"><span data-stu-id="5a131-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="5a131-110">**Incapaz de desativar a AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="5a131-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="5a131-111">AAD-DS não pode ser pausada.</span><span class="sxs-lookup"><span data-stu-id="5a131-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="5a131-112">Se desejar parar de utilizar o seu domínio gerido, este deve ser eliminado.</span><span class="sxs-lookup"><span data-stu-id="5a131-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="5a131-113">Se encontrar problemas, para resolver mensagens de erro comuns e para medidas de resolução de problemas associadas para ajudá-lo a pôr as coisas a funcionar novamente, consulte [os Serviços de Domínio do Diretório Ativo troubleshoot Azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="5a131-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
