---
title: Adicionar utilizadores externos a um Grupo de Distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910943"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar utilizadores externos a um Grupo de Distribuição

A adição de um contacto externo a um Grupo de Distribuição (DG) é um processo em duas etapas:
  
1. Criar um Contacto de Correio para o utilizador externo:
    
    1. No centro de administração, vá à[página](https://admin.microsoft.com/adminportal/home#/Contact) contactos dos **Utilizadores.** >  
    
    2. Selecione **Adicionar um contacto**.
    
    3. Digite as informações para o seu contacto e selecione **Adicionar**.
    
2. Adicione o Contacto de Correio à sua DG:
    
    1. No centro de administração, vá à página **grupos** > de[grupos.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Encontre a DG a que pretende adicionar o utilizador externo e selecione-o para abrir o diálogo de edição.
    
    3. No separador **Dos Membros,** selecione **Ver todos e gerir os membros**. 
    
    4. Selecione **Adicionar membros**.
    
    5. Selecione o Contacto de Correio criado no passo anterior e, em seguida, selecione **Guardar**.
    
Se depois de seguir estes passos, os seus utilizadores externos não podem enviar e-mails para a DG ou não receber e-mails da sua parte, pode ser que a DG esteja marcada para permitir apenas e-mails de utilizadores internos. Pode verificar esta configuração e fixá-la seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Nota:** Estas instruções não se aplicam se o tipo do seu grupo for "Grupo Microsoft 365" em vez de "Grupo de Distribuição". Se for esse o caso, pode adicionar o utilizador externo diretamente ao grupo a partir do Outlook. Informações detalhadas sobre os hóspedes do Grupo Microsoft 365, bem como instruções para adicionar hóspedes externos podem ser encontradas [neste artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  