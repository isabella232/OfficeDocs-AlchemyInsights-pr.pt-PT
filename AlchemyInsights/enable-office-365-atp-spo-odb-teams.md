---
title: Ativar o Office 365 ATP para as equipas SharePoint, OneDrive e Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709918"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1acf8-102">Ativar o Office 365 Advanced Threat Protection for SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1acf8-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1acf8-103">Vá https://protection.office.com e inscreva-se.</span><span class="sxs-lookup"><span data-stu-id="1acf8-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1acf8-104">Escolha **Threat management**os  >  **Policy**  >  **anexos seguros da**política de gestão de ameaças .</span><span class="sxs-lookup"><span data-stu-id="1acf8-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1acf8-105">Selecione **Ligue ATP para SharePoint, OneDrive e Microsoft Teams**e, em seguida, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="1acf8-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1acf8-106">(Recomendado) Como administrador global ou administrador on-line sharePoint, executar o [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *verdadeiro*.</span><span class="sxs-lookup"><span data-stu-id="1acf8-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1acf8-107">(Recomendado) [Configurar alertas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para ficheiros detetados.</span><span class="sxs-lookup"><span data-stu-id="1acf8-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1acf8-108">O ATP irá analisar todos os ficheiros do SharePoint Online, OneDrive ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1acf8-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1acf8-109">Os ficheiros são digitalizados assíncrono, através de um processo que utiliza eventos de partilha e atividade de hóspedes, juntamente com heurística inteligente e sinais de ameaça para identificar ficheiros maliciosos.</span><span class="sxs-lookup"><span data-stu-id="1acf8-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1acf8-110">Ver [ATP para SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1acf8-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>