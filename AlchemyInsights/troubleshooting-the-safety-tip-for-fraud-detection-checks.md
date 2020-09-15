---
title: Resolução de problemas da ponta de segurança para verificação de deteção de fraudes
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658421"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Resolução de problemas da ponta de segurança para verificação de deteção de fraudes

Se estiver a receber uma dica de segurança que diz "O remetente falhou nas nossas verificações de deteção de fraudes e pode não ser quem parece ser", então o remetente não passou nem verificações de autenticação DKIM ou SPF. O melhor método para resolver isto é o remetente autorizar-se a si próprio. Se o remetente estiver a enviar em seu nome, tem de os autorizar adicionando o endereço IP do remetente ao seu registo SPF.
  
Consulte [a resolução de problemas da ponta de segurança vermelha (suspeita) para verificação de fraudes](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obter mais informações.
  
Aqui estão outros links que podem ajudar:
  
- [Como a Microsoft usa o quadro de política de remetente (SPF) para evitar falsificações](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Criar SPF para ajudar a prevenir a falsificação](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
