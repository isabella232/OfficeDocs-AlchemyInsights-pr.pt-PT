---
title: Limpeza automática de dispositivos em intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555227"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="43550-102">Limpeza automática de dispositivos em intune</span><span class="sxs-lookup"><span data-stu-id="43550-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="43550-103">O Intune permite que o administrador configuure um intervalo de tempo entre 90 e 270 dias, após o qual os dispositivos em contrao tempo são removidos do serviço.</span><span class="sxs-lookup"><span data-stu-id="43550-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="43550-104">Esta definição é ampla e uma vez ativada entra em vigor imediatamente.</span><span class="sxs-lookup"><span data-stu-id="43550-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="43550-105">Quaisquer dispositivos não verificados no servidor Intune durante um período que exceda a definição são permanentemente eliminados.</span><span class="sxs-lookup"><span data-stu-id="43550-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="43550-106">**Nota** Apenas os objetos do dispositivo MDM são elegíveis para esta ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="43550-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="43550-107">Excluem-se apenas objetos de dispositivoS EAS.</span><span class="sxs-lookup"><span data-stu-id="43550-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="43550-108">Para informações adicionais sobre quando um dispositivo se torna elegível para eliminação com base na configuração de limpeza do dispositivo e no seu "estado":</span><span class="sxs-lookup"><span data-stu-id="43550-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="43550-109">Definição: **Eliminar dispositivos após a última data de check-in: Sim (algum valor (N) em dias especificados)**</span><span class="sxs-lookup"><span data-stu-id="43550-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="43550-110">Com base no valor (N) configurado na definição, o serviço Intune elimina o dispositivo nos dias especificados após a última verificação com sucesso.</span><span class="sxs-lookup"><span data-stu-id="43550-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="43550-111">Definição: **Eliminar dispositivos após a última data de check-in: Não**</span><span class="sxs-lookup"><span data-stu-id="43550-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="43550-112">180 dias após o termo do certificado do dispositivo e não ser renovado, o dispositivo é eliminado.</span><span class="sxs-lookup"><span data-stu-id="43550-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="43550-113">**Nota** Em ambos os casos, o dispositivo deve ser registado com sucesso no Intune.</span><span class="sxs-lookup"><span data-stu-id="43550-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="43550-114">O registo ocorre durante o primeiro check-in do dispositivo com o serviço Intune.</span><span class="sxs-lookup"><span data-stu-id="43550-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="43550-115">Se um dispositivo se inscrever com sucesso no Intune mas não se tornar intune registado, o dispositivo é eliminado 270 dias após a inscrição.</span><span class="sxs-lookup"><span data-stu-id="43550-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="43550-116">(90 dias para marcar o dispositivo como revogado e, em seguida, mais 180 dias para apagar o registo.)</span><span class="sxs-lookup"><span data-stu-id="43550-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="43550-117">Não existe atualmente nenhum mecanismo na consola Intune para estabelecer a data de validade da certificação do dispositivo para qualquer dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43550-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>