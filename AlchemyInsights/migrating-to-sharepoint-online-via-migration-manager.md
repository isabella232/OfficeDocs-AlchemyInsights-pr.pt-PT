---
title: Migrar para o SharePoint Online através do Gestor de Migração
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932189"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="8d2b3-102">Migrar para o SharePoint Online através do Gestor de Migração</span><span class="sxs-lookup"><span data-stu-id="8d2b3-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="8d2b3-103">**Importante**: muitos clientes do SharePoint Online e OneDrive executam aplicações essenciais para as empresas no serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8d2b3-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8d2b3-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho à distância.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8d2b3-106">Como medida de suporte a este objetivo, implementámos limitações mais restritas em aplicações de segundo plano (soluções de migração, DLP e cópias de segurança) durante as horas diurnas dos dias úteis.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8d2b3-107">Deverá esperar uma limitação bastante restrita por parte destas aplicações durante este período de tempo.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8d2b3-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8d2b3-109">**Gestor de Migração**</span><span class="sxs-lookup"><span data-stu-id="8d2b3-109">**Migration Manager**</span></span>

<span data-ttu-id="8d2b3-110">Localizado no moderno Centro de Administração do SharePoint, o Gestor de Migração guia-o através da configuração dos seus clientes e da criação das suas tarefas.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="8d2b3-111">Pode especificar configurações globais ou de nível da tarefa, visualizar o progresso total da tarefa e transferir relatórios de resumo agregados e ao nível das tarefas.</span><span class="sxs-lookup"><span data-stu-id="8d2b3-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="8d2b3-112">Começar com o Gestor de Migração</span><span class="sxs-lookup"><span data-stu-id="8d2b3-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="8d2b3-113">Configurar clientes do Gestor de Migração</span><span class="sxs-lookup"><span data-stu-id="8d2b3-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="8d2b3-114">Definições do Gestor de Migração</span><span class="sxs-lookup"><span data-stu-id="8d2b3-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
