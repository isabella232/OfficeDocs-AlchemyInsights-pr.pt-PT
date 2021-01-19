---
title: Problemas de problemas com os utilizadores
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901334"
---
# <a name="announcements"></a>Anúncios

Siga as orientações da Google sobre a compatibilidade dos testes para testar se as suas apps estão afetadas. A orientação da Google está disponível em https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Certifique-se de que utiliza o webview do sistema ou o navegador do sistema ao assinar nos seus utilizadores com contas google de consumo. Para obter mais informações, consulte [Problemas de sessão de sessão para aplicações usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Não posso criar um novo utilizador no meu diretório AD Azure**

Para resolver problemas com a questão de não ser capaz de criar um novo utilizador em Azure AD, execute os seguintes passos:

1. Certifique-se de que está autorizado a criar um novo utilizador padrão. Apenas o papel de administrador global ou administrador de utilizador no Azure Ative Directory (AD) pode criar um novo utilizador padrão. Se não estiver numa destas funções, peça a um administrador que o adicione a uma destas funções ou que crie a nova conta de utilizador para si.
2. Certifique-se de que o nome de utilizador está num domínio verificado no seu AD Azure. Se não tiver nenhum nome de domínio personalizado verificado no seu AD Azure, pode utilizar o seu domínio inicial AD Azure, que termina com *.onmicrosoft.com.
3. Certifique-se de que o nome de utilizador está num domínio que não é federado para Azure AD a partir do seu AD no local. Os utilizadores não podem ser adicionados na nuvem com nomes de domínio que são federados do local.
4. Certifique-se de que nenhum outro utilizador ou contacto já tem o nome de utilizador que pretende atribuir ao novo utilizador. Os nomes de utilizador devem ser únicos em todo o Azure AD.
5. Consulte [as funções e administradores da AD Azure](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu AZure AD.
6. Consulte os [nomes de domínio](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) do seu AD Azure.
7. [Reveja os registos de auditoria](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) para ver informações mais detalhadas sobre um utilizador recentemente criado ou eliminado, como quem realizou a ação e quando.
8. Para obter mais informações sobre a adição de novos utilizadores, consulte [utilizar o portal Azure para criar um novo utilizador no seu AD Azure.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
9. Para obter mais informações sobre permissões de função de administrador em Azure AD, consulte [as funções administrativas da AZure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Para obter mais informações sobre a criação de um utilizador que utilize a Azure AD Powershell, consulte [a Azure AD PowerShell para criar um novo utilizador](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problema com a inscrição de self-service**

Para resolver problemas no que diz respeito à inscrição de self-service, execute os seguintes passos:

1. Para utilizar a inscrição de self-service com as suas aplicações, primeiro ative a inscrição de self-service para o seu inquilino. 
2. Para ativar uma aplicação para suportar a inscrição de self-service, adicione-a ao fluxo do seu utilizador . Da próxima vez que for à página de login para essa aplicação, verá uma opção **_Sem conta? Criar um!_* _. Isto inicia o processo de inscrição de autosserviço.
3. Para obter informações sobre como usar o self-service inscreva-se para preencher uma organização em Azure AD, consulte [o Self-service inscreva-se para Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Uma vez associado o fluxo do utilizador a uma ou mais aplicações, os utilizadores que visitarem essa aplicação poderão inscrever-se e obter uma conta de hóspedes utilizando as opções configuradas no fluxo do utilizador. Para obter mais informações sobre a inscrição e a obtenção de uma conta de hóspedes, os utilizadores podem ver [a inscrição de Self-service para utilizadores convidados.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)

_ *Problema de convidar um utilizador externo**

Para resolver problemas em relação à convidar um utilizador externo, execute o seguinte passo:

Certifique-se de que envia o convite de um utilizador para o endereço de e-mail que corresponde ao nome com o qual o utilizador assina. Se enviar o convite para o endereço de e-mail de procuração de um utilizador, o utilizador não pode resgatá-lo. Para mais informações, consulte [a documentação do Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Não posso atribuir licenças a um utilizador.**

Para resolver problemas relativos à atribuição de licenças a um utilizador, execute os seguintes passos:

1. Para gerir as licenças de utilizador, certifique-se de que utiliza uma conta com uma das funções de administrador necessárias: administrador global, administrador de licença ou administrador do utilizador. Pode verificar a função do utilizador no **separador função** do Diretório na lâmina do utilizador.
2. Se estiver a utilizar o portal Azure e a atribuição da licença estiver a falhar, clique na notificação no canto superior direito. Isto abre uma lâmina com detalhes sobre o que correu mal. Na maioria dos casos, isso é suficiente para compreender e resolver o problema.
3. Antes de uma licença poder ser atribuída a um utilizador, certifique-se de que a propriedade **De Localização de Utilização** está definida para o utilizador. Verifique se o utilizador tem a propriedade definida visualizando o **separador Perfil** na lâmina do utilizador.
4. Certifique-se de que existem licenças disponíveis suficientes para o produto que está a tentar atribuir. Pode ver o número de licenças disponíveis no portal Azure, no [Azure Ative Directory -> Licenses -> Todos os produtos](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. O utilizador pode já ter outra licença cujos serviços entram em conflito com os da nova licença que está a tentar atribuir. Por exemplo, se o utilizador tiver o serviço Exchange Online (Plano 1) ativado, não poderá atribuir uma licença ao Exchange Online (Plano 2). Desative um dos serviços para permitir a nova atribuição de licença. Se estiver a utilizar o portal Azure ou os cmdlets PowerShell, a página de detalhes do **problema** lista os serviços específicos que estão a causar o conflito.
6. Se estiver a tentar remover uma licença e isso estiver a falhar, o utilizador poderá ter outras licenças com serviços que dependem dos serviços que está a tentar remover. Se estiver a utilizar o portal Azure ou os cmdlets PowerShell, a mensagem de erro listará os serviços específicos que têm dependências.
7. Se quiser entender por que uma licença foi adicionada/removida de um utilizador (por exemplo, quem mais na sua organização pode ter feito alterações), verifique os registos de auditoria. Desatrei o filtro às **atividades de licença** para mostrar todas as modificações, incluindo o "ator" que as executou.
8. Se estiver a utilizar o Exchange Online, alguns utilizadores do seu inquilino podem estar configurados incorretamente com o mesmo valor de endereço proxy. Nesses casos, pode ver mensagens de erro genéricas quando uma operação de licença falha. [Este artigo](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contém mais informações sobre este problema, incluindo informações sobre [como ligar-se ao Exchange Online utilizando o PowerShell remoto.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) Para identificar quais utilizadores no seu inquilino, conter o mesmo endereço de procuração, execute este cmdlet Exchange Online:

Correr

Get-Recipient | onde {$_. EmailAddresses -match <user principal name> } | nome fL, RecipientType,emailaddresses





