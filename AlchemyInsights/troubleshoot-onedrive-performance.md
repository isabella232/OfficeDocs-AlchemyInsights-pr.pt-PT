---
title: Resolução de problemas Desempenho OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757896"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="cecea-102">Resolução de problemas Desempenho OneDrive</span><span class="sxs-lookup"><span data-stu-id="cecea-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="cecea-103">Se estiver a experimentar uma sincronização mais lenta do que o esperado, ou problemas de desempenho semelhantes com o OneDrive:</span><span class="sxs-lookup"><span data-stu-id="cecea-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="cecea-104">Confirme que não existem problemas conhecidos utilizando o [Painel de Saúde do Serviço](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="cecea-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="cecea-105">[Ativar os Ficheiros A Pedido](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) para que possa aceder a todos os seus ficheiros no OneDrive sem ter de descarregar todos eles e utilizar o espaço de armazenamento no seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cecea-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="cecea-106">[Reveja as melhores práticas](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) para o planeamento e desempenho da rede.</span><span class="sxs-lookup"><span data-stu-id="cecea-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="cecea-107">[Maximize a velocidade de upload e download](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especialmente se estiver a sincronizar um dispositivo pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="cecea-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="cecea-108">Se estiver a sincronizar uma biblioteca com mais de 100.000 itens, a sincronização do OneDrive pode parecer presa durante muito tempo, ou o estado mostra o Processamento 0KB de xMB."</span><span class="sxs-lookup"><span data-stu-id="cecea-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="cecea-109">[Saiba mais sobre sincronizar mais de 100.000 ficheiros,](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) bem como [o limite suportado pelo OneDrive de 300.000 ficheiros](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="cecea-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="cecea-110">Quando um utilizador excede os limites de utilização, o SharePoint Online acelera quaisquer outros pedidos dessa conta de utilizador por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="cecea-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="cecea-111">Todas as ações do utilizador são aceleradas enquanto o acelerador está em vigor.</span><span class="sxs-lookup"><span data-stu-id="cecea-111">All user actions are throttled while the throttle is in effect.</span></span>
