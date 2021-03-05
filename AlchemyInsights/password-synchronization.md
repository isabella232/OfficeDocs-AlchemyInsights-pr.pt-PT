---
title: Password synchronization
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482042"
---
# <a name="password-synchronization"></a><span data-ttu-id="645aa-102">Password synchronization</span><span class="sxs-lookup"><span data-stu-id="645aa-102">Password synchronization</span></span>

<span data-ttu-id="645aa-103">**A sincronização de hash de palavra-passe não funciona de todo**</span><span class="sxs-lookup"><span data-stu-id="645aa-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="645aa-104">Algumas questões comuns que os clientes encontram quando a Sincronização de Password Hash não funciona são:</span><span class="sxs-lookup"><span data-stu-id="645aa-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="645aa-105">A conta ative directory utilizada pelo Azure AD Connect para comunicar com o Ative Directory no local não é concedida Alterações de **Diretório de Replica** e **Alterações de Diretório de Replicatos,** que são necessárias para sincronização de palavras-passe - É necessário corrigi-lo concedendo estas permissões à conta ative Directory.</span><span class="sxs-lookup"><span data-stu-id="645aa-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="645aa-106">A sincronização de hash de palavra-passe é desativada depois de um administrador ter alterado o método de Sign-In do Utilizador da Sincronização de **Passwords** para outra opção, como **a Federação com AD FS** no assistente Ad Connect Azure - Pode corrigi-lo, reativando a função de **sincronização de hash de palavra-passe** no assistente Ad Connect Azure.</span><span class="sxs-lookup"><span data-stu-id="645aa-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="645aa-107">Problema de conectividade com o Ative Directory no local.</span><span class="sxs-lookup"><span data-stu-id="645aa-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="645aa-108">Por exemplo, alguns controladores de domínio não estão [acessíveis](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) pelo Azure AD Connect, ou as portas necessárias são bloqueadas pelo Firewall - É necessário corrigi-lo garantindo que a conectividade entre o servidor AZURE AD Connect e o Ative Directory funciona corretamente.</span><span class="sxs-lookup"><span data-stu-id="645aa-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="645aa-109">O servidor AD Connect Azure está atualmente em modo de fase, o que resultará na falta de acesso do servidor às hashes da palavra-passe - Para resolver o problema, siga os passos descritos na secção [Sincronização de palavras-passe de resolução de problemas com sincronização Azure AD Connect - Não há palavras-passe sincronizadas](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="645aa-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="645aa-110">**A sincronização de hash de palavra-passe não funciona para alguns dos meus utilizadores**</span><span class="sxs-lookup"><span data-stu-id="645aa-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="645aa-111">Se notou que o hash da palavra-passe não está a sincronizar um utilizador, utilize a tarefa **de resolução de problemas** no Azure AD Connect para investigar e resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="645aa-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="645aa-112">Executar as seguintes tarefas:</span><span class="sxs-lookup"><span data-stu-id="645aa-112">Perform the following tasks:</span></span>

    <span data-ttu-id="645aa-113">a.</span><span class="sxs-lookup"><span data-stu-id="645aa-113">a.</span></span> [<span data-ttu-id="645aa-114">Executar a tarefa de resolução de problemas no assistente</span><span class="sxs-lookup"><span data-stu-id="645aa-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="645aa-115">b.</span><span class="sxs-lookup"><span data-stu-id="645aa-115">b.</span></span> [<span data-ttu-id="645aa-116">Use o cmdlet de resolução de problemas para investigar o problema de sincronização de haxixe de palavra-passe para uma utilização específica</span><span class="sxs-lookup"><span data-stu-id="645aa-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="645aa-117">O objeto de utilizador ative directy no local está ativado para **o Utilizador deve alterar a palavra-passe na próxima** opção de início de sposição.</span><span class="sxs-lookup"><span data-stu-id="645aa-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="645aa-118">Quando esta opção estiver ativada, o utilizador é atribuído a uma senha temporária e será solicitado a alterar a palavra-passe no próximo início de sessão.</span><span class="sxs-lookup"><span data-stu-id="645aa-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="645aa-119">O Azure AD Connect não sincroniza palavras-passe temporárias para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="645aa-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="645aa-120">Para resolver a questão acima, execute qualquer uma das seguintes tarefas:</span><span class="sxs-lookup"><span data-stu-id="645aa-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="645aa-121">Peça ao utilizador para iniciar sôms na aplicação no local (por exemplo, Windows Desktop) e altere a palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="645aa-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="645aa-122">A nova palavra-passe será sincronizada com a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="645aa-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="645aa-123">Tenha um administrador a atualizar a palavra-passe do utilizador sem permitir a opção O Utilizador deve alterar a **palavra-passe no próximo início de sê-lo** e partilhar a nova palavra-passe com o utilizador.</span><span class="sxs-lookup"><span data-stu-id="645aa-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="645aa-124">O objeto de utilizador ative directory no local não está **corretamente configurado** para sincronização de objetos ou sincronização de palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="645aa-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="645aa-125">Para resolver este problema, siga os passos descritos na [sincronização de hash de palavra-passe de resolução de problemas com a sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="645aa-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







