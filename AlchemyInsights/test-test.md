---
title: Termos em falta na Loja de Termos do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106437"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Ativar a Encriptação de Bitlocker com o Intune

A Política de Proteção contra Pontos Finais do Intune pode ser utilizada para configurar definições de encriptação Boitlocker para dispositivos Windows conforme descrito em : Definições do Windows10 (e posterior) para proteger dispositivos com o Intune

Deve ter em atenção que muitos dispositivos mais novos a executar o Windows 10 suportam a encriptação de bits automática que é ativada sem a aplicação da política MDM. Isto pode afetar a aplicação da política se estiverem configuradas definições que não sejam predefinições. Consulte as FAQ para mais detalhes.


Perguntas mais frequentes: Que edições de Windows suportam a encriptação de dispositivos com a Política de Proteção do Ponto Final?
A: As definições na Política de Proteção de Pontos Finais do Intune são implementadas através do Bitlocker CSP.  Nem todas as edições ou com builds do Windows suportam o Bitlocker CSP. Neste momento, Windows: Enterprise; São suportadas as versões Educação, Dispositivos Móveis, Mobile Enterprise e Professional (a partir da complicação 1809).




P: Se um dispositivo já estiver encriptado com o Bitlocker, utilizando as predefinições do SO para o método de encriptação e a força da cifra (XTS-AES-128) aplicará uma política com definições diferentes aciona automaticamente a encriptação automática da unidade com as novas definições?

R: Não. Para aplicar as novas definições de cifrões, a unidade tem de ser decifrada primeiro.

Nota: para dispositivos inscritos com o Autopilot, a encriptação automática que ocorria durante o OOBE não é ativada até que a política do Intune seja avaliada, o que permite que as definições baseadas em políticas sejam utilizadas em vez das predefinições do SO




P Se um dispositivo estiver encriptado como resultado da aplicação da política do Intune, este será decifrado quando essa política for removida?

A: A remoção da política relacionada com encriptação NÃO resulta na decifração das unidade que foram configuradas.




P: Por que motivo a política de Conformidade do Intune mostra que o meu dispositivo não tem "Bitlocker Ativado" mas está?

A: A definição "Bitlocker ativado" na política de conformidade intune utiliza o cliente Windows Atestado de Estado de Funcionamento do Dispositivo (DHA). Este cliente só mede o estado do dispositivo no momento de arranque. Por isso, se um dispositivo não tiver sido reiniciado desde que a encriptação do bitlocker foi concluída, o serviço de cliente DHA não irá comunicar que o bitlocker está ativo.