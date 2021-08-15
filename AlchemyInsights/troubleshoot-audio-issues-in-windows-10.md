---
title: Resolução de problemas de áudio no Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039437"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Resolução de problemas de áudio no Windows 10

**Executar a resolução de problemas de áudio**

1.  Abra [as definições de Remoção de Problemas.](ms-settings:troubleshoot)

2.  **Selecione**  >  **Reprodução de Áudio Execute a resolução de problemas**.

**Definir o dispositivo predefinido**

Se estiver a estabelecer ligação a um dispositivo de áudio através de USB ou HDMI, poderá ter de definir esse dispositivo como predefinido:

1. Abra **Iniciar Som**  >  **e,** em seguida, selecione **Som** ou **Alterar sons do** sistema na lista de resultados.

2.  No separador **Reproduzir, selecione** um dispositivo, selecione **Predefinição** e, em seguida, selecione **OK.**

**Verificar cabos, volume, altifalantes e auscultadores com microfone**

1. Verifique se há cabos soltos nas ligações do altifalante e dos auscultadores e certifique-se de que estão ligadas à tomada correta.

2. Verifique os níveis de volume e energia e experimente aumentar todos os controlos de volume.

3. Alguns altifalantes e aplicações têm controlos de volume próprios; poderá ter de verificá-los todos para se certificar de que estão nos níveis certos.

4. Experimente ligar utilizando uma porta USB diferente.

**Nota:** Lembre-se de que os altifalantes podem não funcionar quando os auscultadores estiverem ligados.

**Verificar o Gestor de Dispositivos**

Para se certificar de que os controldores estão sempre actualizados:

1. **Selecione Iniciar**, escreva **Gestor de Dispositivos** e, em seguida, **selecione** Gestor de Dispositivos na lista de resultados.

2. Em **Controladores de som, vídeo** e jogos , selecione  a placa de som, abra-a, selecione o separador Controlador e selecione **Atualizar Controlador**.

**Nota:** Windows não encontrar um novo controlador, procure um no site do fabricante do dispositivo e siga as instruções.

**Reinstalar o controlador**

Se não conseguir atualizar através do Gestor de Dispositivos ou encontrar um novo controlador no site do fabricante, experimente estes passos:

1. No Gestor de Dispositivos, clique com o botão direito do rato (ou prima sem premir) no controlador de áudio e **selecione Desinstalar**. Reinicie o seu dispositivo Windows tentará reinstalar o controlador.

2. Se a reinstalação do controlador não funcionar, experimente utilizar o controlador de áudio genérico do Windows. No Gestor de Dispositivos, clique com o botão direito do rato (ou prima sem premir) no controlador de áudio > Atualizar **software** do controlador Procure software do controlador no meu computador Permita-me escolher a partir de uma lista de controldores de dispositivos no meu computador , selecione Dispositivo de Áudio de Alta Definição , selecione Seguinte e siga as instruções para  >    >  **instalá-lo.**  
