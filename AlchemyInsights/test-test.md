---
title: Termos ausentes da SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053524"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia bitlocker com intune

A política de proteção de ponto final em conjunto pode ser usada para configurar configurações de criptografia Boitlocker para dispositivos Windows, conforme descrito em: configurações do Windows10 (e posteriores) para proteger dispositivos usando O Intune

Você deve estar ciente de que muitos dispositivos mais novos que executam o Windows 10 suportam criptografia automática de bitlocker que é acionada sem a aplicação da política mdm. Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas. Veja o FAQ para mais detalhes.


FAQ  Q: Quais edições da criptografia do dispositivo de suporte ao Windows usando a Política de Proteção de Ponto Final?
 R: As configurações da Política de Proteção de Pontos Finais Intune são implementadas usando o Bitlocker CSP.Nem todas as edições nem compilações de Windows suportam o Bitlocker CSP. 
      Neste momento Windows Editions: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (a partir da construção de 1809) são suportados.




P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do SISTEMA OPERACIONAL para método de criptografia e força de cifra (XTS-AES-128) aplicará uma política com configurações diferentes acionando automaticamente a recriptografia da unidade com as novas configurações?

R: Não. A fim de aplicar as novas configurações de cifra, a unidade deve primeiro ser descriptografada.

Nota Para dispositivos que estão sendo registrados com piloto automático a criptografia automática que ocorreria durante o OOBE não é acionada até que a política de intune seja avaliada, o que permite que as configurações baseadas na política sejam usadas no lugar dos padrões do sistema operacional




Q Se um dispositivo é criptografado como resultado da aplicação da política Intune será descriptografado quando essa política for removida?

R: A remoção da política relacionada à criptografia não resulta na decodificação das unidades que foram configuradas.




P: Por que a política de conformidade intune mostra que meu dispositivo não tem "Bitlocker Habilitado", mas é?

R: A configuração "Bitlocker" configurada em intunte a política de conformidade utiliza o cliente de atestado de saúde do dispositivo Windows (DHA). Este cliente só mede o estado do dispositivo na hora da inicialização. Portanto, se um dispositivo não foi reiniciado desde que a criptografia do bitlocker foi concluída, o serviço de cliente DHA não informará o bitlocker como ativo.