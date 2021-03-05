---
title: Problema com a AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482074"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="1c219-102">Problema com a AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="1c219-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="1c219-103">Certifique-se de que está autorizado a realizar a operação.</span><span class="sxs-lookup"><span data-stu-id="1c219-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="1c219-104">Os Administradores Globais têm acesso por defeito.</span><span class="sxs-lookup"><span data-stu-id="1c219-104">Global Admins have access by default.</span></span> <span data-ttu-id="1c219-105">Além disso, pode utilizar [o Controlo de Acesso Baseado em Função](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) para delegar a permissão de registo ao Contribuinte.</span><span class="sxs-lookup"><span data-stu-id="1c219-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="1c219-106">Certifique-se de que os pontos finais necessários estão ativados e não bloqueados devido à firewall.</span><span class="sxs-lookup"><span data-stu-id="1c219-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="1c219-107">Para mais [informações, consulte os requisitos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="1c219-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="1c219-108">O registo pode falhar devido à comunicação de saída ser submetida a inspeção SSL pela camada de rede.</span><span class="sxs-lookup"><span data-stu-id="1c219-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="1c219-109">Certifique-se de que verificou as definições de notificação para Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="1c219-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="1c219-110">Por favor, reveja a sua configuração.</span><span class="sxs-lookup"><span data-stu-id="1c219-110">Please review your setting.</span></span> <span data-ttu-id="1c219-111">Este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pode ajudá-lo a entender como configurar as definições de notificação para notificações de saúde Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1c219-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="1c219-112">Para saber mais sobre o relatório de sincronização do AAD Connect Health e como descarregá-lo, consulte [o relatório de sincronização do nível de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="1c219-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="1c219-113">Para resolver os alertas de problemas da AAD Connect Health, siga [o guia de resolução de problemas para alertas de frescura de dados AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e para perguntas comumente feitas, consulte [questões de instalação de instalação Common AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="1c219-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
