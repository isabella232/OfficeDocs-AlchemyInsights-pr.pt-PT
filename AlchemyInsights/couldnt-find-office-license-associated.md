---
title: Corrigir Microsoft 365 aplicações Não foi conseguir encontrar a mensagem associada a licenças do Office
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069615"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Corrigir a mensagem Microsoft 365 aplicações "Não foi foi consegui encontrar licenças do Office associadas"

Se receber esta mensagem, experimente o seguinte:

1. Verifique a sua firewall, software antivírus e definições de proxy para confirmar que não estão a bloquear o acesso à Internet a Microsoft 365 aplicações. Consulte [Microsoft 365 intervalos de URLs e endereços IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. [Remova e reatrilhe a Office licença do](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) utilizador afetado. 
3. Abra um aplicação do Office e [terme em](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) qualquer conta de utilizador existente.
4. Vá para o Windows Definições > **Contas de** e& e remova todas as contas de trabalho  >  exceto a conta afetada.
5. Aceda às Windows Definições > **Escolar ou** Escolar do Access e desligue todas as contas de trabalho  >  exceto a conta afetada.
6. Reponha o estado de ativação do Office. [Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Inscreva-se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) com a conta de utilizador afetada.

Para obter soluções de remoção de problemas adicionais, consulte [Erros](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)Produto Não Office .