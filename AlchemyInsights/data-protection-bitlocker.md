---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118605"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Ativar a encriptação do BitLocker com o Intune

A Política de Proteção contra Pontos Finais do Intune pode ser utilizada para configurar as definições de encriptação do Bitlocker Windows dispositivos. Para obter mais informações, consulte [definições Windows 10 (e posterior) para proteger os dispositivos com o Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Além da Política de Proteção do Ponto Final, também existe um Relatório de Encriptação que fornece uma vista mais detalhada do estado de encriptação dos dispositivos. Este relatório pode ser acededo a partir do portal MEM em **Dispositivos > Monitor** e, em seguida, em **Configuração,** selecione Relatório de [encriptação](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Se achar que o Bitlocker não está ativado conforme esperado ou que o perfil que está a ser utilizado para ativar o Bitlocker se encontra num estado de erro, reveja o relatório de encriptação para compreender melhor por que motivo o comportamento está a ocorrer.

Para encontrar detalhes sobre como interpretar o relatório, incluindo os vários valores de estado de encriptação, consulte Monitorizar a encriptação de [dispositivos com o Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Deve ter em atenção que muitos dispositivos mais novos a executar o Windows 10 suportam a encriptação automática do Bitlocker, que é ativada sem a aplicação de política MDM. Isto pode afetar a aplicação da política se estiverem configuradas predefinições que não sejam predefinições. Consulte as seguintes FAQ para mais detalhes.

Para obter informações sobre a remoção de problemas com o bitlocker, consulte Remoção de políticas do [BitLocker Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

P: Que edições de encriptação Windows dispositivo suportam a Política de Proteção contra Pontos Finais?<br>
A: As definições na Política de Proteção contra Pontos Finais do Intune são implementadas através do [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nem todas as edições ou com builds do Windows suportam o Bitlocker CSP. <br><br>

P: Como é que o Bitlocker pode ser ativado em dispositivos sem ter de interagir com o utilizador final?<br>
A: Desde que os pré-requisitos necessários sejam cumpridos, é possível ativar a Encriptação Silenciosa do Bitlocker através do Intune. Consulte os detalhes dos requisitos do dispositivo e exemplos de definições de política para ativar a encriptação silenciosa no seguinte doc: Ativar a Encriptação [bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)de forma silenciosa . <br><br>

P: Se um dispositivo já estiver encriptado com o Bitlocker, utilizando as predefinições do SO para o método de encriptação e a força de cifrões (XTS-AES-128), irá aplicar uma política com definições diferentes aciona automaticamente a nova encriptação da unidade com as novas definições?<br>
R: Não. Para aplicar as novas definições de cifrões, a unidade tem de ser decifrada primeiro.<br><br>
**Nota:** Para os dispositivos inscritos com o Autopilot, a encriptação automática que ocorria durante o OOBE não é ativada até que a política do Intune seja avaliada, o que permite que as definições baseadas em políticas sejam utilizadas em vez das predefinições do SO.
 
P: Se um dispositivo estiver encriptado como resultado da aplicação da política do Intune, será decifrado quando essa política for removida?<br>
A: A remoção da política relacionada com encriptação NÃO resulta na decifração das unidade que foram configuradas.
 
P: Por que motivo a Política de Conformidade do Intune mostra que o meu dispositivo não tem o Bitlocker ativado, apesar de estar?<br>
A: A definição "Bitlocker ativado" na Política de Conformidade do Intune utiliza o cliente Windows Atestado de Estado de Funcionamento do Dispositivo (DHA). Este cliente só mede o estado do dispositivo no momento de arranque. Por isso, se um dispositivo não tiver sido reiniciado desde que a encriptação do Bitlocker foi concluída, o serviço de cliente DHA não reportará o Bitlocker como estando ativo.
 
 