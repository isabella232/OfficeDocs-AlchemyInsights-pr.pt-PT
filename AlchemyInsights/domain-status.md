---
title: Estado do Domínio – não existem serviços selecionados
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1ddf6475e7cf466a39f76486e0f809097917657bc8f4ae7f7f2b516657308f39
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947454"
---
# <a name="domain-status---no-services-selected"></a>Estado do Domínio – não existem serviços selecionados

Nenhum **serviço selecionado** significa que não selecionou serviços do Microsoft 365 como o Exchange Online, o Skype para Empresas ou o Intune e a Gestão de Dispositivos Móveis para Microsoft 365 para utilizar com o seu domínio personalizado. Se estiver a utilizar a filtragem de spam Exchange Híbrido (Exchange no local com Exchange Online) ou a filtragem de spam externa com Exchange e nenhum outro serviços Microsoft, pode ignorar esta mensagem. O estado de estado de saúde do domínio está disponível apenas para domínios ligados diretamente ao serviço.

Para selecionar serviços para o seu domínio:

1. A **partir Definições**, selecione a caixa junto ao domínio com a mensagem de estado Nenhum serviço  >  [](https://admin.microsoft.com/Adminportal/Home) **selecionado.**
1. **Selecione Gerir DNS** para iniciar o Assistente de Configuração de Domínios.
    - Se selecionar **Adicionar os seus próprios registos DNS,** certifique-se de que seleciona um serviço quando lhe for pedido. Poderiam estar disponíveis mais serviços em **Opções Avançadas.**
    - Se selecionar Permitir que a Microsoft adicione os seus registos **DNS** ou Mais opções Configurar automaticamente os meus serviços online, todos os serviços disponíveis serão sugeridos e  >   selecionados automaticamente.
1. Continue com o assistente para concluir a configuração DNS e as suas opções de serviço.
 
Para obter ajuda adicional para configurar o seu domínio, consulte [Adicionar registos DNS para ligar o seu domínio.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

