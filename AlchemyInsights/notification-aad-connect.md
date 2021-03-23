---
title: Notificação AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037240"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="b3079-102">Notificação AAD Connect</span><span class="sxs-lookup"><span data-stu-id="b3079-102">Notification AAD Connect</span></span>

- <span data-ttu-id="b3079-103">Certifique-se de que está autorizado a realizar a operação.</span><span class="sxs-lookup"><span data-stu-id="b3079-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="b3079-104">Os Administradores Globais têm acesso por defeito.</span><span class="sxs-lookup"><span data-stu-id="b3079-104">Global Admins have access by default.</span></span> <span data-ttu-id="b3079-105">Além disso, pode utilizar [o Controlo de Acesso Baseado em Função](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) para delegar a permissão de registo ao Contribuinte.</span><span class="sxs-lookup"><span data-stu-id="b3079-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="b3079-106">Certifique-se de que os pontos finais necessários estão ativados e não bloqueados devido à firewall.</span><span class="sxs-lookup"><span data-stu-id="b3079-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="b3079-107">Para mais [informações, consulte os requisitos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="b3079-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="b3079-108">O registo pode falhar devido à comunicação de saída ser submetida a inspeção SSL pela camada de rede.</span><span class="sxs-lookup"><span data-stu-id="b3079-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="b3079-109">Certifique-se de que verificou as definições de notificação do Azure AD Connect Health e reveja a sua definição.</span><span class="sxs-lookup"><span data-stu-id="b3079-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="b3079-110">Para entender como configurar as definições de notificação para notificações Azure AD Connect Health, consulte este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="b3079-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="b3079-111">Para saber mais sobre o relatório de sincronização do AAD Connect Health e como descarregá-lo, consulte [o relatório de sincronização do nível de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="b3079-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="b3079-112">Para resolver problemas, os alertas de saúde da AAD Connect seguem [o guia de resolução de problemas para alertas de frescura de dados AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e para perguntas comumente colocadas, consulte [questões de instalação comuns da AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="b3079-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
