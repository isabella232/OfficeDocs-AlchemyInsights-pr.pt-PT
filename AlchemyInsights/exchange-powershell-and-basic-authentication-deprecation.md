---
title: PowerShell do Exchange e depreciação da autenticação básica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015700"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>PowerShell do Exchange e depreciação da autenticação básica

Para obter as mais recentes informações sobre como ligar à PowerShell do Exchange Online sem a utilização da Autenticação Básica, [aceda aqui](https://aka.ms/psbasicauth).

Tenha em atenção que a Autenticação Básica ainda precisa de ser ativada no computador cliente.
O novo módulo PowerShell V2 utiliza a Autenticação Moderna para estabelecer uma ligação que permita todos os Cmdlets V2 baseados em REST. Para além dos cmdlets V2, também lhe permite aceder a Cmdlets da PowerShell Remota (RPS) mais antigos, os quais exigem a criação de uma sessão de PowerShell remota. O estabelecimento de uma sessão de RPS no computador Windows requer a ativação do WinRM BasicAuth no computador cliente, mesmo que o módulo utilize o mecanismo de Autenticação Moderna para autenticar o serviço. O pipeline de Autenticação Básica WinRM é utilizado para o transporte de tokens de Autenticação Moderna. Se a Autenticação Básica WinRM estiver desativada no computador cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets RPS mais antigos não funcionarão).
