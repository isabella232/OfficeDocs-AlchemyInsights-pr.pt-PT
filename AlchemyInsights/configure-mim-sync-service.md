---
title: Configure o serviço MIM Sync
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481867"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="bd58b-102">Configure o serviço MIM Sync</span><span class="sxs-lookup"><span data-stu-id="bd58b-102">Configure MIM Sync service</span></span>

<span data-ttu-id="bd58b-103">O Serviço de Sincronização do Microsoft Identity Manager (MIM) é um componente da MIM.</span><span class="sxs-lookup"><span data-stu-id="bd58b-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="bd58b-104">É um serviço centralizado no local que armazena e integra informação para organizações que têm vários diretórios e bases de dados no local.</span><span class="sxs-lookup"><span data-stu-id="bd58b-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="bd58b-105">Poderá resolver o seu problema com a MIM Sync se o problema tiver sido abordado numa recente atualização à MIM ou for um dos outros problemas mencionados na secção abaixo.</span><span class="sxs-lookup"><span data-stu-id="bd58b-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="bd58b-106">**Passos recomendados**</span><span class="sxs-lookup"><span data-stu-id="bd58b-106">**Recommended steps**</span></span>

1. <span data-ttu-id="bd58b-107">Certifique-se de que está a utilizar uma atualização recente do MIM Sync e verifique as [notas de lançamento](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) do MIM Sync para determinar se o problema foi resolvido numa atualização.</span><span class="sxs-lookup"><span data-stu-id="bd58b-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="bd58b-108">Se o problema estiver com o conector Genérico LDAP, Generic SQL, Lotus Domino ou Web Services, certifique-se de que está a utilizar uma atualização recente dos [conectores genéricos](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="bd58b-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="bd58b-109">Se um mim Sync-run parar com um erro, consulte a tabela de códigos de erro de [execução](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) para determinar as causas potenciais.</span><span class="sxs-lookup"><span data-stu-id="bd58b-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="bd58b-110">Se a execução parar com **a exceção extensão- dll,** clique nessas palavras para abrir a janela **das propriedades do Objeto espacial do Conector** e clique no **Stack Trace...** para ver mais informações sobre a causa subjacente, como descrito na [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="bd58b-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="bd58b-111">Se o serviço de notificação de alteração de palavra-passe (PCNS) reportar o **erro 6025** no registo de eventos durante a sincronização da palavra-passe, consulte o guia para verificar o [erro de reporte do PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="bd58b-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="bd58b-112">Se a sincronização total com o Agente de Gestão de Serviços FIM for lenta, verifique a definição **de crescimento automático** para TempDB, conforme descrito na sincronização lenta ou pendurada na [resolução de problemas.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="bd58b-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="bd58b-113">Se encontrar um erro de stop-server com serviços de criação-via-web falhados utilizando o Agente de Gestão de Serviços FIM, consulte [o Support-Info: serviços de criação-via-web falhados](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) para uma visão geral das causas.</span><span class="sxs-lookup"><span data-stu-id="bd58b-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

