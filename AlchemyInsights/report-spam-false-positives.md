---
title: Quer denunciar um falso positivo de spam à Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396626"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Tem mensagens legítimas que estão a ser marcadas como spam?

É frustrante quando um e-mail legítimo é enviado para a pasta Lixo ou na Quarentena. Considere estes motivos mais comuns para falsos positivos:

**Substitui inquilinos (mais comum)** Esta situação está totalmente dentro do seu controlo para remediar.

Submeta a mensagem Microsoft 365 Defender para análise das políticas e regras afetadas; os detalhes rescan estão disponíveis dentro de minutos.
Reveja ou modifique as políticas ou regras conforme aplicável. 

**Substituições do Utilizador Final (comum)** Esta situação está totalmente dentro do seu controlo para remediar. 

Submeta a mensagem Microsoft 365 Defender para análise das políticas e regras afetadas; os detalhes rescan estão disponíveis dentro de minutos. 

Se uma mensagem foi bloqueada por ter sido enviada a partir de um endereço da lista de Remetentes Bloqueados de um utilizador, os cabeçalhos incluem o Veredito de Filtragem de Spam "SFV:BLK".

**Autenticação de e-mail dos recetores** Esta situação está parcialmente dentro do seu controlo para remediar.

Submeta a mensagem para analisar falhas na autenticação de e-mail do remetente no momento da entrega; os resultados estão disponíveis dentro de um dia. 

Se possui a infraestrutura de envio, reveja como alinhar com SPF, DKIM e DMARC para se certificar de que os sistemas de e-mail de destino confiam nas mensagens enviadas a partir do seu domínio. Em alternativa, contacte os re destinatários para endereçarem as suas configurações de DNS.

**Vereditos de filtragem da Microsoft** Esta situação está parcialmente dentro do seu controlo para remediar.

Submeter a mensagem e denunciar a mensagem como segura; Os resultados rescan estão disponíveis dentro de um dia. Utilize a Lista de Bloqueios/Por Inquilinos quando não concordar com os vereditos de filtragem em situações específicas. No entanto, não deve ultrapassar permanentemente a filtragem de vereditos da Microsoft. 

Para mais informações, consulte:

- Permitir que os seus utilizadores finais submetam mensagens à Microsoft. A Microsoft utiliza estas submissões para melhorar a eficácia das tecnologias de proteção de e-mail e aparecem em relatórios de submissão para utilizar como indicação para atualizar políticas. 

- Para ver um breve vídeo sobre como submeter mensagens para análise, consulte [Submeter mensagens para análise.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Utilizar Submissão de Administrador para submeter suspeitas de spam, phish, URLs e ficheiros à Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Gerir a Lista de Acesso/Bloqueio do Inquilino](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Cabeçalhos de mensagens antisspam no Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Proteção contra spam no EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)