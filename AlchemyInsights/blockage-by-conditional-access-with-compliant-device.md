---
title: Estou a ser bloqueado pelo Acesso Condicional com um dispositivo compatível
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019159"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Estou a ser bloqueado pelo Acesso Condicional com um dispositivo compatível

**Ferramentas Altamente Recomendadas**

- [Ferramenta de Remoção de Problemas de Registo de](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) Dispositivos – uma ferramenta abrangente que ajuda a remoção dos problemas de registo de dispositivos mais comuns.
- [Testar o script de Conectividade](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) de Registo de Dispositivos – uma ferramenta utilizada para garantir que um dispositivo pode aceder aos pontos finais de Registo de Dispositivos na conta de sistema.
- Script de Limpeza de [Dispositivos do Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – uma ferramenta utilizada para procurar e gerir dispositivos oblíquios no seu ambiente.

Eis algumas razões comuns pelas quais o Acesso Condicional pode estar a  falhar num dispositivo compatível ou o motivo pelo qual os seus utilizadores podem estar a receber Não pode aceder a partir daqui mensagem durante um pedido de acesso a um recurso organizacional.

1. **O dispositivo não se encontra num estado obrigatório do dispositivo com um MDM:**

Valide que o dispositivo está inscrito num fornecedor de MDM aprovado, como o Intune, e que está *assinalado como conforme.* Para obter mais informações sobre o Intune, consulte este [documento](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Para compreender melhor a conformidade do dispositivo e o Intune, consulte Utilizar a política de conformidade para definir regras para dispositivos que [gere com o Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Se estiver a ter problemas ao inscrever um dispositivo com o Intune, encontre os detalhes da remoção de problemas em Remova a inscrição de [dispositivos na Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Para obter suporte adicional do Intune, crie um pedido de suporte. Para fazê-lo, visite a página de Ajuda e Suporte do [Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **O dispositivo não está associado à rede da organização:**

Para aceder a recursos organizacionais, o dispositivo tem de estar ligado à rede da organização, através de ligação direta ou de uma rede privada virtual (VPN), e também associado a uma rede no local ou Azure Active Directory. Para aderir a um dispositivo de trabalho na rede da organização, consulte Aderir ao seu [dispositivo de trabalho na rede da sua organização.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Para registar um dispositivo pessoal/BYOD, consulte Registar [o seu dispositivo pessoal na rede da sua organização.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Para validar se o dispositivo se juntou à rede, pode seguir os passos para dispositivos registados [aqui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) ou para dispositivos de [trabalho aqui.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Para âmbito do problema para a conectividade de rede da Org, siga as diretrizes abaixo:

    1. Inscreva-se no Windows com a sua conta escolar ou alain@contoso.com.
    2. Ligação para a rede da sua organização através de uma VPN ou DirectAccess.
    3. Depois de estar ligado, prima a tecla do **logótipo do Windows+L** para bloquear o dispositivo.
    4. Desbloquear o seu dispositivo com a sua conta escolar ou pessoal e, em seguida, tente aceder novamente à aplicação ou serviço problemático.

Se vir a **mensagem de erro Não é possível voltar a ver** esta mensagem de erro, é provável que o problema seja outro local.

3. **O sistema operativo não é suportado:**

Certifique-se de que está a executar uma versão suportada do sistema operativo, incluindo:

- **Windows Cliente:** Windows 7 ou posterior

- **Windows Server:** Windows Server 2008 R2 ou posterior

- **macOS:** macOS X ou posterior

- **Android e iOS:** versão mais recente dos sistemas operativos Android e iOS

4. **O browser não é suportado:**

Encontre os browsers suportados abaixo. Para o suporte do Chrome Windows 1703 ou versões posteriores, é necessária uma extensão Windows 10 contas. Para o Edge 85+, o utilizador tem de ter a sua conta para transmitir corretamente as informações de conformidade do dispositivo. Para obter mais detalhes, consulte [aqui.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android:** **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Encontre mais informações sobre **Os passos de remoção de problemas** e mensagens não podem ser lidos aqui. [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
