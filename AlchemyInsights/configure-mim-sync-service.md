---
title: Configure o serviço MIM Sync
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481867"
---
# <a name="configure-mim-sync-service"></a>Configure o serviço MIM Sync

O Serviço de Sincronização do Microsoft Identity Manager (MIM) é um componente da MIM. É um serviço centralizado no local que armazena e integra informação para organizações que têm vários diretórios e bases de dados no local. Poderá resolver o seu problema com a MIM Sync se o problema tiver sido abordado numa recente atualização à MIM ou for um dos outros problemas mencionados na secção abaixo.

**Passos recomendados**

1. Certifique-se de que está a utilizar uma atualização recente do MIM Sync e verifique as [notas de lançamento](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) do MIM Sync para determinar se o problema foi resolvido numa atualização.
2. Se o problema estiver com o conector Genérico LDAP, Generic SQL, Lotus Domino ou Web Services, certifique-se de que está a utilizar uma atualização recente dos [conectores genéricos](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Se um mim Sync-run parar com um erro, consulte a tabela de códigos de erro de [execução](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) para determinar as causas potenciais.
4. Se a execução parar com **a exceção extensão- dll,** clique nessas palavras para abrir a janela **das propriedades do Objeto espacial do Conector** e clique no **Stack Trace...** para ver mais informações sobre a causa subjacente, como descrito na [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Se o serviço de notificação de alteração de palavra-passe (PCNS) reportar o **erro 6025** no registo de eventos durante a sincronização da palavra-passe, consulte o guia para verificar o [erro de reporte do PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Se a sincronização total com o Agente de Gestão de Serviços FIM for lenta, verifique a definição **de crescimento automático** para TempDB, conforme descrito na sincronização lenta ou pendurada na [resolução de problemas.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Se encontrar um erro de stop-server com serviços de criação-via-web falhados utilizando o Agente de Gestão de Serviços FIM, consulte [o Support-Info: serviços de criação-via-web falhados](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) para uma visão geral das causas.

