---
title: Read-Only para mensagem de manutenção ao tentar utilizar SharePoint ou OneDrive
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
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670843"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only para mensagem de manutenção ao tentar utilizar SharePoint ou OneDrive

Os utilizadores podem receber uma mensagem **Read-Only para Manutenção** quando tentarem utilizar o SharePoint ou o OneDrive para um dos seguintes cenários. 

-   Uma atividade de manutenção planeada ou ativa.  Verifique-os navegando no [Centro de Mensagens.](https://portal.office.com/adminportal/home#/messagecenter)
-   Um incidente de serviço ativo de alta prioridade que pode estar a ocorrer. Verifique se há avisos/incidentes navegando para a [Saúde do Serviço](https://portal.office.com/adminportal/home#/servicehealth).
-   Um pequeno cenário de recuperação automática que pode estar a acontecer devido a eventos inesperados nos servidores que podem durar menos de 30 min ou mais. 
    
    Não existem postos de Mensagem ou Serviços de Saúde para estas pequenas recuperações, mas deverá voltar ao normal muito em breve.

Em poucas ocasiões, observámos que um dos três cenários listados acima foram a causa, e o serviço foi restaurado, mas a cache do navegador dos utilizadores não foi limpa.

Por favor, tente limpar a cache do navegador antes de navegar para o site.

1. No seu navegador Microsoft Edge, selecione **Definições**e, em seguida, selecione **Privacidade e Segurança**.
2. Em **Navegação Clara,** **selecione Escolha o que limpar**.
3. Selecione **Cookies e guarde os dados do site,** e selecione **Clear**.

>[!Note] 
> Estes passos podem diferir quando se utilizam outros navegadores como o Mozilla Firefox ou o Google Chrome.

>[!Note] 
> Outra opção seria abrir o seu site SharePoint ou OneDrive numa nova janela InPrivate.