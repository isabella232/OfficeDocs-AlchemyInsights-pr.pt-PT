---
title: Ativar a repetição de escrita de palavras-passe do Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560451"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="f83a1-102">Ativar a repetição de escrita de palavras-passe do Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f83a1-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="f83a1-103">Para ativar a repetição de escrita de reposição personalizada de palavra-passe, ative primeiro a opção repetição de escrita no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f83a1-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="f83a1-104">A partir do seu servidor do Azure AD Connect, efetue os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="f83a1-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="f83a1-105">Inicie sessão no seu servidor do Azure AD Connect e inicie o assistente de configuração do **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="f83a1-106">Na página de **Boas-vindas**, clique em **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="f83a1-107">Na página **Tarefas adicionais**, selecione **Personalizar opções de sincronização** e, em seguida, clique em **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="f83a1-108">Na página **Ligar ao Azure AD**, introduza uma credencial de administrador global para o seu inquilino do Azure e, em seguida, clique em **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="f83a1-109">Nas páginas de filtragem de **Ligar diretórios** e de **Domínio/UO**, clique em **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="f83a1-110">Na página **Funcionalidades opcionais**, selecione a caixa junto a **Repetição de escrita da palavra-passe** e clique em **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="f83a1-111">Na página **Preparado para configurar**, clique em **Configurar** e aguarde até que o processo seja concluído.</span><span class="sxs-lookup"><span data-stu-id="f83a1-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="f83a1-112">Assim que a configuração estiver terminada, clique em **Sair**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="f83a1-113">Com a repetição de escrita de palavra-passe ativada no Azure AD Connect, configure o Azure AD SSPR para a repetição de escrita.</span><span class="sxs-lookup"><span data-stu-id="f83a1-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="f83a1-114">Para ativar a repetição de escrita de uma palavra-passe no SSPR, efetue os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="f83a1-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="f83a1-115">Inicie sessão no portal do Azure através de uma conta de administrador global.</span><span class="sxs-lookup"><span data-stu-id="f83a1-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="f83a1-116">Procure e selecione o **Azure Active Directory**, clique em **Reposição de palavra-passe** e, em seguida, clique em **Integração no local**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="f83a1-117">Defina a opção **Repetir a escrita de palavras-passe no diretório no local?** como **Sim**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="f83a1-118">Defina a opção **Permitir que os utilizadores desbloqueiem as contas sem repor a palavra-passe?** como **Sim**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="f83a1-119">Quando estiver pronto, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="f83a1-119">When ready, click **Save**.</span></span>

<span data-ttu-id="f83a1-120">Para obter mais informações, consulte [Ativar a repetição de escrita de reposição personalizada de palavra-passe do Azure Active Directory num ambiente no local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="f83a1-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="f83a1-121">Se um administrador redefinir a palavra-passe de um utilizador no portal do Azure, se esse utilizador estiver federado ou tiver sincronização de hash de palavra-passe, a escrita da palavra-passe será repetida no local.</span><span class="sxs-lookup"><span data-stu-id="f83a1-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="f83a1-122">Neste momento, esta funcionalidade não é suportada no portal de Administração do Office.</span><span class="sxs-lookup"><span data-stu-id="f83a1-122">This functionality is currently not supported in the Office Admin portal.</span></span>