---
title: Monitorizar o Acesso Condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975112"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorizar o Acesso Condicional para Exchange

Os utilizadores aosdos terão acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização. Para resolver o problema, recomendamos que utilize uma ou mais das seguintes soluções:

- Se o dispositivo estiver predisposta a ser inscrito, receba o utilizador para ir para a aplicação Portal da Empresa e verifique se aparece na Portal da Empresa. Se isso não acontecer, o utilizador deverá inscrever o dispositivo.
- No portal do Azure, vá para Intune > Conformidade do dispositivo. Em Monitorização, clique em Conformidade do dispositivo. Veja o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme.
- No portal do Azure, vá para Intune > Conformidade do dispositivo. Em Gerir, clique em Políticas. Na lista de políticas de conformidade, verifique se está atribuído um perfil ao dispositivo do utilizador. Se não for atribuído nenhum perfil, o Intune não conseguirá confirmar o estado de conformidade do dispositivo.
- Edite a atribuição de acesso condicional do utilizador.

1. No portal do Azure, aceda a Políticas de Acesso Condicional do **Intune.**  >    >  
2. Selecione uma política a partir da lista.
3. Clique em Utilizadores e grupos.
4. Para atingir uma determinada política, adicione-a à lista Incluir. Para se certificar de que uma pessoa é omitida da política, adicione-a à lista Excluir.

Ligações úteis:

[Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Remoção de Problemas da AC](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de remoção de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorizar a conformidade do dispositivo Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: estes passos só são úteis na remoção de problemas na Azure Active Directory Acesso Condicional à funcionalidade. Também é possível bloquear um dispositivo ao bloquear o seu acesso de e-mail com uma Exchange restrita. Mais informações sobre como Exchange gestão de dispositivos podem ser encontradas [aqui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
