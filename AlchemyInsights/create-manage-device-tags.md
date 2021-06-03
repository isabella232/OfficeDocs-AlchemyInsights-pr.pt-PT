---
title: Criar e gerir etiquetas ou grupos de dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731964"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="664af-102">Criar e gerir etiquetas ou grupos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="664af-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="664af-103">Adicione etiquetas em dispositivos para criar uma afiliação de grupo lógica.</span><span class="sxs-lookup"><span data-stu-id="664af-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="664af-104">As etiquetas de dispositivo suportam o mapeamento adequado da rede, permitindo-lhe anexar etiquetas diferentes para capturar o contexto e permitir a criação de listas dinâmicas como parte de um incidente.</span><span class="sxs-lookup"><span data-stu-id="664af-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="664af-105">As etiquetas podem ser utilizadas como um filtro na vista de lista Dispositivos ou para agrupar dispositivos.</span><span class="sxs-lookup"><span data-stu-id="664af-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="664af-106">Para obter mais informações sobre o agrupamento de dispositivos, [consulte Criar e gerir etiquetas de dispositivo.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="664af-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="664af-107">Pode adicionar etiquetas nos dispositivos ao:</span><span class="sxs-lookup"><span data-stu-id="664af-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="664af-108">Utilizar o portal</span><span class="sxs-lookup"><span data-stu-id="664af-108">Using the portal</span></span>

- <span data-ttu-id="664af-109">Definir um valor de chave de registo</span><span class="sxs-lookup"><span data-stu-id="664af-109">Setting a registry key value</span></span>
 
<span data-ttu-id="664af-110">**Nota:** Pode haver latência entre o tempo em que uma etiqueta é adicionada a um dispositivo e a res suas disponibilidade na lista de dispositivos e na página do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="664af-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="664af-111">Para adicionar etiquetas de dispositivo através da API, consulte [Adicionar ou remover API de etiquetas de dispositivo.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="664af-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="664af-112">Adicionar e gerir etiquetas de dispositivo utilizando o portal</span><span class="sxs-lookup"><span data-stu-id="664af-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="664af-113">Selecione o dispositivo em que pretende gerir as etiquetas.</span><span class="sxs-lookup"><span data-stu-id="664af-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="664af-114">Pode selecionar ou procurar um dispositivo a partir de qualquer uma das seguintes vistas:</span><span class="sxs-lookup"><span data-stu-id="664af-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="664af-115">**Dashboard de operações de segurança** Selecione o nome do dispositivo a partir da secção Principais dispositivos com alertas ativos.</span><span class="sxs-lookup"><span data-stu-id="664af-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="664af-116">**Fila de alertas -** Selecione o nome do dispositivo junto ao ícone do dispositivo a partir da fila de alertas.</span><span class="sxs-lookup"><span data-stu-id="664af-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="664af-117">**Lista de dispositivos** – selecione o nome do dispositivo a partir da lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="664af-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="664af-118">**Caixa de pesquisa** - Selecione Dispositivo a partir do menu de menu de lista e introduza o nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="664af-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="664af-119">Também pode chegar à página de alerta através das vistas de ficheiro e IP.</span><span class="sxs-lookup"><span data-stu-id="664af-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="664af-120">**Selecione Gerir Etiquetas** na linha de Ações de resposta.</span><span class="sxs-lookup"><span data-stu-id="664af-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="664af-121">Escreva para encontrar ou criar etiquetas.</span><span class="sxs-lookup"><span data-stu-id="664af-121">Type to find or create tags.</span></span>

<span data-ttu-id="664af-122">As etiquetas são adicionadas à vista dispositivo e são refletidas na vista de lista Dispositivos.</span><span class="sxs-lookup"><span data-stu-id="664af-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="664af-123">Em seguida, pode utilizar o filtro Etiquetas para ver a lista de dispositivos relevante.</span><span class="sxs-lookup"><span data-stu-id="664af-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="664af-124">Para obter mais informações, consulte [Criar e gerir etiquetas de dispositivo.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="664af-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>