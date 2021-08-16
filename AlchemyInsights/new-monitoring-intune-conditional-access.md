---
title: Monitorizar o Acesso Condicional do Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025513"
---
# <a name="monitor-intune-conditional-access"></a>Monitorizar o Acesso Condicional do Intune

Os utilizadores aosdos terão acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização. Para resolver o problema, recomendamos que utilize uma ou mais das seguintes soluções:

1. Se o dispositivo estiver predisposta a ser inscrito, receba o utilizador para ir para a aplicação Portal da Empresa e verifique se aparece na Portal da Empresa. Se isso não acontecer, o utilizador terá de inscrever o dispositivo.
1. No portal do Azure, vá para **Conformidade do dispositivo Intune.**  >   
1. Para ver o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme, em **Monitorização**, clique em Conformidade **do dispositivo**.
1. No portal do Azure, vá para **Conformidade do dispositivo Intune.**  >   Em **Gerir, clique** em **Políticas**. Na lista de políticas de conformidade, verifique se está atribuído um perfil ao dispositivo do utilizador. Se não for atribuído nenhum perfil, o Intune não conseguirá confirmar o estado de conformidade do dispositivo.
1. Edite a atribuição de acesso condicional do utilizador.
1. No portal do Azure, navegue até Políticas de Acesso Condicional do **Intune,** selecione uma política a partir da lista e clique em Utilizadores  >    >   **e grupos**.
1. Para atingir uma determinada política a alguém, adicione-a à **lista Incluir.** Para se certificar de que uma pessoa é omitida da política, adicione-a à **lista Excluir.**

**Ligações úteis:**

- [Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Remoção de Problemas da AC](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Política de remoção de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorizar a conformidade do dispositivo Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Estes passos só são úteis na remoção da Azure Active Directory funcionalidade Acesso Condicional. Também é possível bloquear um dispositivo ao bloquear o seu acesso de e-mail com uma Exchange restrita. Pode encontrar mais informações Exchange gestão de dispositivos [**aqui.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
