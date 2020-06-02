---
title: 'AIP: Políticas que não se comportam como esperado'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506569"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="c664e-102">AIP: Políticas que não se comportam como esperado</span><span class="sxs-lookup"><span data-stu-id="c664e-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="c664e-103">Azure Information Protection: Políticas que não se comportam como esperado, consulte as seguintes orientações recomendadas para várias questões políticas:</span><span class="sxs-lookup"><span data-stu-id="c664e-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="c664e-104">Se tiver problemas com as marcas visuais, reveja [quando as marcas visuais forem aplicadas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="c664e-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="c664e-105">Se tiver problemas com a rotulagem automática, [reveja como configurar as condições para a classificação automática e recomendada para a Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [quais os tipos de informação sensíveis procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="c664e-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="c664e-106">Se tiver problemas com a proteção Native/Pfile, por favor reveja [a configuração da API do ficheiro](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="c664e-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="c664e-107">Verifique se está a utilizar políticas de âmbito que não estejam configuradas corretamente: [Como configurar a política de proteção de informação Azure para utilizadores específicos utilizando políticas de âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="c664e-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="c664e-108">Se a rotulagem automática não estiver a funcionar para o Outlook ao anexar um documento rotulado, verifique se a DRMEncryptProperty não está definida como descrito aqui: [Definições de registo irm para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="c664e-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="c664e-109">Se ainda estiver com problemas, por favor, recolha os registos de clientes da Azure Information Protection e anexe os registos exportados a este bilhete.</span><span class="sxs-lookup"><span data-stu-id="c664e-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="c664e-110">Abra um documento do Office ou crie um novo e-mail no Outlook.</span><span class="sxs-lookup"><span data-stu-id="c664e-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="c664e-111">Clique **em Proteger/Sensibilidade**  >  **Ajuda e feedback**.</span><span class="sxs-lookup"><span data-stu-id="c664e-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="c664e-112">Clique em **Registos de Exportação**.</span><span class="sxs-lookup"><span data-stu-id="c664e-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="c664e-113">Guarde os registos à sua escolha de localização e anexe-os a este pedido de serviço.</span><span class="sxs-lookup"><span data-stu-id="c664e-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="c664e-114">Recursos adicionais:</span><span class="sxs-lookup"><span data-stu-id="c664e-114">Additional resources:</span></span>

- [<span data-ttu-id="c664e-115">Como configurar um rótulo para marcações visuais para proteção de informação Azure</span><span class="sxs-lookup"><span data-stu-id="c664e-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="c664e-116">Rever documentação de proteção de informação do Azure</span><span class="sxs-lookup"><span data-stu-id="c664e-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c664e-117">Use etiquetas de sensibilidade em aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="c664e-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

