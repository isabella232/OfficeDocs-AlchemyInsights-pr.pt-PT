---
title: Utilizar um site WiX com domínios comprados ou geridos do Office 365
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
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825958"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utilizar um site WiX com domínios comprados ou geridos do Office 365

- [Atualizar os registos DNS para manter o seu site junto do seu fornecedor de alojamento atual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- O artigo WiX "A ligar um Domínio ao WiX através do Método Apontador" recomenda utilizar o apontador (adicionar registos DNS por cima da ligação) em vez de mudar os nomes dos servidores ao utilizar o Office 365
- Se ainda decidir alterar os servidores de nomes para o WiX, terá de  [Criar registos DNS em WiX para a Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Se o seu domínio foi comprado da Microsoft, não é possível alterar os servidores de nomes. Se tiver de mudar os servidores de nomes, o domínio comprado da Microsoft teria de ser  [transferido para outro fornecedor de alojamento após 60 dias](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)