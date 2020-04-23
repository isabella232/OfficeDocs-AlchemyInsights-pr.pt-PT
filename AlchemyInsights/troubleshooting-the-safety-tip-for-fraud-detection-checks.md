---
title: Resolução de problemas da dica de segurança para controlos de deteção de fraudes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759523"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Resolução de problemas da dica de segurança para controlos de deteção de fraudes

Se está a receber uma dica de segurança que diz "O remetente falhou nas nossas verificações de deteção de fraude sem ser quem eles parecem ser", então o remetente não passou nem as verificações de autenticação DKIM ou SPF. O melhor método para resolver isto é que o remetente se autorize. Se o remetente estiver a enviar em seu nome, tem de os autorizar adicionando o endereço IP do remetente ao seu registo SPF.
  
Consulte [a resolução de problemas da ponta de segurança vermelha (suspeita) para verificar](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) a deteção de fraudes para obter mais informações.
  
Aqui estão outros links que podem ajudar:
  
- [Como a Microsoft usa o quadro de política do remetente (FpS) para evitar a falsificação](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar SPF para ajudar a prevenir a falsificação](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
