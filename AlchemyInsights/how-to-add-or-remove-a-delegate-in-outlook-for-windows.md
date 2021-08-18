---
title: Como adicionar ou remover um Delegado no Outlook para Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329051"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Como adicionar ou remover um Delegado no Outlook para Windows

Para adicionar um Delegado no Outlook para Windows: 

1. Clique no separador **Ficheiro seguido** de Conta **Definições, em** seguida, selecionar Acesso **Delegado.**
2. Clique em **Adicionar**. Se **a** ligação Adicionar não for apresentada, poderá não existir uma ligação ativa entre Outlook e Exchange. A Outlook de estado da ligação apresenta o estado da ligação.
3. Escreva o nome da pessoa que pretende designar como delegado ou procure e escolha o nome na lista de resultados da pesquisa.

    **Nota:** o delegado tem de ser uma pessoa na Lista de Endereços Exchange Global (GAL) da sua organização.
4. Clique em **Adicionar** seguido de **OK.**
5. Na caixa **de diálogo Permissões dos Delegados,** aceite as predefinições das permissões ou selecione níveis de acesso personalizados Exchange pastas.

    - Se um delegado apenas necessitar de permissão para trabalhar com pedidos de reunião e respostas, as predefinições de permissão, como Delegado, recebem cópias das mensagens que me enviarem sobre reuniões são **suficientes.** Pode deixar a definição **de permissão Caixa** de Entrada como **Nenhuma**. Os pedidos de reunião e as respostas irão diretamente para a caixa de entrada do delegado.

    **Nota:** por predefinição, é concedida ao delegado a permissão **Editor (pode ler,** criar e modificar itens) para a **sua pasta** Calendário. Quando o delegado responder a uma reunião em seu nome, esta será adicionada automaticamente à **sua pasta** Calendário.

5. Para enviar uma mensagem para notificar o delegado sobre as permissões alteradas, selecione a caixa de verificação Enviar automaticamente uma mensagem ao **delegado, resumindo** estas permissões.
6. Se quiser, selecione a caixa **de verificação O delegado pode ver os meus itens** privados.

    **Importante:** esta definição afeta todas as Exchange pastas. Isto inclui todas as pastas Correio, Contactos, Calendário, Tarefas, Notas e Diário. Não é forma de conceder acesso a itens privados apenas em pastas especificadas.

7. Selecione **OK**.

    **Nota:**
    - As mensagens enviadas com permissões Enviar em Nome De incluem os nomes do delegado e do utilizador junto a **De**. Quando uma mensagem é enviada com permissões Enviar Como, apenas o seu nome é exibido.
    - Assim que adicionar alguém como delegado, esta poderá adicionar a sua Exchange correio pessoal ao respetivos Outlook perfil. Para obter instruções, consulte [Gerir o correio e itens de calendário de outra pessoa.](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)

Para remover um Delegado no Outlook para Windows:

1. Clique no **separador** Ficheiro.
2. Clique em **Conta Definições** seguida de **Acesso Delegado.**
3. Escolha o nome do delegado para o qual pretende alterar as permissões e, em seguida, clique em **Remover** seguido de **OK.**
