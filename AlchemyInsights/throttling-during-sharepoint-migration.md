---
title: Limitação durante a Migração do SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958909"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="fd669-102">Limitação do SharePoint</span><span class="sxs-lookup"><span data-stu-id="fd669-102">SharePoint throttling</span></span>

<span data-ttu-id="fd669-103">**Importante:**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="fd669-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="fd669-104">**Limitação do SharePoint**</span><span class="sxs-lookup"><span data-stu-id="fd669-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="fd669-105">O SharePoint Online utiliza a limitação para manter o desempenho e a fiabilidade ideais do serviço do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fd669-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="fd669-106">A limitação restringe o número de ações do utilizador ou chamadas em simultâneo (por script ou código) para evitar a utilização excessiva de recursos.</span><span class="sxs-lookup"><span data-stu-id="fd669-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="fd669-107">Para obter mais informações, visite as seguintes ligações:</span><span class="sxs-lookup"><span data-stu-id="fd669-107">For more information please visit the links below:</span></span>

- <span data-ttu-id="fd669-108">[Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online) (Evitar ser limitado ou bloqueado no SharePoint Online)</span><span class="sxs-lookup"><span data-stu-id="fd669-108">[Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span></span>
- <span data-ttu-id="fd669-109">[Data Migration and SPO Throttling](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/) (Migração de Dados e Limitação de SPO)</span><span class="sxs-lookup"><span data-stu-id="fd669-109">[Data Migration and SPO Throttling](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)</span></span>
- <span data-ttu-id="fd669-110">[SharePoint Online and OneDrive Migration Speed](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed) (Velocidade da Migração do SharePoint Online e do OneDrive)</span><span class="sxs-lookup"><span data-stu-id="fd669-110">[SharePoint Online and OneDrive Migration Speed](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)</span></span>
- <span data-ttu-id="fd669-111">[Handle SharePoint Online throttling by using exponential back off](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off) (Lidar com a limitação do SharePoint Online mediante o recuo exponencial)</span><span class="sxs-lookup"><span data-stu-id="fd669-111">[Handle SharePoint Online throttling by using exponential back off](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)</span></span>
- <span data-ttu-id="fd669-112">[Capacity planning and load testing SharePoint Online](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0) (Planeamento de capacidade e teste de carga do SharePoint Online)</span><span class="sxs-lookup"><span data-stu-id="fd669-112">[Capacity planning and load testing SharePoint Online](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)</span></span>
- <span data-ttu-id="fd669-113">[I am experiencing poor performance or throttling during migration](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting) (Estou a sofrer de fraco desempenho ou de limitações durante a migração)</span><span class="sxs-lookup"><span data-stu-id="fd669-113">[I am experiencing poor performance or throttling during migration](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)</span></span>