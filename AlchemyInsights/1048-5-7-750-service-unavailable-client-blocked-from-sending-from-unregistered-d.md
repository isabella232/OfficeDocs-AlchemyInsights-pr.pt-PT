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
ms.openlocfilehash: 5fe5b343d89c49e1805e4d0cac6698ef35e1dd30
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921935"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="8d0e7-103">5.7.750 cliente impedido de enviar de domínio não registado</span><span class="sxs-lookup"><span data-stu-id="8d0e7-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="8d0e7-104">O erro ocorre quando um grande volume de mensagens são enviadas a partir de domínios que não estão aprovisionados no Office 365 (adicionados como domínios aceites e validado).</span><span class="sxs-lookup"><span data-stu-id="8d0e7-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="8d0e7-105">Para evitar este erro, pode utilizar uma conexão de fluxo de correio baseada em certificados em que o domínio o certificado é um domínio aprovisionado ou pode aprovisionar todos os domínios de envio.</span><span class="sxs-lookup"><span data-stu-id="8d0e7-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

