---
title: Corrigir aplicações da Microsoft 365 Não conseguiu encontrar licenças de escritório associadas mensagem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816499"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Correção da mensagem "Não consegui encontrar licenças de escritório associadas" da Microsoft

Se receber esta mensagem, experimente o seguinte:

1. Verifique as definições de firewall, antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações da Microsoft 365. Consulte [os intervalos de endereços MICROSOFT 365 URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Remova e [reatribua a licença do Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para o utilizador afetado. 
3. Abra uma aplicação do Office e [assine fora](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de quaisquer contas de utilizador existentes.
4. Vá às Definições do Windows > **Contas**  >  **Enviar por email & contas** e remova todas as contas de trabalho, exceto a conta afetada.
5. Vá às Definições do Windows > **Contas**  >  **Aceder ao trabalho ou à escola**, e desligar todas as contas de trabalho, exceto a conta afetada.
6. Reponha o estado de ativação do Office. [Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Inscreva-se utilizando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) a conta de utilizador afetada.

Para obter soluções adicionais de resolução de problemas, consulte [erros de produto não licenciados e erros de ativação no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).