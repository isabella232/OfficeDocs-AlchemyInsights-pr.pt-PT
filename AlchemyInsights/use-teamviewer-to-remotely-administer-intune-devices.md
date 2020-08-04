---
title: Utilize o TeamViewer para administrar remotamente dispositivos Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555245"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Utilize o TeamViewer para administrar remotamente dispositivos Intune

Os dispositivos geridos pelo Intune podem ser administrados remotamente utilizando [o TeamViewer](https://www.teamviewer.com/).

Para administrar o Intune utilizando o TeamViewer, utilize estes passos: 

Comece por obter credenciais do TeamViewer para configurar o Conector TeamViewer no Intune. Isto permite que o administrador introduza credenciais no UI do Conector TeamViewer em Dispositivos, uma operação única para estabelecer a ligação entre o Intune e o serviço TeamViewer.

**Parte 1: Iniciar uma sessão com um dispositivo remoto**

1. Em **Todos os dispositivos,** selecione o dispositivo com o quais pretende iniciar uma sessão remota.
2. De **... Mais**, selecione **Nova sessão de assistência remota**.
3. Selecione **Sim** para reconhecer que deseja estabelecer uma sessão remota.
    Depois de o pedido de "Iniciar uma nova sessão remota" ser reconhecido pelo serviço TeamViewer, verá uma opção para Iniciar assistência **remota** sob os detalhes do painel Desíduo (ou, Essencial) para o dispositivo. Selecione **Ver Mais** para expandir o painel e mostrar o estado de Assistência Remota.
4. Selecione **Iniciar sessão remota** para iniciar a sessão no lado da administração.
5. Opte por descarregar o binário TeamViewer (Windows) e selecione **Executar**.<br/>
    **Nota** Pode ignorar qualquer página de navegador aberta no web site do TeamViewer.

6. Reconheça o pedido da aplicação TeamViewer para escamar alterações no dispositivo (apenas windows).
7. A aplicação TeamViewer começa e inclui o código de sessão para autenticar a ligação com o dispositivo remoto.

**Parte 2: No dispositivo que está a ser alvo de uma sessão remota**

1. Abra o portal da empresa Intune.
2. Procure uma bandeira de notificação: "O seu administrador de TI está a solicitar o controlo deste dispositivo para uma sessão de assistência remota", e selecione a notificação.
3. Opte por descarregar a aplicação TeamViewer ou reconheça o download da aplicação TeamViewer a partir da loja de aplicações e selecione **Run**.
    **Nota** Pode ignorar qualquer página de navegador aberta no web site do TeamViewer.

4. Reconheça o pedido da aplicação TeamViewer para escamar alterações no dispositivo (apenas windows).
5. A aplicação TeamViewer começa e inclui o código de sessão para autenticar a ligação com o dispositivo remoto.
6. Um pop-up pergunta se quer permitir que a sessão comece.

**Nota** Os códigos de sessão gerados pelo serviço TeamViewer são utilizados apenas uma vez. Se perder a ligação, deve:

1. Feche a instância da aplicação TeamViewer no dispositivo remoto e na estação de trabalho de administração.
2. Feche o portal da empresa no dispositivo remoto.
3. Inicie uma nova "nova sessão de assistência remota" a partir do portal de administração.
4. Reabrimos o portal da empresa no dispositivo remoto para receber a nova notificação.
5. Descarregue e abra a aplicação TeamViewer tanto no dispositivo remoto como na estação de trabalho de administração, como antes.