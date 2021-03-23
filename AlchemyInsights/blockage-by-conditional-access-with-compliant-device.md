---
title: Estou a ser bloqueado pelo Acesso Condicional com dispositivo compatível.
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
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037073"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Estou a ser bloqueado pelo Acesso Condicional com dispositivo compatível.

**Ferramentas altamente recomendadas**

- [Ferramenta de resolução de problemas de registo do dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - uma ferramenta abrangente que ajuda a resolver problemas com os problemas de registo do dispositivo mais comuns.
- [Script de conectividade de registo do dispositivo](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) de teste - Uma ferramenta usada para garantir que um dispositivo pode aceder aos pontos finais de Registo do Dispositivo na conta do sistema.
- [Script de limpeza de dispositivos AD Azure](https://github.com/mzmaili/AzureADDeviceCleanup) - Uma ferramenta usada para procurar e gerir dispositivos antigos no seu ambiente.

Estas são algumas razões comuns para que o Acesso Condicional possa estar a falhar por um dispositivo em conformidade ou porque os seus utilizadores podem estar a receber **Não pode chegar lá a partir daqui** durante um pedido de inscrição a um recurso organizacional.

1. **O dispositivo não se encontra num estado de dispositivo obrigatório com um MDM:**

Validar que o dispositivo está matriculado com um fornecedor de MDM aprovado como o Intune e *marcado como conforme*. Para obter mais informações sobre o Intune consulte este [documento.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Para uma melhor compreensão da conformidade do dispositivo e do Intune, consulte a política de [conformidade para definir regras para dispositivos que gere com o Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Se tiver problemas em inscrever um dispositivo com o Intune, encontre detalhes de resolução de problemas na [inscrição do dispositivo Troubleshoot na Microsoft.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Para obter mais apoio intune, crie um pedido de apoio. Para tal, visite a [página De Ajuda e Apoio intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **O dispositivo não se junta à rede de organizações:**

Para acesso a recursos organizacionais, o dispositivo tem de ser conectado à rede da organização, seja através de ligação direta ou de uma rede privada virtual (VPN), e também se adere ao Diretório Ativo no local ou ao Azure Ative. Para se juntar a um dispositivo de trabalho na rede de organização, consulte [Junte o seu dispositivo de trabalho à rede da sua organização.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Para registar um dispositivo pessoal/BYOD, consulte [registar o seu dispositivo pessoal na rede da sua organização.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Para validar se o dispositivo se juntou à rede, pode seguir os passos para dispositivos registados [aqui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) ou dispositivos de trabalho [aqui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Para estender a questão à conectividade da rede Org, siga as diretrizes abaixo:

    1. Inscreva-se no Windows utilizando o seu trabalho ou conta escolar, por exemplo, alain@contoso.com.
    2. Conecte-se à rede da sua organização através de uma VPN ou DirectAccess.
    3. Depois de ligar, prima a tecla do logótipo do **Windows+L** para bloquear o seu dispositivo.
    4. Desbloqueie o seu dispositivo utilizando o seu trabalho ou conta escolar e, em seguida, tente aceder novamente à aplicação ou serviço problemático.

Se vires a **mensagem de** erro de novo, o problema é provável noutro lado.

3. **O sistema operativo não é suportado:**

Certifique-se de que está a executar uma versão suportada do sistema operativo, incluindo:

- **Cliente windows**: Windows 7 ou mais tarde

- **Windows Server**: Windows Server 2008 R2 ou posterior

- **macOS**: macOS X ou mais tarde

- **Android e iOS**: Última versão dos sistemas operativos móveis Android e iOS

4. **O navegador web não é suportado:**

Por favor, encontre navegadores suportados abaixo. Para o suporte do Chrome com versões windows 1703 ou posterior, é necessária uma extensão de Contas Windows 10. Para o Edge 85+, o utilizador precisa de ser contratado para passar corretamente as informações de conformidade do dispositivo. Para mais detalhes, consulte [aqui.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Encontre mais informações sobre o **You't get there** message and troubleshoot steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
