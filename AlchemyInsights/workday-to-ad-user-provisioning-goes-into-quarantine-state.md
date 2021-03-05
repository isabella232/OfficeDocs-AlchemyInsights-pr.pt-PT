---
title: Dia de trabalho para fornecimento de utilizadores ad vai para o estado de quarentena
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481882"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Dia de trabalho para fornecimento de utilizadores ad vai para o estado de quarentena

**Dia de trabalho para fornecimento de utilizadores ad entra em estado de quarentena e nenhum utilizador é criado em AD**

O trabalho de Fornecimento de utilizadores de trabalho para a AD entrou em estado de quarentena e os registos de auditoria mostram eventos de falha de exportação com a mensagem de erro **Erro: OperationsError-SvcErr: Ocorreu um erro de operação. Não foi configurada qualquer referência superior para o serviço de diretório. O serviço de diretório é, portanto, incapaz de emitir referências a objetos fora desta floresta.** Este erro geralmente aparece se o Contentor do Diretório Ativo OU não estiver corretamente definido ou se houver problemas com o Mapeamento de Expressão utilizado para **o nome de pais.**

Verifique o parâmetro padrão da **UA** para obter tipografias. Certifique-se de que a OU especificada já existe no seu AD. Se estiver a utilizar **o nome parentalDistinguishedname** no mapeamento do atributo, certifique-se de que avalia sempre um recipiente conhecido dentro do domínio AD. Consulte o evento Exportação nos registos de auditoria para ver o valor gerado.

Para obter mais informações sobre a configuração do dia de trabalho para o provisionamento automatizado, consulte [Tutorial: Configure Workday para o provisionamento automático do utilizador](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

