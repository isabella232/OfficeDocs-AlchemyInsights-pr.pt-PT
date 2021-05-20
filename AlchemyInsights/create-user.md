---
title: Criar utilizador
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569758"
---
# <a name="create-user"></a>Criar utilizador

**ANÚNCIO:**

- O suporte para o início de trabalho do WebView da Google a partir de [4 de janeiro de 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Teste se as suas aplicações podem ser afetadas ao seguir [as orientações da Google](https://go.microsoft.com/fwlink/?linkid=2157323) sobre a compatibilidade de testes.
- Certifique-se de que utiliza a visualização Web do sistema ou o browser do sistema ao entrar nos seus utilizadores com contas Google de consumidor. Para obter mais informações, [consulte o artigo Problemas ao entrar na(s) aplicação(s) a utilizar apenas o browser Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Não consigo criar um novo utilizador no meu diretório do Azure AD**

1. Certifique-se de que está autorizado a criar um novo utilizador padrão. Apenas a função Administrador global ou Administrador de utilizador no Azure Active Directory (AD) pode criar um novo utilizador padrão. Se não estiver numa destas funções, peça a um administrador para o adicionar a uma destas funções ou para criar a nova conta de utilizador.
1. Certifique-se de que o nome de utilizador está num domínio verificado no seu Azure AD. Se não tiver nomes de domínio personalizados verificados no seu Azure AD, pode utilizar o seu domínio inicial do Azure AD, que termina com *.onmicrosoft.com.
1. Certifique-se de que o nome de utilizador está num domínio que não está federado para o Azure AD a partir do seu AD no local. Os utilizadores não podem ser adicionados à nuvem com nomes de domínios federados a partir do local.
1. Certifique-se de que nenhum outro utilizador ou contacto já tem o nome de utilizador que pretende atribuir ao novo utilizador. Os nomes de utilizador têm de ser exclusivos no Azure AD.
1. Consulte [Funções e administradores do Azure AD para](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) o seu Azure AD.
1. Consulte os [nomes de domínio](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) do seu Azure AD.
1. [Reveja registos de](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) auditoria para ver informações mais detalhadas sobre um utilizador recentemente criado ou eliminado, como quem efetuou a ação e quando.
1. Para obter mais informações sobre como adicionar novos utilizadores, consulte Utilizar o portal do Azure para criar um novo utilizador no [seu Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Funções administrativas do Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)permissões de função de administrador Azure Active Directory
1. Também pode utilizar [o Azure AD PowerShell para criar um novo utilizador.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
