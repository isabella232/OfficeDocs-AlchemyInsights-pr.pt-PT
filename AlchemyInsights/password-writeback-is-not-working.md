---
title: A writeback da palavra-passe não está a funcionar
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243519"
---
# <a name="password-writeback-is-not-working"></a>A writeback da palavra-passe não está a funcionar

**Estou com problemas em configurar a gravação de passwords.**

- A gravação de palavra-passe é uma característica premium.
- Certifique-se de que compreende os requisitos de licenciamento:
  - Deve ter pelo menos uma licença atribuída na sua organização
  - **Utilizadores da Cloud -** Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic
  - **Utilizadores em nuvem e/ou no local** - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)
    - Para saber mais sobre os requisitos de licenciamento, consulte [os requisitos de licenciamento para reposição da palavra-passe de autosserviço Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Tem pelo menos uma conta de administrador e uma conta de utilizador de teste com uma das licenças apropriadas.
- Tem de ligar o Azure AD Connect ao Emulador do Controlador de Domínio Primário para que a gravação da palavra-passe funcione. Pode configurar o Azure AD Connect para utilizar um Controlador de Domínio Primário clicando nas **propriedades** do conector de sincronização do Diretório Ativo e, em seguida, selecionando **divisórias de diretório de configuração**. A partir daí, procure a secção de **definições de conexão do controlador de domínio** e verifique a caixa intitulada **apenas utilizar controladores de domínio preferidos**.
  > [!NOTE]
  > Se o DC preferido não for um emulador PDC, o Azure AD Connect ainda contactará o PDC para obter a gravação de passwords.
- O reset da palavra-passe foi configurado e ativado no seu inquilino. Para obter mais informações, consulte [Ativar os utilizadores para redefinir as suas palavras-passe AD Azure](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Certifique-se de que a conta de administrador utilizada para ativar o Writeback de Password é uma conta de administrador em nuvem (criada em AD Azure e não no local AD)
- Tem uma implementação de AD de uma única ou multi-floresta no local com o Windows Server 2008 R2, Windows Server 2012 ou Windows Server 2012 R2 com os mais recentes pacotes de serviços instalados
- Tem a ferramenta Azure AD Connect instalada e preparou o seu ambiente AD para sincronização na nuvem. Antes de testar a gravação da palavra-passe, certifique-se de que primeiro completa uma importação completa e sincronização completa tanto da AD como da AZure AD no Azure AD Connect.
- Para saber mais, veja como fazer uma [sincronização completa e importação completa em Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Estou tendo um problema com a conectividade de gravação de palavra-passe**

1. Faça o download e ative a versão mais recente do [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuração de firewall: A ferramenta Azure AD Connect (1.1.443 ou superior) necessitará de acesso **HTTPS de saída** para:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Deixe que as ligações inativas permaneçam durante pelo menos 2-3 minutos

**Ainda estou com problemas com a gravação da palavra-passe.**

- Se ainda tiver dificuldades, tente desativar e voltar a ativar o serviço de writeback de palavra-passe na ferramenta Azure AD Connect
- Para saber mais, veja como [desativar e ativar o writeback de palavras-passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
