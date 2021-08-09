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
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934844"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adicionar utilizadores externos a um Grupo de Distribuição

Adicionar um contacto externo a um Grupo de Distribuição (GD) é um processo de dois passos:
  
1. Criar um Contacto de Correio para o utilizador externo:
    
    1. No centro de administração, vá para a página  >  [Contactos do](https://admin.microsoft.com/adminportal/home#/Contact) Utilizador. 
    
    2. **Selecione Adicionar um contacto**.
    
    3. Escreva as informações do seu contacto e **selecione Adicionar**.
    
2. Adicione o Contacto de Correio ao seu GD:
    
    1. No centro de administração, vá para a página  >  [Grupos.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Localmente o GD ao que pretende adicionar o utilizador externo e selecione-o para abrir a caixa de diálogo Editar.
    
    3. No separador **Membros,** selecione **Ver todos e gerir membros**. 
    
    4. **Selecione Adicionar membros**.
    
    5. Selecione o Contacto de Correio que criou no passo anterior e, em seguida, selecione **Guardar**.
    
Se, após seguir estes passos, os seus utilizadores externos não conseguirem enviar e-mails para o GD ou receber e-mails do mesmo, é possível que o GD só permita e-mails de utilizadores internos. Pode verificar esta configuração e corrigi-la seguindo as instruções [aqui.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Nota:** Estas instruções não se aplicam se o tipo do seu grupo for "grupo de Microsoft 365" em vez de "Grupo de Distribuição". Se for esse o caso, pode adicionar o utilizador externo diretamente ao grupo a partir Outlook. Pode encontrar informações detalhadas Microsoft 365 convidados dos Grupos e instruções para adicionar convidados externos [neste artigo.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  