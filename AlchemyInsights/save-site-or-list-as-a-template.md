---
title: Guardar site ou lista como um modelo
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727542"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="fa864-102">Guardar site ou lista como um modelo</span><span class="sxs-lookup"><span data-stu-id="fa864-102">Save site or list as a template</span></span>

<span data-ttu-id="fa864-103">Os modelos do site SharePoint são definições pré-construídas desenhadas em torno de uma necessidade de negócio particular.</span><span class="sxs-lookup"><span data-stu-id="fa864-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="fa864-104">Para obter mais informações, consulte [utilizar modelos para criar diferentes tipos de sites SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="fa864-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="fa864-105">Aqui estão algumas questões/soluções comuns sobre a poupança de um site ou lista como um modelo no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fa864-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="fa864-106">**O botão de modelo de site/lista não está disponível ou em falta**.</span><span class="sxs-lookup"><span data-stu-id="fa864-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="fa864-107">Os administradores terão de permitir o Script Personalizado para ativar as funcionalidades do modelo.</span><span class="sxs-lookup"><span data-stu-id="fa864-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="fa864-108">Para etapas detalhadas, exemplos e considerações consulte [Permitir ou impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="fa864-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="fa864-109">O site Save como comando de modelo não é suportado e pode causar problemas em sites que usam a Infraestrutura de Publicação do Servidor SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fa864-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="fa864-110">**O modelo do site não pode ser criado ou não funciona corretamente**</span><span class="sxs-lookup"><span data-stu-id="fa864-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="fa864-111">O modelo pode estar a perder uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado.</span><span class="sxs-lookup"><span data-stu-id="fa864-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="fa864-112">Se a funcionalidade não estiver disponível para ser ativada na recolha atual do site, não poderá utilizar o modelo do site para criar um site.</span><span class="sxs-lookup"><span data-stu-id="fa864-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="fa864-113">Verifique se alguma lista ou biblioteca excede o limiar limite de [visualização](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de lista de 5000 itens, uma vez que isso pode bloquear a criação de um modelo de site.</span><span class="sxs-lookup"><span data-stu-id="fa864-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="fa864-114">O site pode estar a usar demasiados recursos e, portanto, o modelo do site excede o limite de 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="fa864-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="fa864-115">Existem problemas em apresentar dados de uma lista que utiliza uma coluna de procuração.</span><span class="sxs-lookup"><span data-stu-id="fa864-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="fa864-116">Para obter mais informações, consulte [a lista gerada por Modelos não exibe dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="fa864-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="fa864-117">Para obter informações mais detalhadas sobre problemas e soluções comuns, consulte, [crie e use modelos de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="fa864-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

