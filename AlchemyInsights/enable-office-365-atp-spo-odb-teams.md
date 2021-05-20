---
title: Ativar Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543939"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="c7f15-102">Ativar o Microsoft Defender Office 365 para SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c7f15-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="c7f15-103">Vá para https://protection.office.com e inscreva-se.</span><span class="sxs-lookup"><span data-stu-id="c7f15-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="c7f15-104">**Selecionar Política de**  >    >  **Gestão de Cofre Anexos**.</span><span class="sxs-lookup"><span data-stu-id="c7f15-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="c7f15-105">**Selecione Acionar o Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams e,** em seguida, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="c7f15-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="c7f15-106">(Recomendado) Como administrador global ou administrador do SharePoint Online, execute o cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido para *true*.</span><span class="sxs-lookup"><span data-stu-id="c7f15-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="c7f15-107">(Recomendado) [Configurar alertas para ficheiros](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) detetados.</span><span class="sxs-lookup"><span data-stu-id="c7f15-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="c7f15-108">O Microsoft Defender Office 365 irá analisar todos os ficheiros no SharePoint Online, OneDrive ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7f15-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="c7f15-109">Os ficheiros são analisados assíncronamente através de um processo que utiliza eventos de partilha e de atividade de convidados, juntamente com sinais de heurística e ameaça inteligentes para identificar ficheiros maliciosos.</span><span class="sxs-lookup"><span data-stu-id="c7f15-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="c7f15-110">Consulte [Microsoft Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c7f15-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>