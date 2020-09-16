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
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migração da AIP para mOP/Rotulagem Unificada no Centro de Conformidade

Para migrar das etiquetas AIP para a Rotulagem Unificada no centro de Segurança e Conformidade, faça o seguinte:

**Ativar a proteção a partir do portal Azure**

1. Se ainda não o fez, abra uma nova janela do navegador e [inscreva-se no portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navegue para a lâmina **de proteção de informação Azure.** Por exemplo, no menu do hub, clique em **Todos os serviços** e comece a escrever **Informações** na caixa filtro. Selecione **Azure Information Protection**. Se ainda não acedeu à lâmina de Proteção de Informação Azure, consulte os [passos adicionais](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) de uma vez para adicionar esta lâmina ao portal. Para abrir a lâmina de proteção de informação Azure, deve ter um [plano Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou um plano Office 365 que inclua a Gestão de Direitos. Se tiver uma destas subscrições, mas vir uma mensagem de que não é possível encontrar uma subscrição válida, [contacte o Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ou utilize os seus canais de suporte padrão.

2. Localize as opções do menu **Gerir** e selecione **ativação de proteção**. Clique **em Ativar**e, em seguida, confirme a sua ação. Quando a ativação estiver concluída, a barra de informação mostra **a ativação terminada com sucesso**.

**Migrar etiquetas de proteção de informação do Azure para o Office 365 Security & Compliance Center**

1. Certifique-se de que está a iniciar sessão como um utilizador com permissão de Administrador Global.

2. Navegue para a lâmina **de proteção de informação Azure.**

3. A partir da opção menu **Gerir,** selecione **a rotulagem unificada.**

4. Na **Proteção de Informações Azure - Lâmina de rotulagem unificada,** clique em **Ativar** e siga as instruções on-line.

**Nota:** Verifique se tem as permissões adequadas antes de ativar a migração do Centro de Conformidade & de Segurança. Consulte estes artigos para mais informações:

1. [Precisa de ser um administrador global para configurar a Azure Information Protection, ou posso delegar a outros administradores?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informações importantes sobre funções administrativas após migração para o Centro de Conformidade & de Segurança.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Para obter mais informações sobre a migração da AIP para a rotulagem unificada para o Centro de Segurança e Conformidade, consulte [as etiquetas Migrate](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
