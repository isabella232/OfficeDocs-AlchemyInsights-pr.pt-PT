---
title: Problema com grupos de segurança
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177629"
---
# <a name="issue-with-security-groups"></a>Problema com grupos de segurança

**Se estiver a receber O Erro de Rede AADDS104**

As regras do grupo de segurança da rede inválidas são a causa mais comum de erros de rede para os Serviços de Domínio do Diretório Ativo Azure (DS AD). O grupo de segurança da rede virtual deve permitir o acesso a portas e protocolos específicos. Se estas portas estiverem bloqueadas, a plataforma Azure não pode monitorizar ou atualizar o domínio gerido. A sincronização entre o Azure AD e o Azure AD DS também é impactada. Certifique-se de que mantém as portas padrão abertas para evitar interrupções no serviço.

Para compreender e resolver alertas comuns para problemas de configuração do grupo de segurança de rede, consulte [Grupos de Segurança Adicionar e Verificar](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
