---
title: Receção de sugestão de segurança para verificações de deteção de fraude
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955977"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Receção de sugestão de segurança para verificações de deteção de fraude

Se estiver a obter um sugestão de segurança que diz "O remetente falhou as nossas verificações de deteção de fraude e pode não ser quem aparentam ser", isso significa que o remetente não passou nas verificações de autenticação DKIM ou SPF. O melhor método para resolver este problema é que o remetente se autorize a si próprio. Se o remetente for enviado em seu nome, tem de autorizá-lo ao adicionar o endereço IP do remetente ao seu registo SPF.
  
Consulte [Remoção de problemas de sistema vermelhos (suspeitos) sugestão de segurança verificações de fraude para](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) mais informações.
  
Eis algumas outras ligações que podem ajudar:
  
- [Como a Microsoft utiliza o SPF (Sender Policy Framework) para impedir o spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar SPF para ajudar a impedir o spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
