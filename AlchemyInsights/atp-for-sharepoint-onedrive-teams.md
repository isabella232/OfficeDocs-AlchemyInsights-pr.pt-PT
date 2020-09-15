---
title: ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715572"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="53ed0-102">ATP para SharePoint, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="53ed0-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="53ed0-103">Siga estes passos para permitir a Proteção Avançada de Ameaças:</span><span class="sxs-lookup"><span data-stu-id="53ed0-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="53ed0-104">Vá [https://protection.office.com](https://protection.office.com) e inscreva-se com um administrador global ou conta de administrador de segurança.</span><span class="sxs-lookup"><span data-stu-id="53ed0-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="53ed0-105">No painel de navegação à **Policy** esquerda sob **gestão de ameaças,** escolha \> **Os Anexos Seguros de**Política .</span><span class="sxs-lookup"><span data-stu-id="53ed0-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="53ed0-106">Selecione **Ligue ATP para SharePoint, OneDrive e Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="53ed0-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="53ed0-107">[Crie uma política de alerta de atividade](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) para receber notificações quando detetarmos ficheiros maliciosos.</span><span class="sxs-lookup"><span data-stu-id="53ed0-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="53ed0-108">Para obter instruções completas, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="53ed0-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="53ed0-109">**Nota:** Por design, o ATP não digitaliza todos os ficheiros do SharePoint Online, OneDrive for Business ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="53ed0-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="53ed0-110">Os ficheiros são analisados assíncrono por um processo que utiliza atividade de partilha, atividade de hóspedes e sinais de ameaça para identificar ficheiros maliciosos.</span><span class="sxs-lookup"><span data-stu-id="53ed0-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="53ed0-111">Para mais informações, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="53ed0-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
