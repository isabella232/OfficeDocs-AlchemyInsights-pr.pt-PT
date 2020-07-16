---
title: Problemas de carregamento de imagem de resolução de problemas em Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148295"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="238aa-102">Problemas de carregamento de imagem de resolução de problemas em Yammer</span><span class="sxs-lookup"><span data-stu-id="238aa-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="238aa-103">Quando ocorrem problemas com fotos e pré-visualizações de ficheiros no Yammer, a resolução de problemas verificando se o problema ocorre para todos os utilizadores, se ocorre em dispositivos móveis e se é reprodutível ao carregar o anexo.</span><span class="sxs-lookup"><span data-stu-id="238aa-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="238aa-104">**Questões de fotos de perfil**</span><span class="sxs-lookup"><span data-stu-id="238aa-104">**Profile photo issues**</span></span>  

<span data-ttu-id="238aa-105">Se os utilizadores finais assinarem no Yammer via Microsoft 365, devem alterar o seu perfil, incluindo a sua foto de perfil.</span><span class="sxs-lookup"><span data-stu-id="238aa-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="238aa-106">Se os utilizadores não estiverem autorizados a fazer atualizações de perfil, um administrador pode fazer a atualização para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="238aa-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="238aa-107">Para mais informações, consulte [Ver e atualizar o seu perfil no Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="238aa-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="238aa-108">Para obter informações sobre a edição de perfis, incluindo fotos de perfil, consulte [Alterar o meu perfil e configurações de Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="238aa-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="238aa-109">As fotos de perfil atualizadas são sincronizadas de forma diferente dos atributos do perfil.</span><span class="sxs-lookup"><span data-stu-id="238aa-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="238aa-110">Os utilizadores devem iniciar uma sincronização da sua foto de perfil.</span><span class="sxs-lookup"><span data-stu-id="238aa-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="238aa-111">Para obter informações, consulte [as imagens do perfil do utilizador atualizadas do Office 365 para Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="238aa-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="238aa-112">Para obter informações sobre o ciclo de vida do utilizador para a Yammer, consulte [os utilizadores da Manage Yammer através do seu ciclo de vida a partir do Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="238aa-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="238aa-113">Para obter mais detalhes sobre como funciona a sincronização de imagens de perfil no Microsoft 365, consulte [informações sobre a sincronização de imagens de perfil na Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="238aa-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="238aa-114">**Pré-visualizações de documentos e problemas de miniatura de imagem**</span><span class="sxs-lookup"><span data-stu-id="238aa-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="238aa-115">Quando os ficheiros ou imagens são publicados no Yammer, as pré-visualizações podem não aparecer porque:</span><span class="sxs-lookup"><span data-stu-id="238aa-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="238aa-116">O ficheiro é corrupto e não pode ser processado.</span><span class="sxs-lookup"><span data-stu-id="238aa-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="238aa-117">O ficheiro não foi recentemente enviado para o SharePoint Online, ou o Yammer tem metadados inválidos por outras razões.</span><span class="sxs-lookup"><span data-stu-id="238aa-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="238aa-118">Os URLs necessários para o carregamento das imagens de pré-visualização estão bloqueados.</span><span class="sxs-lookup"><span data-stu-id="238aa-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="238aa-119">A pré-visualização do ficheiro foi removida pelo utilizador antes de ser publicada.</span><span class="sxs-lookup"><span data-stu-id="238aa-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="238aa-120">Um problema de serviço impediu que se gerasse uma pré-visualização.</span><span class="sxs-lookup"><span data-stu-id="238aa-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="238aa-121">**Nota** As pré-visualizações de links e uploads de ficheiros podem comportar-se de forma diferente.</span><span class="sxs-lookup"><span data-stu-id="238aa-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="238aa-122">As ligações a ficheiros na internet ou links que exijam autenticação adicional podem não ser apresentados corretamente.</span><span class="sxs-lookup"><span data-stu-id="238aa-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="238aa-123">Para obter mais informações, consulte [anexar um ficheiro ou imagem a uma mensagem Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="238aa-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 