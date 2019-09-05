---
title: Adicionar utilizadores externos a um grupo de distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737884"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar utilizadores externos a um grupo de distribuição

Adicionar um contacto externo para um grupo de distribuição (DG) é um processo composto por dois passos:
  
1. Crie um contacto de correio para o utilizador externo:
    
    1. No Centro de administração, vá para os **utilizadores** > página de[contactos](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Seleccione **Adicionar um contacto**.
    
    3. Escreva as informações para contacto e seleccione **Adicionar**.
    
2. Adicione o contacto de correio para a direcção-geral:
    
    1. No Centro de administração, vá para os **grupos** > página[grupos](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Localizar DG que pretende adicionar o utilizador externo e, seleccione-a para abrir a caixa de diálogo de edição.
    
    3. No separador **Membros** , seleccione **Ver tudo e gerir os membros**. 
    
    4. Seleccione **Adicionar membros**.
    
    5. Seleccione o contacto de correio que criou no passo anterior e, em seguida, seleccione **Guardar**.
    
Se depois de seguir estes passos utilizadores externos não é possível enviar mensagens de correio electrónico para a direcção-geral ou se não recebem mensagens de correio electrónico a partir do mesmo, é possível que a direcção-geral está marcada para permitir apenas mensagens de correio electrónico de utilizadores internos. Pode verificar esta configuração e corrigi-lo seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Nota:** Estas instruções não se aplicam se o tipo de um grupo é "Grupo do Office 365" em vez de "Grupo de distribuição". Se for esse o caso, pode adicionar o utilizador externo directamente para o grupo a partir do Outlook. Obter informações detalhadas sobre os convidados de grupos do Office 365, bem como instruções para adicionar convidados externos podem encontrar-se no [presente artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  