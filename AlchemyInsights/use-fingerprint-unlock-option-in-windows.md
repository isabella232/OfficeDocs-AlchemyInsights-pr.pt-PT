---
title: Utilize a opção de desbloqueio de impressões digitais no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588326"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Utilize a opção de desbloqueio de impressões digitais no Windows 10

**Ativar a impressão digital Do Windows Hello**

Para desbloquear o Windows 10 utilizando a sua impressão digital, é necessário configurar o Windows Hello Fingerprint adicionando (deixando o Windows aprender a reconhecer) pelo menos um dedo. 

1. Vá a **Definições > Contas > opções de iniciar sessão** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)). As opções de inscrição disponíveis serão listadas. Por exemplo:

    ![Opções de inscrição.](media/sign-in-options.png)

2. Clique ou toque no **Windows Hello Fingerprint**e, em seguida, clique em **Configurar**. Na janela de configuração do Windows Hello, clique **em Iniciar**. O sensor de impressões digitais activa-se-á e pedir-lhe-á que coloque o dedo no sensor:

   ![Sensor de impressões digitais.](media/fingerprint-sensor.png)

3. Siga as instruções, que lhe pedirão para digitalizar repetidamente o dedo. Quando isto estiver terminado, terá a opção de adicionar outros dedos que poderá querer utilizar para iniciar sessão. Da próxima vez que iniciar sessão no Windows 10, terá a opção de utilizar a sua impressão digital para o fazer.

**Windows Hello Fingerprint não disponível como opção de inscrição**

Se o Windows Hello Fingerprint não for apresentado como uma opção nas **opções de acesso,** significa que o Windows não tem conhecimento de nenhum leitor/scanner de impressões digitais ligado ao seu PC, ou que uma política do sistema impede a sua utilização (se, por exemplo, o seu PC for gerido pelo seu local de trabalho). Para resolver problemas: 

1. Selecione o botão **Iniciar** na barra de tarefas e procure o **Gestor do Dispositivo**.

2. Clique ou toque para abrir o **Gestor de Dispositivos**.

3. No Gestor de Dispositivos, expanda os dispositivos biométricos clicando no seu chevron.

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. O seu scanner de impressões digitais deve ser listado como um dispositivo biométrico, como o scanner WBDI sináptico:

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. Se o seu scanner de impressões digitais não for mostrado e o scanner estiver integrado no seu PC, vá ao site do fabricante do PC. Na secção de suporte técnico para o seu modelo PC, procure um controlador Windows 10 para um scanner que possa instalar.

6. Se o scanner estiver separado do PC (ligado via USB), vá ao site do fabricante do scanner para encontrar e instalar o software de controlador do dispositivo Windows 10 para o modelo de scanner que tem.
