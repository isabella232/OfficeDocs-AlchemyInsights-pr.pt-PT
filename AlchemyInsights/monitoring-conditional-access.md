---
title: Acesso Condicional de Monitorização
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708685"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorização do Acesso Condicional para Troca

Os utilizadores direcionados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

- Caso se presuma que o dispositivo esteja matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e verificar se aparece no Portal da Empresa. Se não o fizer, o utilizador deverá inscrever o dispositivo.
- No portal Azure vai para a conformidade do Dispositivo Intune >. No Monitor clique na conformidade do dispositivo. Consulte o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme.
- No portal Azure vai para a conformidade do Dispositivo Intune >. Em Gestão, clique em Políticas. Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do seu utilizador. Se não for atribuído nenhum perfil, o Intune não poderá confirmar o estado de conformidade do dispositivo.
- Editar a atribuição de acesso condicional do utilizador.

1. No portal Azure aceda às Políticas de Acesso Condicionado **Intune**  >    >  .
2. Selecione uma política da lista.
3. Clique em Utilizadores e grupos.
4. Para direcionar uma determinada política a alguém, adicione-a à lista de incluir. Para garantir que uma pessoa é omitida da apólice, adicione-a à lista de exclusão.

Links úteis:

[Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Resolução de problemas CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de resolução de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorização da conformidade do dispositivo Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: estes passos só são úteis para resolver problemas na resolução do Azure Ative Directory recurso Acesso Condicional. Também é possível colocar em quarentena um dispositivo que bloqueia o seu acesso por e-mail com a política de Troca. Mais informações sobre a gestão de dispositivos Exchange podem ser encontradas https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) [aqui].
