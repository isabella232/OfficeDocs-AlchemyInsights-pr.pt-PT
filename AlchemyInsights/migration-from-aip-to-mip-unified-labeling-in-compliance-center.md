---
title: Migração da AIP para mOP/Rotulagem Unificada no Centro de Conformidade
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674337"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="bdaa2-102">Migração da AIP para mOP/Rotulagem Unificada no Centro de Conformidade</span><span class="sxs-lookup"><span data-stu-id="bdaa2-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="bdaa2-103">Para migrar das etiquetas AIP para a Rotulagem Unificada no centro de Segurança e Conformidade, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="bdaa2-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="bdaa2-104">**Ativar a proteção a partir do portal Azure**</span><span class="sxs-lookup"><span data-stu-id="bdaa2-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="bdaa2-105">Se ainda não o fez, abra uma nova janela do navegador e [inscreva-se no portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="bdaa2-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="bdaa2-106">Navegue para a lâmina **de proteção de informação Azure.**</span><span class="sxs-lookup"><span data-stu-id="bdaa2-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="bdaa2-107">Por exemplo, no menu do hub, clique em **Todos os serviços** e comece a escrever **Informações** na caixa filtro.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="bdaa2-108">Selecione **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="bdaa2-109">Se ainda não acedeu à lâmina de Proteção de Informação Azure, consulte os [passos adicionais](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) de uma vez para adicionar esta lâmina ao portal.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="bdaa2-110">Para abrir a lâmina de proteção de informação Azure, deve ter um [plano Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou um plano Office 365 que inclua a Gestão de Direitos.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="bdaa2-111">Se tiver uma destas subscrições, mas vir uma mensagem de que não é possível encontrar uma subscrição válida, [contacte o Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ou utilize os seus canais de suporte padrão.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="bdaa2-112">Localize as opções do menu **Gerir** e selecione **ativação de proteção**.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="bdaa2-113">Clique **em Ativar**e, em seguida, confirme a sua ação.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="bdaa2-114">Quando a ativação estiver concluída, a barra de informação mostra **a ativação terminada com sucesso**.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="bdaa2-115">**Migrar etiquetas de proteção de informação do Azure para o Office 365 Security & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="bdaa2-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="bdaa2-116">Certifique-se de que está a iniciar sessão como um utilizador com permissão de Administrador Global.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="bdaa2-117">Navegue para a lâmina **de proteção de informação Azure.**</span><span class="sxs-lookup"><span data-stu-id="bdaa2-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="bdaa2-118">A partir da opção menu **Gerir,** selecione **a rotulagem unificada.**</span><span class="sxs-lookup"><span data-stu-id="bdaa2-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="bdaa2-119">Na **Proteção de Informações Azure - Lâmina de rotulagem unificada,** clique em **Ativar** e siga as instruções on-line.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="bdaa2-120">**Nota:** Verifique se tem as permissões adequadas antes de ativar a migração do Centro de Conformidade & de Segurança.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="bdaa2-121">Consulte estes artigos para mais informações:</span><span class="sxs-lookup"><span data-stu-id="bdaa2-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="bdaa2-122">Precisa de ser um administrador global para configurar a Azure Information Protection, ou posso delegar a outros administradores?</span><span class="sxs-lookup"><span data-stu-id="bdaa2-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="bdaa2-123">Informações importantes sobre funções administrativas após migração para o Centro de Conformidade & de Segurança.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="bdaa2-124">Para obter mais informações sobre a migração da AIP para a rotulagem unificada para o Centro de Segurança e Conformidade, consulte [as etiquetas Migrate](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="bdaa2-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
