---
title: Problema com o Estado de Ligação AAD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923763"
---
# <a name="problem-with-aad-connect-health"></a>Problema com o Estado de Ligação AAD

- Certifique-se de que está autorizado a efetuar a operação. Os Administradores Globais têm acesso por predefinição. Além disso, pode utilizar o Controlo de [Acesso Baseado em Funções](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) para delegar permissões de registo ao Contribuinte.
- Certifique-se de que os pontos finais obrigatórios estão ativados e não bloqueados devido à firewall. Para obter detalhes, consulte [os requisitos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- O registo pode falhar devido à comunicação de saída ser sujeita à inspeção SSL pela camada de rede.
- Certifique-se de que verificou as definições de notificação do Azure AD Ligação Estado de Ligação Estado de Trabalho. Reveja a sua definição. Este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pode ajudá-lo a compreender como configurar as definições de notificação do Azure AD com Ligação de estado de vida.
- Para saber mais sobre o relatório de sincronização do Ligação Estado de Trabalho do AAD e sobre como transferi-lo, consulte Relatório de [sincronização ao nível do objeto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Para remoção de alertas de Saúde do AAD Ligação, siga o guia de remoção de problemas do [AAD Ligação Alertas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) de estado de saúde de alertas e, para perguntas mais frequentes, consulte Perguntas mais frequentes sobre a instalação do [AAD Ligação Estado](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)de Saúde.
