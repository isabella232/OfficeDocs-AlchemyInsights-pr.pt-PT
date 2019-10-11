---
title: Preso na caixa de saída por causa de grandes anexos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441316"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corrigir mensagens que estão presas na caixa de saída

Recomendamos que você comece executando o cenário "Estou [tendo problemas para enviar, receber ou localizar mensagens de email"](https://aka.ms/SaRA-OutlookSendReceive) da ferramenta assistente de [recuperação e suporte da Microsoft](https://diagnostics.office.com/#/) .

Quando uma mensagem fica presa na sua caixa de saída, as causas mais prováveis são:
- Grandes anexos.
- A opção **enviar imediatamente quando conectada** não está habilitada.

Para remover anexos grandes: 

1. No Outlook, selecione **Enviar/receber** > **trabalho offline**. 
2. No painel de navegação, selecione **caixa de saída**. A partir daqui, você pode: 
    - Exclua a mensagem (selecione-a e, em seguida, selecione **excluir**).
    - Arraste a mensagem para a pasta Rascunhos, clique duas vezes para abri-la e remover o anexo selecioná-lo e, em seguida, selecione **excluir**).
3. Se você receber um erro que diz que o Outlook está tentando transmitir a mensagem, feche o Outlook. Pode demorar alguns instantes para sair. Se o Outlook não fechar, pressione Ctrl + Alt + Delete e selecione **iniciar Gerenciador de tarefas**. No Gerenciador de tarefas, selecione a guia **processos** , role para baixo até Outlook. exe e selecione **finalizar processo**.
4. Depois que o Outlook fecha, reinicie-o e repita as etapas 2 e 3. 
5. Depois de remover o anexo, clique em **Enviar/receber** > **trabalho offline** para retomar o trabalho online. 

As mensagens também ficam presas na caixa de saída quando você clica em **Enviar**, mas você não está conectado. Clique em **Enviar/receber** e veja o botão **trabalhar offline** . Se for azul, você está desconectado. Selecione-o para se conectar (o botão fica branco) e clique em **enviar tudo**.
 
Para habilitar o **envio imediatamente quando conectado**:
 
- Selecione **** > **** opções >  de arquivo**avançadas**.
Na seção **Enviar e receber** , selecione **enviar imediatamente quando conectado**e, em seguida, escolha **OK**.
 
Para obter detalhes completos, consulte:
- [Vídeo: enviar ou excluir um e-mail preso](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [O email permanece na pasta caixa de saída até que você inicie manualmente uma operação de envio/recebimento no Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
