---
title: Criar um site SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515009"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="5ca77-102">Criar sites do SharePoint utilizando modelos</span><span class="sxs-lookup"><span data-stu-id="5ca77-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="5ca77-103">Modelos de site do SharePoint são definições previamente concebidas destinadas em torno de uma determinada necessidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="5ca77-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="5ca77-104">Para mais informações, consulte [utilizar modelos para criar diferentes tipos de sites do SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="5ca77-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="5ca77-105">Eis algumas questões/soluções comuns relativas ao guardar um Site ou lista como um modelo no Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="5ca77-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="5ca77-106">**Botão de modelo de site/lista de guardar não está disponível ou em falta**</span><span class="sxs-lookup"><span data-stu-id="5ca77-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="5ca77-107">Os administradores serão necessário permitir Script personalizado para activar as funcionalidades do modelo.</span><span class="sxs-lookup"><span data-stu-id="5ca77-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="5ca77-108">Para obter informações detalhadas, consulte os exemplos e considerações</span><span class="sxs-lookup"><span data-stu-id="5ca77-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="5ca77-109">Permitir ou impedir que o script personalizado</span><span class="sxs-lookup"><span data-stu-id="5ca77-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="5ca77-110">O site de guardar como comando de modelo não é suportado e pode causar problemas em sites que utilizem a infra-estrutura de publicação do SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="5ca77-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="5ca77-111">**O modelo de site não é possível criar ou não funciona correctamente**</span><span class="sxs-lookup"><span data-stu-id="5ca77-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="5ca77-112">O modelo pode estar em falta uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não vai activar.</span><span class="sxs-lookup"><span data-stu-id="5ca77-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="5ca77-113">Se a funcionalidade não está disponível para activar a colecção de sites actual, é possível utilizar o modelo de site para criar um site.</span><span class="sxs-lookup"><span data-stu-id="5ca77-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="5ca77-114">Verifique se todas as listas ou bibliotecas de excederem o [Limiar de limite de vista de lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, como este pode bloquear a criação de um modelo de site.</span><span class="sxs-lookup"><span data-stu-id="5ca77-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="5ca77-115">O site poderá estar a utilizar demasiados recursos e, por conseguinte, o modelo de site excede o limite de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="5ca77-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="5ca77-116">Existem problemas em visualizar dados de uma lista que utiliza uma coluna de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="5ca77-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="5ca77-117">Para mais informações, consulte a [lista gerada de modelo não apresenta os dados na lista de pesquisa correcta no SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="5ca77-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="5ca77-118">Para obter informações mais detalhadas sobre problemas e soluções comuns, consulte [criar e utilizar modelos de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="5ca77-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



