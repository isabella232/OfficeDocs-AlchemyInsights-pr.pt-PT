---
title: Os indicadores não funcionam com o browser Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326272"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Os indicadores não funcionam com o browser Edge

Depois de criar um Indicador, este não é honrado pelo Edge (Smartscreen). Para obter mais informações, [consulte Criar indicadores para IPs e URLs/domínios.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Passo 1: certifique-se de que o seguinte

- Verifique se o indicador está correto (sem erros de digitação em IP/URL, a ação correta, os grupos RBAC corretos).
- Aguarde pelo menos 2 horas após criar o indicador para ter em conta qualquer latência possível.
- Confirme que o(s) sistema(s) está ativo(s) no Microsoft Defender para Endpoint.
- Verifique se o(s) sistema(s) pode comunicar com a Nuvem.
- Verifique se o Smartscreen está ativado e acessível ao ir para o [site de teste.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Passo 2: remoção do possível problema

- Certifique-se de que o cliente cumpre os requisitos. Para obter detalhes, [consulte Criar indicadores para IPs e URLs/domínios.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Certifique-se de que está a executar a versão mais recente do browser Edge. Para saber qual é a versão mais recente, [consulte Saber que versão do Microsoft Edge que tem.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Reinicie o browser Edge.
- Navegue para o site para o qual tem um indicador de configuração. Se o site não aparecer como esperado, continue para o Passo 3. 

## <a name="step-3-collect-data"></a>Passo 3: recolher dados

- Recolha **dados de diagnóstico do MDEClientAnalyzer.** Para obter instruções, consulte [Problemas com máquinas de iboard no Microsoft Defender para Endpoint.](issues-with-onboarding-machines.md)
- Se estiver à vontade a instalar e a recolher um rastreio Do Fiddler, consulte [Telerik Fiddler.](http://www.telerik.com/fiddler)
- Se preferir orientação do Suporte da Microsoft, selecione o ícone de Suporte abaixo para abrir um caso de suporte.
