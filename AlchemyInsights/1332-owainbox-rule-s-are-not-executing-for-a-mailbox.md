---
title: 1332 OWA - regra (s) de pasta a receber é não execução de uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306146"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra de pasta a receber não funciona conforme esperado

Verifique se as seguintes definições:
  
- Uma mensagem pode ser redireccionada, reencaminhadas ou respondidas automaticamente com base nas regras da pasta a receber apenas uma vez. Uma regra de redireccionamento (uma regra de pasta a receber ou uma regra de fluxo de correio, também conhecido como uma regra de transporte) pode adicionar um máximo de dez de reencaminhamento de destinatários para uma mensagem. Para mais informações, consulte [os limites de regra de diário, o transporte e a receber](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Regras da pasta a receber não funcionam com a caixa de correio do registo em diário alternativo. Para mais informações sobre a caixa de correio do registo em diário alternativo, consulte a [caixa de correio do registo em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Para corrigir estes problemas, consulte [2829319 da KB](https://support.microsoft.com/kb/2829319).
  
Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de pasta a receber antes de comunicar o problema à Microsoft Support:
  
1. Abrir a caixa de correio no Outlook na web e clique em **Definições** \> **Opções** \> **mensagem de correio electrónico organizar** \> **regras da pasta a receber**.
    
2. Na parte inferior da página, clique em **se as regras não estão a funcionar em clique aqui para gerar um relatório de diagnóstico**.
    

