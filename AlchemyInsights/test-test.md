---
title: Termos em falta do arquivo de termos de Online do SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762081"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activar a encriptação de Bitlocker com Intune

Política de protecção de ponto final de Intune pode ser utilizada para configurar definições de encriptação de Boitlocker para os dispositivos Windows conforme descrito em: Windows10 (e posterior) as definições para proteger dispositivos que utilizem Intune

Deverá ter em atenção que muitos dispositivos mais recentes com o Windows 10 suportam a encriptação de bitlocker automático que é accionada sem a aplicação da política do MDM. Se as definições predefinidas não forem configuradas, isto pode afectar a aplicação da política. Consulte as perguntas mais frequentes para obter mais detalhes.


Perguntas mais frequentes  p: quais as edições do Windows suportam a encriptação de dispositivo utilizando a política de protecção de ponto final?
 R: as definições de política de protecção de ponto final de Intune são implementadas utilizando o CSP do Bitlocker.Nem todas as edições nem versões do Windows que suportam o CSP do Bitlocker. 
      Neste momento tempo as edições do Windows: empresa; Educação, portáteis, móveis Enterprise e Professional (de compilação 1809 e posteriores) são suportados.




Q: se um dispositivo já está encriptado com Bitlocker utilizando as predefinições do sistema operativo para o método de encriptação e intensidade da cifra (XTS-AES-128) irá aplicar uma política com diferentes definições de accionam automaticamente reencriptação da unidade com as novas definições?

R: ' não '. Para aplicar as novas definições de cifra que a unidade deve, primeiro, ser desencriptada.

Nota para dispositivos que está a ser inscritos com Autopilot a encriptação automática que ocorreria durante a OOBE, não é activada até que é avaliada a política de Intune, que permite que a política com base em definições para ser utilizado em vez das predefinições de SO




Q se um dispositivo é encriptado na sequência da aplicação da política de Intune será-desencriptado quando é removida dessa política?

R: remoção de encriptação relacionados com a política não resulta na desencriptação das unidades que foram configuradas.




P: por que razão intune política conformidade mostrar que o dispositivo não tem "Bitlocker activado", mas é?

R: o "Bitlocker activado" na política de conformidade intune utiliza o cliente de atestado de saúde de dispositivo do Windows (DHA). Este cliente medidas apenas o estado do dispositivo no momento do arranque. Por isso, se um dispositivo não ter sido reiniciado desde a encriptação de bitlocker foi concluída o serviço de cliente DHA não reportará bitlocker como estando activo.