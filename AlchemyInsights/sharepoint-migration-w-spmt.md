---
title: Migração sharePoint com SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931561"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="41ef7-102">Migração sharePoint com SPMT</span><span class="sxs-lookup"><span data-stu-id="41ef7-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="41ef7-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="41ef7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="41ef7-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="41ef7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="41ef7-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="41ef7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="41ef7-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="41ef7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="41ef7-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="41ef7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="41ef7-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="41ef7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="41ef7-109">**Ferramenta de Migração do SharePoint**</span><span class="sxs-lookup"><span data-stu-id="41ef7-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="41ef7-110">Projetada para ser usada para migrações que vão desde o menor conjunto de ficheiros a uma migração empresarial em larga escala, a Ferramenta de Migração SharePoint permitirá transferir as suas informações para a nuvem e tirar partido da mais recente colaboração, inteligência e soluções de segurança com o Office 365.</span><span class="sxs-lookup"><span data-stu-id="41ef7-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="41ef7-111">Descarregue e instale a Ferramenta de Migração SharePoint</span><span class="sxs-lookup"><span data-stu-id="41ef7-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="41ef7-112">Resolução de problemas comum problemas e erros de SPMT</span><span class="sxs-lookup"><span data-stu-id="41ef7-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="41ef7-113">Problemas de resolução de problemas problemas de instalação SPMT</span><span class="sxs-lookup"><span data-stu-id="41ef7-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
