---
title: Regras de redução da superfície de ataque
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676439"
---
# <a name="attack-surface-reduction-rules"></a>Regras de redução da superfície de ataque

Excluir ficheiros ou pastas pode reduzir gravemente a proteção fornecida pelas regras de redução da superfície de ataque. Os ficheiros que teriam sido bloqueados por uma regra têm permissão para ser executados e não é registado nenhum relatório ou evento. Uma exclusão aplica-se a todas as regras que permitem exclusões.

As exclusões ASR utilizam a mesma sintaxe que as Antivírus do Microsoft Defender exclusões. Para obter detalhes, [consulte Configurar e validar exclusões para Antivírus do Microsoft Defender análises.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Para evitar problemas, [reveja erros comuns a evitar ao definir exclusões](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Nem todas as regras ASR suportam exclusões. Para validar se a sua regra suporta exclusões, consulte a tabela Regras de redução da [superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regras de redução da superfície de ataque

A superfície de ataque da sua organização inclui todos os locais onde um atacante pode comprometer os dispositivos ou redes da organização. Reduzir a sua superfície de ataque significa proteger os dispositivos e a rede da organização, o que deixa os atacantes com menos formas de efetuar ataques. Configurar regras de redução da superfície de ataque no Microsoft Defender para Pontos Finais pode ajudar.

Para mais informações, consulte:

- [Mapear GUID da regra ASR para nome](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Requisitos de regras ASR:
    - [Windows 10 Pro, versão 1709 ou posterior](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versão 1709 ou posterior](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Servidor, versão 1803 (Via de Atualizações Semesuais) ou posterior](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identificar a exclusão correta a aplicar

1. Procure o eventID 1121 ou 1122 no registo Microsoft-Windows-Windows Defender/Operacional.

1. Avalie o cenário e o contexto do bloqueio e confirme que este cenário tem de ser desbloqueado.

1. Leia o valor Caminho nos detalhes do evento, que é o valor que define a exclusão.
    - Tornar a exclusão o mais estrita possível.
    - Aplicar um cartão wildcard onde for necessário (por exemplo, substituir variável de Utilizador).

1. Aplique a exclusão de acordo com as suas necessidades de implementação. Para obter detalhes, consulte [Personalizar regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>A exclusão não é honrada

1. Determine se a regra suporta exclusões. Para obter detalhes, consulte Regras de redução [da superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Reveja as exclusões aplicadas e verifique com os dados do evento se existem erros tipográficos ou comnados. Para mais informações, consulte Tipos de [exclusão suportados](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. se o impacto da regra for demasiado elevado, considere mover a regra (para trás) para o Modo de auditoria para efetuar uma validação posterior. Para obter detalhes, consulte [Testar como o Microsoft Defender para funcionalidades do Endpoint funciona em modo de auditoria.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Recolha dados de suporte para abrir um caso de suporte utilizando este comando:
    
   ** MDEClientAnalyzer.cmd -v**

    Para obter mais informações, consulte [Problemas com os sistemas de iboarding no Microsoft Defender para Pontos finais.](issues-with-onboarding-machines.md)
