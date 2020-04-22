---
title: Termos em falta na SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766864"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitar a encriptação bitlocker com Intune

A Intune Endpoint Protection Policy pode ser usada para configurar as definições de encriptação boitlocker para dispositivos Windows, conforme descrito em : Windows10 (e mais tarde) definições para proteger dispositivos que utilizem Intune

Deve estar ciente de que muitos dispositivos mais recentes que executam o Windows 10 suportam encriptação automática de bitlockers que é desencadeada sem a aplicação da política de MDM. Isto pode ter impacto na aplicação da política se as definições não predefinidas forem configuradas. Consulte as FAQ para obter mais detalhes.


FAQ  Q: Que edições da encriptação do dispositivo de suporte do Windows utilizando a Política de Proteção do Ponto Final?
 R: As definições na Política de Proteção de Pontos Finais intune são implementadas utilizando o Bitlocker CSP.Nem todas as edições nem as construções do Windows suportam o Bitlocker CSP. 
      Neste momento, as Edições Windows: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (a partir da construção 1809) são apoiados.




P: Se um dispositivo já estiver encriptado com o Bitlocker utilizando as definições predefinidas do OS para o método de encriptação e a força da cifra (XTS-AES-128) aplicará uma política com diferentes configurações que desencadeiem automaticamente a reencriptação da unidade com as novas definições?

A: Não. Para aplicar as novas definições de cifra, a unidade deve primeiro ser desencriptada.

Nota Para dispositivos que estão a ser matriculados com Autopilot a encriptação automática que ocorreria durante o OOBE não é acionada até que a política Intune seja avaliada, o que permite que as definições baseadas na política sejam utilizadas no lugar dos predefinições do SO




Q Se um dispositivo for encriptado como resultado da aplicação da política Intune será desencriptado quando essa política for removida?

R: A remoção da política relacionada com a encriptação NÃO resulta na desencriptação das unidades configuradas.




P: Porque é que a política de conformidade intune mostra que o meu dispositivo não tem "Bitlocker Enabled" mas é?

R: A definição "Bitlocker ativada" na política de conformidade inoportuna utiliza o cliente de Attestation de Saúde do Dispositivo Windows (DHA). Este cliente só mede o estado do dispositivo no momento do arranque. Portanto, se um dispositivo não tiver sido reiniciado desde que a encriptação bitlocker foi concluída, o serviço de cliente DHA não reportará o bitlocker como estando ativo.