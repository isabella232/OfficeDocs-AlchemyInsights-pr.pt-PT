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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747023"
---
# <a name="create-user"></a>Criar utilizador

**ANÚNCIO:**

- [Depreciação do suporte de sing-in webView do Google a partir de 4 de janeiro de 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Teste se as suas apps podem ser afetadas seguindo a [orientação da Google](https://go.microsoft.com/fwlink/?linkid=2157323) sobre a compatibilidade dos testes.
- Certifique-se de que utiliza o webview do sistema ou o navegador do sistema ao assinar nos seus utilizadores com contas google de consumo. Para obter mais informações, consulte [Problemas de sessão de sessão para aplicações usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Não posso criar um novo utilizador no meu diretório AD Azure**

1. Certifique-se de que está autorizado a criar um novo utilizador padrão. Apenas o administrador global ou o papel de administrador do utilizador no Azure Ative Directory (AD) podem criar um novo utilizador padrão. Se não estiver numa destas funções, peça a um administrador que o adicione a uma destas funções ou que crie a nova conta de utilizador para si.
1. Certifique-se de que o nome de utilizador está num domínio verificado no seu AD Azure. Se não tiver nenhum nome de domínio personalizado verificado no seu AD Azure, pode utilizar o seu domínio inicial AD Azure, que termina com *.onmicrosoft.com.
1. Certifique-se de que o nome de utilizador está num domínio que não é federado para Azure AD a partir do seu AD no local. Os utilizadores não podem ser adicionados na nuvem com nomes de domínio que são federados do local.
1. Certifique-se de que nenhum outro utilizador ou contacto já tem o nome de utilizador que pretende atribuir ao novo utilizador. Os nomes de utilizador devem ser únicos em todo o Azure AD.
1. Consulte [as funções e administradores da AD Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu AZure AD.
1. Consulte os [nomes de domínio](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) do seu AD Azure.
1. [Reveja os registos de auditoria](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para ver informações mais detalhadas sobre um utilizador recentemente criado ou eliminado, como quem realizou a ação e quando.
1. Para obter mais informações sobre a adição de novos utilizadores, consulte [utilizar o portal Azure para criar um novo utilizador no seu AD Azure.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Funções administrativas Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Permissões de função de administrador no Azure Ative Directory
1. Também pode [utilizar o Azure AD PowerShell para criar um novo utilizador](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
