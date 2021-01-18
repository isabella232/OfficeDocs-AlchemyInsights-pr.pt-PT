---
title: Emissão juntando VMs
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885665"
---
# <a name="issue-joining-vms"></a>Emissão juntando VMs

Para resolver problemas que ocorrem ao tentar juntar VMs, execute os seguintes passos:

1. Tente iniciar sação utilizando o formato **UPN** (por exemplo, 'joeuser@contoso.com') em vez do formato **SAMAccountName** ('CONTOSO\joeuser').
2. Certifique-se de que ativou a sincronização da palavra-passe de acordo com os passos descritos no guia *'Iniciar'.*
3. Certifique-se de que a conta de utilizador afetada não é uma conta externa no inquilino AZURE AD. Os utilizadores externos não podem entrar no domínio gerido, uma vez que os Serviços de Domínio AD Azure não têm credenciais para essas contas de utilizador.
4. Se a conta de utilizador afetada for uma conta de utilizador exclusivamente na nuvem, certifique-se de que os utilizadores alteraram a sua palavra-passe depois de ter ativado os Serviços de Domínio Azure AD. Este passo faz com que os haques credenciais necessários para que os Serviços de Domínio AD AD do Azure sejam gerados.
5. Se as contas de utilizador afetadas forem sincronizadas a partir de um diretório no local, verifique se a libertação recomendada do Azure AD Connect foi configurada para realizar uma sincronização completa.
6. Se os problemas persistirem após confirmar o Passo 4, execute os seguintes comandos da sua máquina de sincronização:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.