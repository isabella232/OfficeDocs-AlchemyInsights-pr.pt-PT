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
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493164"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="00228-102">AIP: Políticas que não se comportam como esperado</span><span class="sxs-lookup"><span data-stu-id="00228-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="00228-103">Azure Information Protection: Políticas que não se comportam como esperado, consulte as seguintes orientações recomendadas para várias questões políticas:</span><span class="sxs-lookup"><span data-stu-id="00228-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="00228-104">Se tiver problemas com as marcas visuais, reveja [quando as marcas visuais forem aplicadas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="00228-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="00228-105">Se tiver problemas com a rotulagem automática, [reveja como configurar as condições para a classificação automática e recomendada para a Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [quais os tipos de informação sensíveis procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="00228-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="00228-106">Se tiver problemas com a proteção Native/Pfile, por favor reveja [a configuração da API do ficheiro](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="00228-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="00228-107">Verifique se está a utilizar políticas de âmbito que não estejam configuradas corretamente: [Como configurar a política de proteção de informação Azure para utilizadores específicos utilizando políticas de âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="00228-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="00228-108">Se a rotulagem automática não estiver a funcionar para o Outlook ao anexar um documento rotulado, verifique se a DRMEncryptProperty não está definida como descrito aqui: [Definições de registo irm para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="00228-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="00228-109">Se ainda estiver com problemas, por favor, recolha os registos de clientes da Azure Information Protection e anexe os registos exportados a este bilhete.</span><span class="sxs-lookup"><span data-stu-id="00228-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="00228-110">Abra um documento do Office ou crie um novo e-mail no Outlook.</span><span class="sxs-lookup"><span data-stu-id="00228-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="00228-111">Clique **em Proteger/Sensibilidade**  >  **Ajuda e feedback**.</span><span class="sxs-lookup"><span data-stu-id="00228-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="00228-112">Clique em **Registos de Exportação**.</span><span class="sxs-lookup"><span data-stu-id="00228-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="00228-113">Guarde os registos à sua escolha de localização e anexe-os a este pedido de serviço.</span><span class="sxs-lookup"><span data-stu-id="00228-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="00228-114">Recursos adicionais:</span><span class="sxs-lookup"><span data-stu-id="00228-114">Additional resources:</span></span>

- [<span data-ttu-id="00228-115">Como configurar um rótulo para marcações visuais para proteção de informação Azure</span><span class="sxs-lookup"><span data-stu-id="00228-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="00228-116">Rever documentação de proteção de informação do Azure</span><span class="sxs-lookup"><span data-stu-id="00228-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="00228-117">Use etiquetas de sensibilidade em aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="00228-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

