---
title: Monitor Intune Acesso Condicional
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427926"
---
# <a name="monitor-intune-conditional-access"></a>Monitor Intune Acesso Condicional

Os utilizadores direcionados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

1. Caso se presuma que o dispositivo esteja matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e verificar se aparece no Portal da Empresa. Se não o fizer, o utilizador deve inscrever o dispositivo.
1. No portal Azure aceda à conformidade do Dispositivo **Intune**  >  . 
1. Para ver o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme, no **Monitor**, clique na **conformidade do Dispositivo**.
1. No portal Azure aceda à conformidade do Dispositivo **Intune**  >  . Em **Gestão,** clique em **Políticas**. Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do seu utilizador. Se não for atribuído nenhum perfil, o Intune não poderá confirmar o estado de conformidade do dispositivo.
1. Editar a atribuição de acesso condicional do utilizador.
1. No portal Azure, navegue para Políticas de Acesso Condicionado **Intune**  >    >  , selecione uma política da lista e clique em **Utilizadores e grupos**.
1. Para direcionar uma determinada política a alguém, adicione-a à **lista Incluindo.** Para garantir que uma pessoa é omitida da apólice, adicione-a à **lista de exclusão**.

**Links úteis:**

- [Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Resolução de problemas CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Política de resolução de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorização da conformidade do dispositivo Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Estes passos só são úteis para resolver problemas na resolução do recurso Azure Ative Directory Conditional Access. Também é possível colocar em quarentena um dispositivo que bloqueia o seu acesso por e-mail com a política de Troca. Mais informações sobre a gestão do dispositivo Exchange podem ser [**encontradas aqui.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
