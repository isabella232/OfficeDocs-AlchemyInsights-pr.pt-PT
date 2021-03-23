---
title: Estou a ser bloqueado pelo Acesso Condicional com dispositivo de adesão ao domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038099"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Estou a ser bloqueado pelo Acesso Condicional com dispositivo de adesão ao domínio

**Ferramentas altamente recomendadas**

[Ferramenta de resolução de problemas de registo do dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A ferramenta que ajuda a resolver problemas de resolução dos problemas de registo do dispositivo mais comuns.

[Script de conectividade de registo do dispositivo](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) de teste - O script que ajuda a garantir que um dispositivo pode aceder aos pontos finais de Registo do Dispositivo na conta do sistema.

[Script de limpeza de dispositivos AD Azure](https://github.com/mzmaili/AzureADDeviceCleanup) - O script que lhe permite procurar e gerir dispositivos antigos no seu ambiente.

Eis algumas razões comuns para que o acesso condicional possa estar a falhar num dispositivo que se juntou a um domínio (Hybrid Azure AD).

1. **Não existe nenhum Azure AD PRT no dispositivo** - É necessário garantir que o dispositivo tem Token de AZure AD Primary Refresh (PRT). Para mais informações sobre o PRT, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Para verificar se tem Azure AD PRT, pode executar `dsregcmd/status` o comando no dispositivo e verificar se "AzureAdPrt" é igual a "SIM".

Se "AzureAdPrt" for "NO", verifique o seguinte:

- **Se tem um ambiente federado com FS AD, e é inacessível a partir das redes domésticas dos seus utilizadores**: Neste caso, certifique-se de que os seus pontos finais "usernamemixed" estão acessíveis a partir da extranet. Se o seu FS AD estiver por detrás de uma VPN, certifique-se de que os utilizadores se ligam à VPN e re-iniciam sessão no dispositivo. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Se o TPM do dispositivo está defeituoso e, portanto, não pode autenticar o dispositivo**: Verifique "tpm.msc" para ver se o estado do TPM está "Pronto". Caso contrário, corra `dsregcmd/leave` e deixe o dispositivo voltar a juntar-se ao Azure AD. Então, tente de novo. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Está a usar um fornecedor de identidade de terceiros, que não suporta WS-Trust protocolo.** Como descrito nos nossos documentos, os dispositivos híbridos Azure AD-joins não podem funcionar neste caso. Por favor, trabalhe com o seu fornecedor de identidade para apoio.

2. **Os utilizadores estão a utilizar o navegador Chrome sem as contas do Windows 10** ou **extensão do Office O Chrome não utiliza automaticamente o PRT em dispositivos ligados a AAD ou híbridos- AAD-AAD-** Isto leva a falhas de quaisquer políticas de acesso condicional baseadas no dispositivo, com mensagem de erro "dispositivo não registado" exibida. Para utilizar o navegador Chrome corretamente, tem de instalar as "Contas Windows 10" ou "Extensão do Office para o navegador Chrome dos utilizadores" via SCCM ou Intune. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Se não for possível empurrar a extensão remotamente, notifique os utilizadores para instalarem manualmente uma das extensões acima para acederem a aplicações por trás do Acesso Condicional baseado no dispositivo. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. **O dispositivo foi corretamente híbrido Azure AD aderido, mas foi inadvertidamente eliminado ou desativado, quer devido a alterações sincronizadas no Azure AD Connect quer a partir do portal Azure**: Se isso acontecer, o objeto do dispositivo já não é reconhecido como um dispositivo totalmente ligado, mesmo que o estado "AzureAdJoined" e "PRT" apareçam como válidos no dispositivo.

Para corrigir este problema, corra `dsregcmd/leave` nos dispositivos afetados e deixe-os voltar a Azure AD. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Se os seus dispositivos estiverem na atualização do Windows 10, 1809, com VPN/Cloud Proxy e vir problemas com o estado "AzureAdPrt" ou qualquer aplicação com problema SSO (outlook que não se liga à caixa de correio, mesmo que tenha PRT), certifique-se de que tem este patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ou atualização cumulativa de abril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) para evitar falhas de PRT nessas máquinas.

















