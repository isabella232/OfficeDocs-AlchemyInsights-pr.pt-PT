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
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941619"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Trabalhar com listas e bibliotecas grandes no SharePoint

As listas e bibliotecas do SharePoint podem conter até 30 milhões de itens, mas quando têm mais de 5000 itens, poderá ver um erro Limiar de Vista de Lista quando tenta trabalhar com as mesmas. Este limiar está em vigor para manter o desempenho do serviço. Não pode ser alterado. Para evitar atingir este limiar:

**Utilizar moderno**

As vistas que mostram muitos itens funcionam melhor na experiência moderna. [Utilize a experiência moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) para evitar erros que possa ver na experiência clássica.

**Adicionar índices**

Quando filtra ou ordena por uma coluna que não tem um índice, poderá ver uma mensagem de erro. [Adicione um índice manualmente](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) a partir **da lista Definições** no menu definições e, em seguida, **Colunas Indexadas.**

**Editar a vista de lista**

Se ocorrer um erro ao trabalhar com uma lista grande, [edite](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)a sua vista de lista .

As quatro alterações seguintes irão remover os erros do limiar de vista de lista. Faça as quatro alterações para remover todos os erros. Se continuar a receber erros, selete [Gerir listas e bibliotecas grandes.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. **Selecione** Nenhum de ambos **os tipos de ordenação: primeiro pela coluna e,** **em seguida, ordenar pela coluna**.
2. **Selecione Nenhum** a partir **de ambos os grupos Primeiro pela coluna e,** em **seguida, agrupe pela coluna**.
3. **Selecione** Nenhum para todas as colunas na **secção Totais.**
4. Desmarce todas as colunas menos uma para apresentação **a partir da secção Colunas.**

