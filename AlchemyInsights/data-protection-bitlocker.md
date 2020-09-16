---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731250"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Ativar a encriptação bitlocker com Intune

 A Política de Proteção de Pontos Finais intune pode ser utilizada para configurar definições de encriptação bitlocker para dispositivos Windows. Para obter mais informações, consulte [as definições do Windows 10 (e posterior) para proteger os dispositivos que utilizam o Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)
 
Deve estar ciente de que muitos dispositivos mais recentes que executam a encriptação automática do Bitlocker do Windows 10, que é desencadeada sem a aplicação da política DOM. Isto pode ter impacto na aplicação da política se as definições não padrão forem configuradas. Consulte as seguintes FAQ para obter mais detalhes.
 
Para obter informações sobre problemas de resolução de problemas, consulte [as políticas bitLocker de resolução de problemas no Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

 P: Que edições de encriptação do dispositivo de suporte do Windows utilizando a Política de Proteção de Pontos Finais?<br>
 R: As definições na Política de Proteção do Ponto Final intune são implementadas utilizando o [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nem todas as edições ou construções do Windows suportam o Bitlocker CSP. <br><br>
      Neste momento, as seguintes edições do Windows são suportadas: Enterprise, Education, Mobile, Mobile Enterprise e Professional (build 1809 e posterior).
 
P: Se um dispositivo já estiver encriptado com o Bitlocker utilizando as definições padrão do SISTEMA para o método de encriptação e a resistência cifra (XTS-AES-128), aplicará uma política com diferentes configurações desencadeando automaticamente a reen encriptação da unidade com as novas definições?<br>
R: Não. Para aplicar as novas definições de cifra, a unidade deve primeiro ser desencriptado.<br><br>
**Nota:** Para os dispositivos que estão a ser matriculados com o Autopilot, a encriptação automática que ocorreria durante o OOBE não é ativada até que a política do Intune seja avaliada, o que permite que as definições baseadas em políticas sejam utilizadas em vez dos padrãos de SISTEMA.
 
P: Se um dispositivo for encriptado como resultado da aplicação da política Intune, será desencriptado quando essa política for removida?<br>
R: A remoção da política relacionada com a encriptação NÃO resulta na desencriptação das unidades configuradas.
 
P: Porque é que a Intune Compliance Policy mostra que o meu dispositivo não tem o Bitlocker ativado, mesmo que seja?<br>
R: A definição "Bitlocker ativada" na Política de Conformidade intune utiliza o cliente windows device Health Attestation (DHA). Este cliente só mede o estado do dispositivo na hora do arranque. Assim, se um dispositivo não tiver sido reiniciado desde que a encriptação Bitlocker foi concluída, o serviço de clientes DHA não reportará bitlocker como estando ativo.
 
 