---
title: Adicionar utilizadores externos a um Grupo de Distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663524"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar utilizadores externos a um Grupo de Distribuição

A adição de um contacto externo a um Grupo de Distribuição (DG) é um processo em duas fases:
  
1. Criar um Contacto de Correio para o utilizador externo:
    
    1. No centro de administração, aceda à página **Contactos dos Utilizadores.**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. **Selecione Adicione um contacto**.
    
    3. Digite as informações para o seu contacto e selecione **Adicionar**.
    
2. Adicione o Contacto de Correio à sua DG:
    
    1. No centro de administração, **Groups**aceda à página  >  [grupos de grupos.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Encontre a DG a que pretende adicionar o utilizador externo e selecione-o para abrir o diálogo de edição.
    
    3. No separador **Membros,** **selecione Ver todos e gerir os membros**. 
    
    4. Selecione **Adicionar os membros**.
    
    5. Selecione o Contacto de Correio que criou no passo anterior e, em seguida, **selecione Guardar**.
    
Se depois de seguir estes passos os seus utilizadores externos não puderem enviar e-mails à DG ou não receberem e-mails do mesmo, pode ser que a DG esteja marcada apenas para permitir e-mails de utilizadores internos. Pode verificar esta configuração e corrigi-la seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Nota:** Estas instruções não se aplicam se o tipo do seu grupo for "Microsoft 365 group" em vez de "Grupo de Distribuição". Se for esse o caso, pode adicionar o utilizador externo diretamente ao grupo do Outlook. Informações detalhadas sobre os hóspedes do Grupo Microsoft 365, bem como instruções para a adição de hóspedes externos podem ser encontradas [neste artigo.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  