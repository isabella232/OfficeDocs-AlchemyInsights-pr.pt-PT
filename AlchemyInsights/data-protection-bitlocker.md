---
title: Proteção de dados - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908720"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia bitlocker com Intune

 A Política de Proteção de Ponto Final insumo pode ser usada para configurar configurações de criptografia bitlocker para dispositivos Windows. Para obter mais informações, consulte as configurações do [Windows 10 (e posteriores) para proteger os dispositivos que usam o Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)
 
Você deve estar ciente de que muitos dispositivos mais novos que executam o Windows 10 suportam criptografia bitlocker automática, que é ativada sem a aplicação da política mdm. Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas. Veja o SEGUINTE FAQ para mais detalhes.
 
Para obter informações sobre problemas de solução de problemas, consulte [as políticas troubleshoot BitLocker no Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

 P: Quais edições da criptografia do dispositivo de suporte ao Windows usando a Política de Proteção de Ponto Final?<br>
 R: As configurações da Política de Proteção de Ponto Final Intune são implementadas usando o [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nem todas as edições ou compilações de Windows suportam o Bitlocker CSP. <br><br>
      Neste momento, as seguintes edições do Windows são suportadas: Enterprise, Education, Mobile, Mobile Enterprise e Professional (build 1809 and later).
 
P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do SISTEMA OPERACIONAL para método de criptografia e força de cifra (XTS-AES-128), aplicará uma política com configurações diferentes acionando automaticamente a recriptografia da unidade com as novas configurações?<br>
R: Não. Para aplicar as novas configurações de cifra, a unidade deve primeiro ser descriptografada.<br><br>
**Nota:** Para dispositivos que estão sendo registrados com piloto automático, a criptografia automática que ocorreria durante o OOBE não é ativada até que a política de intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional.
 
P: Se um dispositivo for criptografado como resultado da aplicação da política de Intune, ele será descriptografado quando essa política for removida?<br>
R: A remoção da política relacionada à criptografia não resulta na decodificação das unidades configuradas.
 
P: Por que a Política de Conformidade Intune mostra que meu dispositivo não tem o Bitlocker habilitado, mesmo que seja?<br>
R: A configuração "Bitlocker habilitado" na Política de Conformidade Intune utiliza o cliente de Atestado de Saúde do Dispositivo Windows (DHA). Este cliente só mede o estado do dispositivo na hora da inicialização. Portanto, se um dispositivo não foi reiniciado desde que a criptografia bitlocker foi concluída, o serviço de cliente DHA não informará o Bitlocker como ativo.
 
 