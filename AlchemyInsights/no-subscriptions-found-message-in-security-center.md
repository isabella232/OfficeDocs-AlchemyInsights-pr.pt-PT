---
title: Nenhuma mensagem de subscrições encontrada no Centro de Segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544119"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Nenhuma mensagem de subscrições encontrada no Centro de Segurança

Se ao aceder ao Centro de Segurança do Microsoft Defender receber a mensagem "Não foram encontradas subscrições", significa que o Azure Active Directory (AAD) utilizado para loginar o utilizador no portal não tem uma licença Microsoft Defender ATP.  

Os Windows E5 e Office E5 são licenças separadas.

Abra um caso de suporte se a licença tiver sido comprada, mas não tiver sido aprovisionada para esta instância do AAD. Tem: <br/>
-   Um possível problema de aprovisionamento de licenças.<br/>
-   Aprovisionou inadvertidamente a licença para um Microsoft AAD diferente da que foi utilizada para a autenticação no serviço.