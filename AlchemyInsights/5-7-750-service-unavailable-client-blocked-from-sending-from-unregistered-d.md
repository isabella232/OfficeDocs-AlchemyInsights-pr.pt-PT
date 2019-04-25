---
title: 1048 5.7.750 serviço indisponível. Cliente impedido de enviar a partir de domínios não registados
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 06be6babc524ae0d8065355218426c695f49be66
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32365873"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="3dd27-103">5.7.750 cliente impedido de enviar de domínio não registado</span><span class="sxs-lookup"><span data-stu-id="3dd27-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="3dd27-104">O erro ocorre quando um grande volume de mensagens são enviadas a partir de domínios que não estão aprovisionados no Office 365 (adicionados como domínios aceites e validado).</span><span class="sxs-lookup"><span data-stu-id="3dd27-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="3dd27-105">Para evitar este erro, pode utilizar uma conexão de fluxo de correio baseada em certificados em que o domínio o certificado é um domínio aprovisionado ou pode aprovisionar todos os domínios de envio.</span><span class="sxs-lookup"><span data-stu-id="3dd27-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
