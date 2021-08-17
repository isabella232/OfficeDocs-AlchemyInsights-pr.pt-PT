---
title: Encontrar aplicações em falta no blade Registo de Aplicações
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057113"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Encontrar aplicações em falta no blade Registo de Aplicações

1. Não é possível encontrar aplicações no portal de Registo de Aplicações.

    Se uma aplicação for uma aplicação multi-inquilino e tiver sido registada noutro inquilino, não será apresentada com a folha de Registo de Aplicações. No entanto, pode encontrá-la no campo Enterprise Applications depois de este ser acededo (após o consentimento) e o principal de serviço tiver sido criado no seu inquilino. Para obter mais informações, consulte [Aplicações & principais de serviço no Azure AD - plataforma de identidades da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Apesar de ser um administrador, não é possível ver aplicações na folha Registo de Aplicações.

    Certifique-se de que está no diretório certo no portal do Azure.
3. A minha aplicação não está listada no blade Enterprise Applications, mas é mostrada quando consulta o comando PowerShell.

    Por vezes, depois de eliminar a aplicação do portal do Azure, esta não é mostrada no portal, mas poderá não ter sido eliminada completamente. Para mais informações, consulte:
    - Pode obter a lista de aplicações eliminadas anteriormente e ver se a aplicação aparece na lista com o comando PowerShell: **Get-AzureADDeletedApplication**. Para saber mais, consulte [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Se quiser remover completamente a aplicação, pode experimentar o seguinte no PowerShell: **Remove-AzureADApplication -ObjectID.** Para saber mais, consulte [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Em alternativa, pode tentar restaurar a aplicação eliminada através do seguinte comando do PowerShell: **Restaurar AzureADDeletedApplication -ObjectID.** Para saber mais, consulte [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Não consigo encontrar uma lista de todas as aplicações empresariais pré-instaladas no meu novo inquilino do Azure.

    Por predefinição, não existem aplicações empresariais pré-instaladas no Azure AD. Tem de a adicionar manualmente a partir da opção "Nova aplicação" ao navegar na mesma a partir da galeria do Azure AD ou adicionar uma aplicação que não seja de galeria. Para saber mais, consulte Guia de Utilização: Adicionar uma aplicação ao [seu inquilino do Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Se for um administrador global, pode aceder facilmente às suas aplicações através do Iniciador [Microsoft 365 Aplicações](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Não é possível encontrar as minhas aplicações a partir do portal As Minhas Aplicações.

    Certifique-se de que as aplicações não estão ocultas na página da coleção As Minhas Aplicações. Para saber mais, consulte [Coleções (pré-visualização) no portal as Minhas Aplicações – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Para iniciar aplicações a partir do portal As Minhas Aplicações, consulte Localizar e & utilizar aplicações no portal As Minhas [Aplicações – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 A aplicação Mover não é mostrada no blade Enterprise Applications após a instalação.

    A aplicação "Office 365 Mover" é uma aplicação multi-inquilino que não precisa de ser adicionada ao AAD através da secção Aplicações de Galeria em Registo de Aplicações de Empresa. Para aceder Office 365 aplicação Mover, basta inscrever-se na aplicação e pedir o consentimento do utilizador para as permissões. Assim que o utilizador fornecer o consentimento, esta aplicação será automaticamente adicionada ao inquilino com o ID de e-mail em que tem sessão sessão.

    Após ter entrado na aplicação, deverá conseguir encontrar a entrada desta aplicação por baixo da porta Do Enterprise Applications no AAD. Tem de procurar essa aplicação ao escrever o nome completo, ou seja, "Mover Office 365 ou simplesmente procurar "office" e esta deverá listar a aplicação. Para saber mais, consulte Office 365 Mover diz que já está instalado, mas não está listado na galeria [Aplicação Empresarial](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).
8. Guia de Utilização Rápida: Ver a lista de aplicações que estão a utilizar o seu inquilino do [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) para gestão de identidades mostra-lhe como ver as aplicações, também conhecidas como aplicações, que já estão configuradas para utilizar o seu inquilino do Azure AD como fornecedor de Identidade (IdP).
9. [Resolver problemas comuns ao](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) adicionar ou remover uma aplicação ao Azure Active Directory ajuda-o a compreender os problemas comuns que as pessoas enfrentam ao ver aplicações no Azure Active Directory.
