---
title: Migração de AIP para MIP/Etiquetagem Unificada no Centro de Conformidade
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000367"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migração de AIP para MIP/Etiquetagem Unificada no Centro de Conformidade

Para migrar de etiquetas AIP para Etiquetas Unificadas no Centro de Conformidade e Segurança, faça o seguinte:

**Ativar proteção a partir do portal do Azure**

1. Caso ainda não o tenha feito, abra uma nova janela do browser e [inscreva-se no portal do Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Navegue até ao blade **do Azure Information Protection.** Por exemplo, no menu central, clique em Todos **os serviços** e comece a escrever **Informações** na caixa Filtro. **Selecione Azure Information Protection.** Se ainda não acedeu ao blade do Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection, consulte os passos adicionais únicos para adicionar esta porta ao portal. Para abrir o blade do Azure Information Protection, tem de ter um plano [do Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou um plano de Office 365 que inclua a Gestão de Direitos. Se tiver uma destas subscrições, mas vir uma mensagem a dizer que não é possível encontrar uma subscrição válida, [contacte](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) o Suporte da Microsoft ou utilize os seus canais de suporte padrão.

2. Localize **as opções do** menu Gerir e selecione **Ativação da proteção.** Clique em **Ativar** e, em seguida, confirme a sua ação. Quando a ativação estiver concluída, a barra de informações apresenta **Ativação concluída com êxito.**

**Migrar as etiquetas do Azure Information Protection para Office 365 Centro & Conformidade e Segurança**

1. Certifique-se de que tem sessão de utilizador com permissão de Administrador Global.

2. Navegue até ao blade **do Azure Information Protection.**

3. A partir da **opção** de menu Gerir, selecione **Etiqueta unificada**.

4. Na folha **de etiquetagem do Azure Information Protection - Unified,** clique em **Ativar** e siga as instruções online.

**Nota:** verifique se tem as permissões adequadas antes de ativar a Migração do Centro & conformidade. Consulte estes artigos para mais informações:

1. [Tem de ser um administrador global para configurar o Azure Information Protection ou posso delegar para outros administradores?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informações importantes sobre funções administrativas depois de migrar para o Centro de & conformidade.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Para obter mais informações sobre a migração de Etiquetas Unificada para o Centro de Conformidade e Segurança, consulte [Migrar etiquetas.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
