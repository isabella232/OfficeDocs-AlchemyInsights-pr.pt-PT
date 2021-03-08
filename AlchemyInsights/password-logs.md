---
title: Registos de palavra-passe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527178"
---
# <a name="password-logs"></a>Registos de palavra-passe

**Estou com problemas em aceder a registos de auditoria de redefinição de passwords**

Para resolver problemas no que diz respeito ao acesso aos registos de auditoria de redefinição de passwords, execute o seguinte passo:

Certifique-se de que está autorizado a visualizar os registos de auditoria. 

Apenas são autorizadas as seguintes funções:
 - Administrador global
 - Administrador de segurança
 - Leitor de segurança

**Quero ver todos os eventos de auditoria de redefinição de passwords a partir do momento em que inicialmente desloquei**

Até 120.000 eventos de reset/registo de passwords são armazenados nos relatórios dos últimos 30 dias. Este limite máximo aplica-se à UI ao descarregar o CSV. 1 milhão de eventos estão disponíveis através do PowerShell.
Para mais informações, consulte os links abaixo:

- [Autosserviço de autosserviço redefinir eventos da AZure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Como descarregar eventos de registo de redefinição de password rapidamente com o PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Quero saber mais sobre as capacidades de reporte de redefinição de passwords**

Verifique quem está a registar ou a redefinir palavras-passe com registos de auditoria de redefinição de password AD do Azure no portal Azure sob **Utilizadores e grupos**.
Para mais informações, consulte os seguintes links:

- [Relatórios de reset de palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Como visualizar relatórios de reset de palavra-passe no portal Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Autosserviço de autosserviço redefinir eventos da AZure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Como descarregar eventos de registo de redefinição de password rapidamente com o PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


