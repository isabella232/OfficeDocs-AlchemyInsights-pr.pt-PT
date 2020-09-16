---
title: Guardar site ou lista como um modelo
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727542"
---
# <a name="save-site-or-list-as-a-template"></a>Guardar site ou lista como um modelo

Os modelos do site SharePoint são definições pré-construídas desenhadas em torno de uma necessidade de negócio particular. Para obter mais informações, consulte [utilizar modelos para criar diferentes tipos de sites SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Aqui estão algumas questões/soluções comuns sobre a poupança de um site ou lista como um modelo no SharePoint Online.

**O botão de modelo de site/lista não está disponível ou em falta**. 

- Os administradores terão de permitir o Script Personalizado para ativar as funcionalidades do modelo. Para etapas detalhadas, exemplos e considerações consulte [Permitir ou impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- O site Save como comando de modelo não é suportado e pode causar problemas em sites que usam a Infraestrutura de Publicação do Servidor SharePoint.


**O modelo do site não pode ser criado ou não funciona corretamente**

- O modelo pode estar a perder uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado. Se a funcionalidade não estiver disponível para ser ativada na recolha atual do site, não poderá utilizar o modelo do site para criar um site.


- Verifique se alguma lista ou biblioteca excede o limiar limite de [visualização](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de lista de 5000 itens, uma vez que isso pode bloquear a criação de um modelo de site.


- O site pode estar a usar demasiados recursos e, portanto, o modelo do site excede o limite de 50 megabyte (MB).


- Existem problemas em apresentar dados de uma lista que utiliza uma coluna de procuração. Para obter mais informações, consulte [a lista gerada por Modelos não exibe dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Para obter informações mais detalhadas sobre problemas e soluções comuns, consulte, [crie e use modelos de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

