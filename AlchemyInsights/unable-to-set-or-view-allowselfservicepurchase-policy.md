---
title: Incapaz de definir ou ver a política de Compra allowSelfService
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091746"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="dde2f-102">Incapaz de definir ou ver a política de Compra allowSelfService</span><span class="sxs-lookup"><span data-stu-id="dde2f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="dde2f-103">Ao tentar definir ou visualizar a política AllowSelfServicePurchase, recebe a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="dde2f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="dde2f-104">*HandleError : Falha na recuperação da política do produto com o PolicyId 'AllowSelfServicePurchase', ErrorMessage - A ligação subjacente foi fechada: Ocorreu um erro inesperado num envio.*</span><span class="sxs-lookup"><span data-stu-id="dde2f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="dde2f-105">Isto pode ser devido a uma versão mais antiga da Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="dde2f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="dde2f-106">Para ligar o serviço MSCommerce, precisa de utilizar o TLS 1.2 ou superior.</span><span class="sxs-lookup"><span data-stu-id="dde2f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="dde2f-107">Tente os seguintes passos para ativar/definir o protocolo TLS para 1.2, verificar e voltar a tentar.</span><span class="sxs-lookup"><span data-stu-id="dde2f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="dde2f-108">No pedido de comando PowerShell\) (PS C: insira o seguinte comando para definir o protocolo TLS na versão 1.2:</span><span class="sxs-lookup"><span data-stu-id="dde2f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="dde2f-109">\[Net.ServicePointManager]::SecurityProtocol \[= Net.SecurityProtocolType:::Tls12</span><span class="sxs-lookup"><span data-stu-id="dde2f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="dde2f-110">Verifique os protocolos TLS em uso, com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="dde2f-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="dde2f-111">\[Net.ServicePointManager]::Protocolo de segurança</span><span class="sxs-lookup"><span data-stu-id="dde2f-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="dde2f-112">Tente novamente os comandos Get ou Update, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="dde2f-112">Retry the Get or Update commands as needed.</span></span>

