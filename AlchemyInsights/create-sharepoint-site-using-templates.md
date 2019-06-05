---
title: Criar um site SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 2097933dd20f326a7bda2151596d514c37d566ff
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717777"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites do SharePoint utilizando modelos

Modelos de site do SharePoint são definições previamente concebidas destinadas em torno de uma determinada necessidade da empresa. Para mais informações, consulte <a href="https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4">utilizar modelos para criar diferentes tipos de sites do SharePoint.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Eis algumas questões/soluções comuns relativas ao guardar um Site ou lista como um modelo no Sharepoint Online.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Botão de modelo de site/lista de guardar não está disponível ou em falta.</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Os administradores serão necessário permitir Script personalizado para activar as funcionalidades do modelo. Para obter passos detalhados, exemplos e considerações Consulte </span> </span> <a style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Permitir ou impedir que o script personalizado</a>.</li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O site de guardar como comando de modelo não é suportado e pode causar problemas em sites que utilizem a infra-estrutura de publicação do SharePoint Server.</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O modelo de site não é possível criar ou não funciona correctamente</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O modelo de uma <a href="https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx">funcionalidade</a> poderão estar em falta e ganha&rsquo;t activar. Se a funcionalidade não está disponível para activar a colecção de sites actual, é possível utilizar o modelo de site para criar um site.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Verifique se todas as listas ou bibliotecas de excederem os <a href="https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59">Limiar de limite de vista de lista de</a> 5000 itens, como este pode bloquear a criação de um modelo de site.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O site poderá estar a utilizar demasiados recursos e, por conseguinte, o modelo de site excede o limite de 50 MB.</span></li> <li>
Existem problemas em visualizar dados de uma lista que utiliza uma coluna de pesquisa. Para mais informações, consulte </span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> <a style="box-sizing: border-box; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a"> <span style="color: #0067b8; text-decoration: none; text-underline: none;">gerado pelo modelo de lista&rsquo;t apresentar dados na lista de pesquisa correcta no SharePoint Online.

Para mais informações sobre problemas e soluções comuns, consulte <a href="https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989">criar e utilizar modelos de site.



