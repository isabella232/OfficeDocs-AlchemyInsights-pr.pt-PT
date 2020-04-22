---
title: Ativar o Office 365 ATP para equipas SharePoint, OneDrive e Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703437"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="f5000-102">Ativar o Office 365 Advanced Threat Protection for SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f5000-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="f5000-103">Vá https://protection.office.com e inscreva-se.</span><span class="sxs-lookup"><span data-stu-id="f5000-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="f5000-104">Escolha**anexos seguros**de**política** > de gestão de **ameaças.** > </span><span class="sxs-lookup"><span data-stu-id="f5000-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="f5000-105">Selecione **ligar ATP para As equipas SharePoint, OneDrive e Microsoft**e, em seguida, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="f5000-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="f5000-106">(Recomendado) Como administrador global ou administrador do SharePoint Online, execute o [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DesdefinidoInizadoFileDownload** definido como *verdadeiro*.</span><span class="sxs-lookup"><span data-stu-id="f5000-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="f5000-107">(Recomendado) [Configurar alertas](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para ficheiros detetados.</span><span class="sxs-lookup"><span data-stu-id="f5000-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="f5000-108">O ATP irá analisar todos os ficheiros do SharePoint Online, OneDrive ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f5000-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="f5000-109">Os ficheiros são digitalizados assincronicamente, através de um processo que utiliza eventos de partilha e atividade de hóspedes, juntamente com heurística inteligente e sinais de ameaça para identificar ficheiros maliciosos.</span><span class="sxs-lookup"><span data-stu-id="f5000-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="f5000-110">Consulte [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="f5000-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>