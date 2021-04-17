---
title: Problemas de áudio no Windows 10
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
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833302"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Problemas de resolução de problemas de áudio no Windows 10

**Executar o resolução de problemas de áudio**

1.  Abra as [definições de resolução de problemas](ms-settings:troubleshoot).

2.  Selecione **Reproduzir áudio**  >  **Executar o resolução de problemas**.

**Desafine o dispositivo predefinido**

Se estiver a ligar-se a um dispositivo de áudio utilizando USB ou HDMI, poderá ter de definir esse dispositivo como padrão:

1. Abra **o Start**  >  **Sound** e, em seguida, selecione sons do sistema De **som** ou **de alteração** da lista de resultados.

2.  No **separador Reprodução,** selecione um dispositivo, selecione **'Padrão'** e, em seguida, selecione **OK**.

**Verifique os cabos, volume, altifalantes e auscultadores**

1. Verifique se os cabos de altifalantes e auscultadores estão ligados à tomada correta.

2. Verifique os níveis de potência e volume e tente aumentar todos os controlos de volume.

3. Alguns altifalantes e aplicações têm os seus próprios controlos de volume; talvez tenha que verificar todos para ter certeza de que estão nos níveis certos.

4. Tente ligar utilizando uma porta USB diferente.

**Nota:** Lembre-se de que os altifalantes podem não funcionar quando os auscultadores estiverem ligados.

**Verifique o gestor do dispositivo**

Para se certificar de que os condutores estão atualizados:

1. Selecione **Iniciar**, digite **o Gestor de Dispositivos** e, em seguida, selecione o Gestor de **Dispositivos** na lista de resultados.

2. Em **Controladores de Som, vídeo e jogo**, selecione a sua placa de som, abra-a, selecione o **separador Condutor** e selecione 'Atualizar Driver' ( **'Atualizar' (')**

**Nota:** Se o Windows não encontrar um novo controlador, procure um no site do fabricante do dispositivo e siga as suas instruções.

**Reinstalar o controlador**

Se não conseguir atualizar através do Device Manager ou encontrar um novo controlador no site do fabricante, experimente estes passos:

1. No Gestor de Dispositivos, clique à direita (ou prima e retenha) o controlador de áudio e selecione **Desinstalar**. Reinicie o seu dispositivo e o Windows tentará reinstalar o controlador.

2. Se a reinstalação do controlador não funcionar, tente utilizar o controlador de áudio genérico que vem com o Windows. No Gestor de Dispositivos, clique com o botão direito (ou prima e retenha) o seu controlador de áudio > **atualizar o software do controlador**  >  **Navegue no meu computador para obter software** do condutor  >  **Deixe-me escolher a partir de uma lista de controladores de dispositivos no meu computador**, selecione Dispositivo de Áudio de Alta **Definição,** selecione **Seguinte**, e siga as instruções para o instalar.
