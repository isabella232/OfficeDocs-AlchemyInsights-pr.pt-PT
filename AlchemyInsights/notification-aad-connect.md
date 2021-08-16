---
title: Notificação AAD Ligação
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
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097317"
---
# <a name="notification-aad-connect"></a>Notificação AAD Ligação

- Certifique-se de que está autorizado a efetuar a operação. Os Administradores Globais têm acesso por predefinição. Além disso, pode utilizar o Controlo de [Acesso Baseado em Funções](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) para delegar permissões de registo ao Contribuinte.
- Certifique-se de que os pontos finais obrigatórios estão ativados e não bloqueados devido à firewall. Para obter detalhes, consulte [os requisitos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- O registo pode falhar devido à comunicação de saída ser sujeita à inspeção SSL pela camada de rede.
- Certifique-se de que verificou as definições de notificação do Azure AD para Ligação estado de trabalho e reveja a sua definição. Para compreender como configurar as definições de notificação para as notificações de Estado Ligação AD do Azure, consulte este [guia.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Para saber mais sobre o relatório de sincronização do Ligação Estado de Trabalho do AAD e sobre como transferi-lo, consulte Relatório de [sincronização ao nível do objeto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Para remoção de alertas de saúde do AAD Ligação siga o guia de remoção de problemas do [AAD Ligação Alertas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) sobre a recente estado de vida dos dados e para perguntas mais frequentes, consulte Perguntas mais frequentes sobre a instalação do [AAD Ligação](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)Estado de Trabalho.
