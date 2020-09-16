---
title: 'AIP: Políticas que não se comportam como esperado'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663200"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="f60f4-102">AIP: Políticas que não se comportam como esperado</span><span class="sxs-lookup"><span data-stu-id="f60f4-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="f60f4-103">Azure Information Protection: Políticas que não se comportam como esperado, consulte as seguintes orientações recomendadas para várias questões políticas:</span><span class="sxs-lookup"><span data-stu-id="f60f4-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="f60f4-104">Se tiver problemas com as marcas visuais, reveja [quando as marcas visuais forem aplicadas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="f60f4-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="f60f4-105">Se tiver problemas com a rotulagem automática, [reveja como configurar as condições para a classificação automática e recomendada para a Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [quais os tipos de informação sensíveis procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="f60f4-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="f60f4-106">Se tiver problemas com a proteção Native/Pfile, por favor reveja [a configuração da API do ficheiro](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="f60f4-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="f60f4-107">Verifique se está a utilizar políticas de âmbito que não estejam configuradas corretamente: [Como configurar a política de proteção de informação Azure para utilizadores específicos utilizando políticas de âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="f60f4-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="f60f4-108">Se a rotulagem automática não estiver a funcionar para o Outlook ao anexar um documento rotulado, verifique se a DRMEncryptProperty não está definida como descrito aqui: [Definições de registo irm para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="f60f4-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="f60f4-109">Se ainda estiver com problemas, por favor, recolha os registos de clientes da Azure Information Protection e anexe os registos exportados a este bilhete.</span><span class="sxs-lookup"><span data-stu-id="f60f4-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="f60f4-110">Abra um documento do Office ou crie um novo e-mail no Outlook.</span><span class="sxs-lookup"><span data-stu-id="f60f4-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="f60f4-111">Clique **em Proteger/Sensibilidade**  >  **Ajuda e feedback**.</span><span class="sxs-lookup"><span data-stu-id="f60f4-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="f60f4-112">Clique em **Registos de Exportação**.</span><span class="sxs-lookup"><span data-stu-id="f60f4-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="f60f4-113">Guarde os registos à sua escolha de localização e anexe-os a este pedido de serviço.</span><span class="sxs-lookup"><span data-stu-id="f60f4-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="f60f4-114">Recursos adicionais:</span><span class="sxs-lookup"><span data-stu-id="f60f4-114">Additional resources:</span></span>

- [<span data-ttu-id="f60f4-115">Como configurar um rótulo para marcações visuais para proteção de informação Azure</span><span class="sxs-lookup"><span data-stu-id="f60f4-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="f60f4-116">Rever documentação de proteção de informação do Azure</span><span class="sxs-lookup"><span data-stu-id="f60f4-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f60f4-117">Utilize etiquetas de sensibilidade em aplicações microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f60f4-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

