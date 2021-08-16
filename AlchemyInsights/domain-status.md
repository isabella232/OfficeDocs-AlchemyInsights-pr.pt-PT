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
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874406"
---
# <a name="domain-status---no-services-selected"></a>Estado do Domínio – não existem serviços selecionados

Nenhum **serviço selecionado** significa que não selecionou serviços de Microsoft 365 como o Exchange Online, o Skype para Empresas ou o Intune e a Gestão de Dispositivos Móveis para Microsoft 365 para utilizar com o seu domínio personalizado. Se estiver a utilizar a filtragem de spam Exchange Híbrido (Exchange no local com Exchange Online) ou a filtragem de spam externa com Exchange e mais nenhuma serviços Microsoft, pode ignorar esta mensagem. O estado de estado de saúde do domínio está disponível apenas para domínios ligados diretamente ao serviço.

Para selecionar serviços para o seu domínio:

1. A **partir Definições**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home), selecione a caixa junto ao domínio com a mensagem de estado Nenhum serviço **selecionado**.
1. **Selecione Gerir DNS** para iniciar o Assistente de Configuração de Domínios.
    - Se selecionar **Adicionar os seus próprios registos DNS,** certifique-se de que seleciona um serviço quando lhe for pedido. Poderiam estar disponíveis mais serviços em **Opções Avançadas.**
    - Se selecionar Permitir que a Microsoft adicione os seus registos **DNS** ou Mais opções Configurar automaticamente os meus serviços online, todos os serviços disponíveis serão sugeridos e  >   selecionados automaticamente.
1. Continue com o assistente para concluir a configuração DNS e as suas opções de serviço.
 
Para obter ajuda adicional para configurar o seu domínio, consulte [Adicionar registos DNS para ligar o seu domínio.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

