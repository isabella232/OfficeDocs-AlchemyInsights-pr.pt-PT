---
title: Criar um site no SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732246"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="de42e-102">Criar sites sharePoint usando modelos</span><span class="sxs-lookup"><span data-stu-id="de42e-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="de42e-103">A capacidade de salvar um site como modelo não é suportada com comunicações modernas ou sites de equipa.</span><span class="sxs-lookup"><span data-stu-id="de42e-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="de42e-104">Para obter mais informações sobre a utilização de modelos [consulte Guardar, transferir e carregar um site do SharePoint como modelo.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)</span><span class="sxs-lookup"><span data-stu-id="de42e-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="de42e-105">Aqui estão algumas questões/soluções comuns sobre guardar um site ou lista como um modelo no Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="de42e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="de42e-106">**O botão de modelo de site/lista não está disponível ou em falta**</span><span class="sxs-lookup"><span data-stu-id="de42e-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="de42e-107">Os administradores terão de permitir o Script Personalizado para ativar as funcionalidades do modelo.</span><span class="sxs-lookup"><span data-stu-id="de42e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="de42e-108">Para passos, exemplos e considerações detalhadas ver</span><span class="sxs-lookup"><span data-stu-id="de42e-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="de42e-109">Permitir ou prevenir script personalizado</span><span class="sxs-lookup"><span data-stu-id="de42e-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="de42e-110">O site Save como comando de modelo não é suportado e pode causar problemas em sites que usam a Infraestrutura de Publicação do Servidor SharePoint.</span><span class="sxs-lookup"><span data-stu-id="de42e-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="de42e-111">**O modelo do site não pode ser criado ou não funciona corretamente**</span><span class="sxs-lookup"><span data-stu-id="de42e-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="de42e-112">O modelo pode estar a perder uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado.</span><span class="sxs-lookup"><span data-stu-id="de42e-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="de42e-113">Se a funcionalidade não estiver disponível para ser ativada na recolha atual do site, não poderá utilizar o modelo do site para criar um site.</span><span class="sxs-lookup"><span data-stu-id="de42e-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="de42e-114">Verifique se alguma lista ou biblioteca excede o limiar limite de [visualização](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de lista de 5000 itens, uma vez que isso pode bloquear a criação de um modelo de site.</span><span class="sxs-lookup"><span data-stu-id="de42e-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="de42e-115">O site pode estar a usar demasiados recursos e, portanto, o modelo do site excede o limite de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="de42e-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="de42e-116">Existem problemas em apresentar dados de uma lista que utiliza uma coluna de procuração.</span><span class="sxs-lookup"><span data-stu-id="de42e-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="de42e-117">Para obter mais informações, consulte [a lista gerada por Modelos não exibe dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="de42e-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="de42e-118">Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique [criar e utilizar modelos do site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="de42e-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



