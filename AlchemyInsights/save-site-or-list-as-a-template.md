---
title: Guardar site ou lista como um modelo
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243591"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="f4a7c-102">Guardar site ou lista como um modelo</span><span class="sxs-lookup"><span data-stu-id="f4a7c-102">Save site or list as a template</span></span>

<span data-ttu-id="f4a7c-103">Modelos de site do SharePoint são definições previamente concebidas destinadas em torno de uma determinada necessidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="f4a7c-104">Para mais informações, consulte [utilizar modelos para criar diferentes tipos de sites do SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="f4a7c-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="f4a7c-105">Eis algumas questões/soluções comuns relativas ao guardar um Site ou lista como um modelo no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="f4a7c-106">**Guardar site/lista modelo botão não estiver em falta ou não disponível**.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="f4a7c-107">Os administradores serão necessário permitir Script personalizado para activar as funcionalidades do modelo.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="f4a7c-108">Para obter passos detalhados, exemplos e considerações consulte [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="f4a7c-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="f4a7c-109">O site de guardar como comando de modelo não é suportado e pode causar problemas em sites que utilizem a infra-estrutura de publicação do SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="f4a7c-110">**O modelo de site não é possível criar ou não funciona correctamente**</span><span class="sxs-lookup"><span data-stu-id="f4a7c-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="f4a7c-111">O modelo pode estar em falta uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não vai activar.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="f4a7c-112">Se a funcionalidade não está disponível para activar a colecção de sites actual, é possível utilizar o modelo de site para criar um site.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="f4a7c-113">Verifique se todas as listas ou bibliotecas de excederem o [Limiar de limite de vista de lista](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, como este pode bloquear a criação de um modelo de site.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="f4a7c-114">O site poderá estar a utilizar demasiados recursos e, por conseguinte, o modelo de site excede o limite de 50 megabytes (MB).</span><span class="sxs-lookup"><span data-stu-id="f4a7c-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="f4a7c-115">Existem problemas em visualizar dados de uma lista que utiliza uma coluna de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f4a7c-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="f4a7c-116">Para mais informações, consulte a [lista gerada de modelo não apresenta os dados na lista de pesquisa correcta no SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="f4a7c-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="f4a7c-117">Para obter informações mais detalhadas sobre problemas comuns e soluções utilize a referência, [criar e utilizar modelos de site](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="f4a7c-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

