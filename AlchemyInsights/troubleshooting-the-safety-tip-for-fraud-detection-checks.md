---
title: A sugestão de segurança para detecção de fraudes de resolução de problemas verifica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533209"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>A sugestão de segurança para detecção de fraudes de resolução de problemas verifica

Se estiver a obter uma sugestão de segurança que indica "o remetente falhou o nosso controlos de detecção de fraudes e poderá não ser que o que parecem estar", em seguida, o remetente falhou a transmissão de DKIM ou SPF verificações de autenticação. É o melhor método para resolver este problema para o remetente autorizar próprios. Se o remetente está a enviar em seu nome, terá de lhes confira adicionando o endereço IP do remetente ao registo SPF.
  
Para obter mais informações, consulte [a sugestão de segurança (suspeitas) vermelho para detecção de fraudes de resolução de problemas verifica](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Eis algumas hiperligações que podem ajudar:
  
- [Como o Office 365 utiliza o quadro de política de emissor (SPF) para impedir a fraude de identidade](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar SPF no Office 365 para ajudar a impedir o spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
