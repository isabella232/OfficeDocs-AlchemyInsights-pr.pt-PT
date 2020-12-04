---
title: Como adicionar ou remover um delegado no Outlook para windows
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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573574"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Como adicionar ou remover um delegado no Outlook para windows

Para adicionar um delegado no Outlook for Windows: 

1. Clique no **separador Ficheiro** seguido de **Definições de Conta** e, em seguida, escolha O Acesso **delegado**.
2. Clique em **Adicionar**. Se **o Add** não aparecer, pode não existir uma ligação ativa entre o Outlook e o Exchange. A barra de estado do Outlook apresenta o estado de ligação.
3. Digite o nome da pessoa que pretende designar como seu delegado, ou procure e escolha o nome na lista de resultados de pesquisa.

    > [!NOTE]
    > O delegado deve ser uma pessoa na Lista de Endereços Globais da sua organização (GAL).
4. Clique em **Adicionar** seguido por **OK**.
5. Na caixa de diálogo **Dedesemesta permissões,** aceite as definições de permissão predefinidos ou selecione níveis de acesso personalizados para pastas De troca.

    - Se um delegado precisar de permissão para trabalhar apenas com pedidos e respostas de reunião, as definições de permissão por defeito, como **delegado, recebem cópias de mensagens relacionadas com a reunião enviadas para mim são suficientes.** Pode deixar a definição de permissão **de caixa de** entrada em **Nenhum**. Os pedidos e respostas da reunião irão diretamente para a caixa de entrada do delegado.

    > [!NOTE]
    > Por predefinição, o delegado recebe permissão **do Editor (pode ler, criar e modificar itens)** para a sua pasta **Calendar.** Quando o delegado responde a uma reunião em seu nome, é automaticamente adicionado à sua pasta **Calendar.**

5. Para enviar uma mensagem para notificar o delegado das permissões alteradas, selecione a **enviar automaticamente uma mensagem para delegar resumindo a caixa de verificação destas permissões.**
6. Se quiser, selecione o Delegado pode ver a minha caixa de verificação **de itens privados.**

    > [!IMPORTANT]
    > Esta definição afeta todas as pastas Exchange. Isto inclui todas as pastas de Correio, Contactos, Calendário, Tarefas, Notas e Diário. Não existe forma de conceder acesso a itens privados apenas em pastas especificadas.

7. Selecione **OK**.

    > [!NOTE]
    >
    > - As mensagens enviadas com permissões enviar em nome incluem tanto as do delegado como os seus nomes ao lado **de From**. Quando uma mensagem é enviada com permissões de Envio como, apenas o seu nome aparece.
    > - Uma vez que adicione alguém como delegado, eles podem adicionar a sua caixa de correio Exchange ao seu perfil Outlook. Para obter instruções, consulte [Gerir o correio e os itens de calendário de outra pessoa](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Para remover um delegado no Outlook for Windows:

1. Clique no **separador Ficheiro.**
2. Clique em **Definições de Conta** seguida **de Acesso delegado.**
3. Escolha o nome do delegado para quem pretende alterar permissões e, em seguida, clique em **Remover** seguido por **OK**.
