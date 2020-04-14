---
title: Preso no Outbox por causa de grandes anexos
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241263"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corrija mensagens que estão presas na Caixa de Saída

Recomendamos que comece por executar o cenário ["Estou com problemas em enviar, receber ou encontrar mensagens](https://aka.ms/SaRA-OutlookSendReceive) de correio eletrónico" da ferramenta [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)

Quando uma mensagem fica presa na sua Outbox, a causa mais provável é um grande anexo ou a opção "Enviar imediatamente quando estiver ligada" não está ativada.

**Retire o acessório grande**

1. No Outlook, selecione **Enviar / Receber** > **Trabalho Offline**. 
2. No painel de navegação, selecione **Outbox**. A partir daqui, pode: 
    - Apagar a mensagem (selecione-a e, em seguida, **selecione Apagar**).
    - Arraste a mensagem para a pasta Drafts, clique duas vezes para abri-la e remova o anexo selecione-o e, em seguida, **selecione Delete**).
3. Se receber um erro que diga que o Outlook está a tentar transmitir a mensagem, feche o Outlook. Pode levar alguns momentos para sair. Se o Outlook não fechar, prima Ctrl+Alt+Delete e selecione **Start Task Manager**. No Gestor de Tarefas, selecione o separador **Processos,** desloque-se para outlook.exe e selecione **End Process**.
4. Depois do Outlook fechar, reinicie-o e repita os passos 2 e 3. 
5. Depois de remover o anexo, clique em **Enviar / Receber** > **Trabalho Offline** para retomar o trabalho online. 

As mensagens também ficam presas na Caixa de Saída quando clica em **Enviar**, mas não está ligada. Clique em **Enviar / Receber** e ver o botão Work **Offline.** Se é azul, estás desligado. Clique nele para ligar (o botão fica branco) e clique em **Enviar tudo**.
 
**Ativar Enviar imediatamente quando ligado**
 
1. No separador Ficheiro, clique em **Opções**.

2. Na caixa de diálogo Outlook Options, clique **em Advanced**.

3. Na secção Enviar e receber, clique para ativar **Enviar imediatamente quando ligado**. Clique em **OK**.
 
Para mais detalhes, consulte:
- [Vídeo: Enviar ou apagar um e-mail preso](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [O e-mail permanece na pasta Outbox até iniciar manualmente uma operação de envio/receção no Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
