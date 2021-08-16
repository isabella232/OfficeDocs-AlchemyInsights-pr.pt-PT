---
title: PowerShell do Exchange e depreciação da autenticação básica
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069255"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>PowerShell do Exchange e depreciação da autenticação básica

Para obter as mais recentes informações sobre como ligar à PowerShell do Exchange Online sem a utilização da Autenticação Básica, [aceda aqui](https://aka.ms/exops-docs). O módulo PowerShell v2 não utiliza autenticação básica.

Tenha em atenção que a Autenticação Básica ainda precisa de ser ativada no computador cliente.
O novo módulo PowerShell V2 utiliza a Autenticação Moderna para estabelecer uma ligação que permita todos os Cmdlets V2 baseados em REST. Para além dos cmdlets V2, também lhe permite aceder a Cmdlets da PowerShell Remota (RPS) mais antigos, os quais exigem a criação de uma sessão de PowerShell remota. O estabelecimento de uma sessão de RPS no computador Windows requer a ativação do WinRM BasicAuth no computador cliente, mesmo que o módulo utilize o mecanismo de Autenticação Moderna para autenticar o serviço. O pipeline de Autenticação Básica WinRM é utilizado para o transporte de tokens de Autenticação Moderna. Se a Autenticação Básica WinRM estiver desativada no computador cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets RPS mais antigos não funcionarão).
