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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109215"
---
# <a name="save-site-or-list-as-a-template"></a>Guardar site ou lista como um modelo

Os modelos de site do SharePoint são definições pré-concebidas concebidas para uma necessidade empresarial específica. Para obter mais informações, [consulte Utilizar modelos para criar diferentes tipos de sites do SharePoint.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Eis alguns problemas comuns/soluções sobre Guardar um Site ou Uma Lista como um modelo no SharePoint Online.

**O botão Guardar modelo de site/lista não está disponível ou em falta.** 

- Os administradores terão de Permitir o Script Personalizado para ativar as funcionalidades de modelo. Para obter passos detalhados, exemplos e considerações, consulte [Permitir ou impedir scripts personalizados.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- O comando Guardar site como modelo não é suportado e pode causar problemas em sites que utilizem a Infraestrutura de Publicação do SharePoint Server.


**O modelo de site não pode ser criado ou não funciona corretamente**

- O modelo poderá estar em falta uma [funcionalidade e](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) não será ativado. Se a funcionalidade não estiver disponível para ser ativada na coleção de sites atual, não pode utilizar o modelo de site para criar um site.


- Verifique se as listas ou bibliotecas excedem o [Limiar do Limite da Vista de Lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, pois pode bloquear a criação de um modelo de site.


- O site pode estar a utilizar demasiados recursos e, por isso, o modelo de site excede o limite de 50 megabyte (MB).


- Existem problemas ao apresentar dados da lista que utiliza uma coluna de pesquisa. Para obter mais informações, consulte A lista gerada pelo modelo não apresenta dados da lista de [procura correta no SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Para obter informações mais detalhadas sobre problemas comuns e soluções, consulte Criar [e utilizar modelos de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

