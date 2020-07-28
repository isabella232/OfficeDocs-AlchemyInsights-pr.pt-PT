---
title: Excluir um canal privado das Equipas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439918"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="4949d-102">Excluir um canal privado das Equipas</span><span class="sxs-lookup"><span data-stu-id="4949d-102">Delete a Teams private channel</span></span>

<span data-ttu-id="4949d-103">A Microsoft está ciente de um problema que elimina um canal privado do Teams se tiver políticas de retenção sharePoint ativadas para o site SharePoint subjacente.</span><span class="sxs-lookup"><span data-stu-id="4949d-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="4949d-104">A Microsoft está a trabalhar numa correção.</span><span class="sxs-lookup"><span data-stu-id="4949d-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="4949d-105">Entretanto, pode utilizar as seguintes soluções para eliminar o canal privado.</span><span class="sxs-lookup"><span data-stu-id="4949d-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="4949d-106">**Excluir a recolha team/site da política de retenção de Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="4949d-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="4949d-107">Vá ao portal de administração do Office 365 e selecione **Mostrar tudo** no painel de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="4949d-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="4949d-108">Nos **centros de administração,** vá para a Política de Prevenção de Perda de Dados de Conformidade & De **Segurança**  >  **Data Loss Prevention**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="4949d-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="4949d-109">Identifique qualquer política que se aplique aos sites sharepoint e modifique a política para que o site sharepoint para a equipa que contenha o canal privado NÃO seja incluído na política de retenção.</span><span class="sxs-lookup"><span data-stu-id="4949d-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="4949d-110">Salve a apólice.</span><span class="sxs-lookup"><span data-stu-id="4949d-110">Save the policy.</span></span>
    <span data-ttu-id="4949d-111">Pode levar até 24 horas para que as definições de política produzam efeitos.</span><span class="sxs-lookup"><span data-stu-id="4949d-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="4949d-112">Depois de o site ter sido excluído, pode apagar o canal privado.</span><span class="sxs-lookup"><span data-stu-id="4949d-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="4949d-113">Poderá ***might*** eliminar o canal privado utilizando o Microsoft Teams no seu dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="4949d-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="4949d-114">Para obter informações relacionadas com o SharePoint, consulte [Não conseguir eliminar itens no SharePoint Online ou no OneDrive para negócios.](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)</span><span class="sxs-lookup"><span data-stu-id="4949d-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>