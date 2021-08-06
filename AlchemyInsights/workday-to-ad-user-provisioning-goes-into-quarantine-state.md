---
title: Dia de trabalho para Aprovisionamento de Utilizadores AD entra em estado de quarentena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036503"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Dia de trabalho para Aprovisionamento de Utilizadores AD entra em estado de quarentena

**O Dia de trabalho para o Aprovisionamento de Utilizadores AD entra em estado de quarentena e não são criados utilizadores no AD**

A tarefa de Dia de Trabalho para Aprovisionamento de Utilizadores AD entrou em estado de quarentena e os registos de auditoria mostram eventos de falha de exportação com a mensagem de erro **Erro: OperationsError-SvcErr: ocorreu um erro de operação. Não foi configurada nenhuma referência superior no serviço de diretório. Por conseguinte, o serviço de diretório não consegue emitir referências a objetos fora desta floresta.** Normalmente este erro é mostrado se o Contentor do Active Directory ou se houver problemas com o Mapeamento de Expressões utilizado para **parentDistinguishedName**.

Verifique se o parâmetro Predefinido OU **para** Novos Utilizadores está digitado. Certifique-se de que o OU especificado já existe no seu AD. Se estiver a utilizar **parentDistinguishedName** no mapeamento de atributos, certifique-se de que avalia sempre um contentor conhecido no domínio do AD. Verifique o evento Exportar nos registos de auditoria para ver o valor gerado.

Para obter mais detalhes sobre como configurar o dia de trabalho para o aprovisionamento automatizado, consulte [Tutorial: Configurar](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)Dia de Trabalho para o aprovisionamento automático de utilizadores.

