---
title: Problemas de áudio no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265027"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Problemas de resolução de problemas de áudio no Windows 10

**Executar o problema de áudio**

1.  Abra as definições de [Troubleshoot](ms-settings:troubleshoot).

2.  Selecione **Reproduzir áudio** > **Executar o resolução de problemas**.

**Definir o dispositivo predefinido**

Se estiver a ligar-se a um dispositivo de áudio utilizando USB ou HDMI, poderá ter de definir esse dispositivo como predefinido:

1.  > Abra **** o**Start Sound**e, em seguida, selecione **sons** do sistema **Sound** or Change da lista de resultados.

2.  No **separador Reprodução,** selecione um dispositivo, selecione **'Definir Padrão**' e, em seguida, selecione **OK**.

**Verifique os cabos, volume, altifalantes e auscultadores**

1. Verifique se os altifalantes e os auscultadores estão ligados à tomada correta.

2. Verifique os níveis de potência e volume e tente aumentar todos os controlos de volume.

3. Alguns oradores e aplicações têm os seus próprios controlos de volume; Talvez tenha que verificar todos para se certificar de que estão nos níveis certos.

4. Tente ligar-se utilizando uma porta USB diferente.

**Nota:** Lembre-se de que os altifalantes podem não funcionar quando os auscultadores estiverem ligados.

**Verificar Gestor de Dispositivos**

Para garantir que os condutores estão atualizados:

1. Selecione **Iniciar,** digitar **Gestor de Dispositivos**e, em seguida, selecione Gestor de **Dispositivos** na lista de resultados.

2. Em **comandos de som, vídeo e jogo,** selecione a sua placa de som, abra-a, selecione o separador **Driver** e selecione 'Controlador de **atualização**' .

**Nota:** Se o Windows não encontrar um novo controlador, procure um no site do fabricante do dispositivo e siga as suas instruções.

**Reinstalar o controlador**

Se não conseguir atualizar via Device Manager ou encontrar um novo controlador no site do fabricante, experimente estes passos:

1. No Gestor do Dispositivo, clique à direita (ou prima e segure) o controlador de áudio e selecione **Desinstalar**. Reiniciar o seu dispositivo e o Windows tentará reinstalar o controlador.

2. Se a reinstalação do controlador não funcionar, tente utilizar o controlador de áudio genérico que vem com o Windows. No Gestor do Dispositivo, clique à direita (ou pressione e segure) o seu controlador de áudio > **Atualizar o software** > do controlador**Navegue no meu computador para** > o software do controlador**Deixe-me escolher de uma lista de controladores de dispositivos no meu computador,** selecione Dispositivo de Áudio de **Alta Definição,** selecione **Next**, e siga as instruções para instalá-lo.
