---
title: Mudar de microsoft nameservers para gerir os seus próprios registos DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506969"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Mudar de microsoft nameservers para gerir os seus próprios registos DNS

Alterou anteriormente os seus registos NS para apontar para Microsoft (ns1.bdm.microsoftonline.com), mas decidiu agora gerir os seus próprios registos DNS:

No Site da sua pessoa de registo de domínios, altere novamente o servidor de nomes para a sua registo de domínios ou para a definição anterior. Se não está familiarizado com DNS, contacte o suporte da entidade de registo de domínios. Tenha em atenção que as alterações dos nomes podem demorar até 48 horas a propagar. 

1. No portal Microsoft 365 administração, vá a **Definições**, selecione a caixa de verificação junto ao domínio e  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **selecione Gerir DNS.** 

2. No assistente, selecione **Adicionar os seus próprios registos DNS e** conclua o assistente. Esta ação altera a forma como o seu DNS é gerido e, em seguida, permite-lhe adicionar os registos DNS personalizados necessários para suportar os serviços selecionados.

Em alternativa, se alterou os registos do seu serviço de nomes para a Microsoft e tem um site, pode adicionar registos DNS para o site em vez de alterar os nomes de volta. Para obter mais informações, consulte [Atualizar os registos DNS para manter o seu site junto do seu fornecedor de anfitrião atual.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


