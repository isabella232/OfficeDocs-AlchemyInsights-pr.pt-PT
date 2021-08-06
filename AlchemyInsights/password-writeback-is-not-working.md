---
title: A Escrita de Palavra-passe não está a funcionar
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
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999755"
---
# <a name="password-writeback-is-not-working"></a>A Escrita de Palavra-passe não está a funcionar

**Estou a ter problemas com a configuração do writeback da palavra-passe**

- O writeback por palavra-passe é uma funcionalidade premium.
- Certifique-se de que compreende os requisitos de licenciamento:
  - Tem de ter pelo menos uma licença atribuída na sua organização
  - **Apenas utilizadores na nuvem** – Office 365 SKU pago (O365) ou Azure AD Basic
  - **Utilizadores da nuvem e/ou** no local : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Para saber mais sobre os requisitos de licenciamento, consulte Requisitos de licenciamento para a reposição de palavra-passe de responsabilidade do [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Tem, pelo menos, uma conta de administrador e uma conta de utilizador de teste com uma das licenças adequadas.
- Tem de ligar o Azure AD Ligação ao Controlador de Domínio Principal Emulator que a escrita de palavra-passe funcione. Pode configurar o Azure AD Ligação para utilizar um Controlador de  Domínio Principal ao clicar com o botão direito do rato nas propriedades do conector de sincronização do Active Directory e, em seguida, selecionar configurar partições de **diretório.** A partir daí, procure a secção definições de ligação do **controlador** de domínio e marque a caixa intitulada utilizar apenas controladores **de domínio preferenciais.**
  > [!NOTE]
  > Se o DC preferido não for um emulador PDC, o Azure AD Ligação continuará a contactar o PDC para escrever a palavra-passe.
- A reposição da palavra-passe foi configurada e ativada no seu inquilino. Para obter mais informações, consulte Permitir [que os utilizadores reporem as respetivas palavras-passe do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Certifique-se de que a conta de administrador que está a ser utilizada para ativar o Writeback da Palavra-passe é uma conta de administrador na nuvem (criada no Azure AD e não no AD no local)
- Tem uma implementação única ou multi-floresta do AD no local a executar o Windows Server 2008 R2, Windows Server 2012 ou Windows Server 2012 R2 com os service packs mais recentes instalados
- Tem a ferramenta Azure AD Ligação instalada e preparou o seu ambiente de AD para sincronização com a nuvem. Antes de testar a escrita da palavra-passe, certifique-se de que primeiro conclui uma importação completa e uma sincronização completa do AD e do Azure AD no Azure Ligação.
- Para saber mais, veja como e quanto uma sincronização completa e a importação [completa no Azure AD Ligação](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Estou a ter um problema com a conectividade de escrita de palavra-passe**

1. Transferir e ativar a versão mais [recente do Azure AD Ligação](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuração da firewall: a ferramenta Azure AD Ligação (1.1.443 e superior) necessita de acesso **HTTPS** de saída para:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Permitir que as ligações inativos persistam durante, pelo menos, 2 a 3 minutos

**Ainda estou a ter problemas com a escrita de palavras-passe**

- Se continuar a ter dificuldades, experimente desativar e reativar o serviço de escrita de palavras-passe na ferramenta de comentários do Azure AD Ligação.
- Para saber mais, veja como desativar [e reativar o writeback da palavra-passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
