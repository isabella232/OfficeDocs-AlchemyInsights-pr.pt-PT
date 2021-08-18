---
title: Read-Only para a Mensagem de Manutenção ao tentar utilizar o SharePoint ou o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329459"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only para a Mensagem de Manutenção ao tentar utilizar o SharePoint ou o OneDrive

Os utilizadores poderão receber uma mensagem **Só** de Leitura para Manutenção ao tentarem utilizar o SharePoint ou OneDrive um dos seguintes cenários. 

-   Uma atividade de manutenção planeada ou ativa.  Procure-os ao navegar para o Centro [de Mensagens.](https://portal.office.com/adminportal/home#/messagecenter)
-   Um incidente de serviço ativo de alta prioridade que poderá estar a ocorrer. Procure avisos/incidentes ao navegar para Estado [de Saúde do Serviço.](https://portal.office.com/adminportal/home#/servicehealth)
-   Um cenário de recuperação que poderia ocorrer devido a eventos inesperados nos servidores que podem durar menos de 30 minutos. 
    
    Não existem mensagens no Centro de Mensagens ou Estado de Funcionamento do Serviço para estas recuperações secundárias, mas deverá voltar ao normal brevemente.

Em poucas ocasiões, constatamos que um dos três cenários indicados acima foi a causa e o serviço foi restaurado, mas a cache do browser dos utilizadores não foi limpa.

Tente limpar a cache do browser antes de navegar para o site.

1. No seu browser Microsoft Edge, selecione Definições **e, em** seguida, selecione **Privacidade e Segurança.**
2. Em **Limpar navegação, selecione** **Escolher o que limpar**.
3. **Selecione Cookies e dados do site guardados** e selecione **Limpar**.

**Nota:** estes passos poderão ser diferentes ao utilizar outros browsers como o Mozilla Firefox ou o Google Chrome.

**Nota:** Outra opção seria abrir o seu site do SharePoint OneDrive numa nova janela InPrivate.