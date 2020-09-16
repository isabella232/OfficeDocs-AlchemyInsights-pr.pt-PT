---
title: Faltam termos na SharePoint Online Term Store
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
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750462"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitar a encriptação bitlocker com Intune

A Política de Proteção de Pontos Finais intune pode ser usada para configurar as definições de encriptação do Boitlocker para dispositivos Windows, conforme descrito em : Definições do Windows10 (e posteriormente) para proteger dispositivos que utilizam o Intune

Deve estar ciente de que muitos dispositivos mais recentes que executam a encriptação automática do Bitlocker do Windows 10, que é acionada sem a aplicação da política DOM. Isto pode ter impacto na aplicação da política se as definições não padrão forem configuradas. Consulte as FAQ para obter mais detalhes.


FAQ   Q: Que edições de encriptação de dispositivo de suporte do Windows utilizando a Política de Proteção de Pontos Finais?
 R: As definições na Política de Proteção do Ponto Final intune são implementadas utilizando o CSP Bitlocker.Nem todas as edições nem as construções do Windows suportam o Bitlocker CSP. 
      Neste momento Windows Editions: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (a partir da construção 1809) são apoiados.




P: Se um dispositivo já estiver encriptado com o Bitlocker utilizando as definições padrão do SISTEMA para o método de encriptação e a resistência cifra (XTS-AES-128) aplicará uma política com diferentes configurações, desencadeie automaticamente a reencriminação da unidade com as novas definições?

R: Não. Para aplicar as novas definições de cifra, a unidade deve ser desencriptado primeiro.

Nota Para os dispositivos que estão a ser matriculados com o Autopilot, a encriptação automática que ocorreria durante o OOBE não é ativada até que a política do Intune seja avaliada, o que permite que as definições baseadas na política sejam utilizadas em vez dos padrãos de SISTEMA




Q Se um dispositivo for encriptado como resultado da aplicação da política Intune será desencriptado quando essa política for removida?

R: A remoção da política relacionada com a encriptação NÃO resulta na desencriptação das unidades configuradas.




P: Porque é que a política de conformidade intune mostra que o meu dispositivo não tem "Bitlocker Enabled" mas é?

R: A definição "Bitlocker ativada" na política de conformidade intune utiliza o cliente windows Device Health Attestation (DHA). Este cliente só mede o estado do dispositivo na hora do arranque. Assim, se um dispositivo não tiver sido reiniciado desde que a encriptação bitlocker foi concluída, o serviço de clientes DHA não reportará bitlocker como estando ativo.