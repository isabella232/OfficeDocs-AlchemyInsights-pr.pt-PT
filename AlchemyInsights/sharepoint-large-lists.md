---
title: Listas grandes do SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720144"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Trabalhar com grandes listas e bibliotecas no SharePoint

As listas e bibliotecas do SharePoint podem conter até 30 milhões de itens, mas quando têm mais de 5.000 itens, poderá ver um erro do Limiar de Visualização de Listas quando tentar trabalhar com eles. Este limiar está em vigor para manter o desempenho do serviço. Não pode ser alterado. Para evitar atingir este limiar:

**Use moderno**

As vistas que mostram muitos itens funcionam melhor na experiência moderna. [Use a experiência moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) para evitar erros que possa ver na experiência clássica.

**Adicionar índices**

Quando filtra ou classifica por uma coluna que não tem um índice, pode ver uma mensagem de erro. [Adicione um índice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente a partir de **Definições** de Lista no menu de definições e, em seguida, **Colunas Indexadas**.

**Editar a vista da lista**

Se ocorrer um erro ao trabalhar com uma lista grande, [edite a sua visualização da lista](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

As quatro alterações seguintes eliminarão os erros do limiar de visualização da lista. Faça as quatro alterações para remover todos os erros. Se ainda estiver a obter erros, verifique [Gerir grandes listas e bibliotecas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Selecione **Nenhum** de ambos **os primeiros classificados pela coluna** **e, em seguida, ordenar pela coluna**.
2. Selecione **Nenhum** de ambos **os primeiros grupos pela coluna** **e, em seguida, agrupe pela coluna**.
3. Selecione **Nenhuma** para todas as colunas na secção **'Totais'.**
4. Desseleccione todas as colunas, menos uma, para visualização da secção **Colunas.**

