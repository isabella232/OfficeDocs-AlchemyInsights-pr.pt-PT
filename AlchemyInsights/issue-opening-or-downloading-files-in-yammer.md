---
title: Emissão de abrir ou descarregar ficheiros em Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148337"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="ba92a-102">Emissão de abrir ou descarregar ficheiros em Yammer</span><span class="sxs-lookup"><span data-stu-id="ba92a-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="ba92a-103">A Classic Yammer suporta múltiplas opções para uploads de ficheiros para mensagens e grupos.</span><span class="sxs-lookup"><span data-stu-id="ba92a-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="ba92a-104">Dependendo da configuração da rede, os ficheiros predefinição para armazenamento no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ba92a-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="ba92a-105">O selecionador de ficheiros em novo Yammer ainda não suporta todas as opções disponíveis no clássico Yammer.</span><span class="sxs-lookup"><span data-stu-id="ba92a-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="ba92a-106">Uma futura atualização irá adicionar funcionalidades adicionais.</span><span class="sxs-lookup"><span data-stu-id="ba92a-106">A future update will add additional features.</span></span> <span data-ttu-id="ba92a-107">Para obter mais informações, consulte [anexar um ficheiro ou imagem a um post de conversação Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="ba92a-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="ba92a-108">**Incapaz de abrir ou descarregar um ficheiro**</span><span class="sxs-lookup"><span data-stu-id="ba92a-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="ba92a-109">Um ficheiro pode ser enviado para o Yammer, mas também estar ligado a um ficheiro no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ba92a-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="ba92a-110">Para resolver problemas, primeiro tem de determinar a localização do ficheiro.</span><span class="sxs-lookup"><span data-stu-id="ba92a-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="ba92a-111">Se o ficheiro tiver sido enviado para o Yammer, terá uma URL de yammer.com.</span><span class="sxs-lookup"><span data-stu-id="ba92a-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="ba92a-112">Certifique-se de que os URLs e endereços IP necessários estão desbloqueados.</span><span class="sxs-lookup"><span data-stu-id="ba92a-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="ba92a-113">Para obter mais informações, consulte o post de blog [Usando endereços IP codificados para Yammer não é recomendado](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="ba92a-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="ba92a-114">Verifique se um utilizador que também é administrador global pode descarregar o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="ba92a-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="ba92a-115">Se o ficheiro for privado, poderá ter de utilizar o Modo de Conteúdo Privado.</span><span class="sxs-lookup"><span data-stu-id="ba92a-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="ba92a-116">Para obter mais informações, consulte então [monitorize o conteúdo privado em Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="ba92a-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="ba92a-117">**Hóspedes e ficheiros ao nível da rede Yammer no SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="ba92a-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="ba92a-118">[Os hóspedes de nível de rede em Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) não usam Azure AD B2B e são internos ao serviço Yammer, por isso não podem aceder aos ficheiros Yammer armazenados no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ba92a-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="ba92a-119">Crie um utilizador AAD B2B externo que possa aceder a bibliotecas documentais no SharePoint Online utilizando essa identidade.</span><span class="sxs-lookup"><span data-stu-id="ba92a-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="ba92a-120">Para obter informações sobre o futuro suporte de hóspedes Azure AD B2B em Yammer, consulte [suporte de clientes Business-to-Business (B2B) em Yammer Preview - Termos do Cliente e FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="ba92a-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>