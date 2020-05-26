---
title: 'Scanner AIP: instalação e configuração'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358104"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scanner AIP: instalação e configuração

**Para instalar o scanner AIP, siga as diretrizes recomendadas:**

1. Se estiver a atualizar e não efetuar uma instalação limpa, certifique-se de que seguiu as orientações para a atualização do scanner de [proteção de informação Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e para o cliente de rotulagem unificado, consulte [a atualização do scanner de proteção de informação Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Verifique se cumpre todos os requisitos de definições de [firewalls e de infraestrutura](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)de rede.
3. Certifique-se de que as suas [políticas estão definidas](https://docs.microsoft.com/azure/information-protection/configure-policy) para a rotulagem automática ou tem um rótulo predefinido na política.
4. Certifique-se de que o tipo de ficheiro relevante está configurado para etiqueta/proteção, conforme descrito nos tipos de [ficheiros suportados pelo cliente de Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Além disso, se pretender alterar o comportamento predefinido, siga estas orientações: [Alterar o nível de proteção padrão dos ficheiros](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verifique se a conta de utilizador configurada para executar o serviço de scanner tem permissões para aceder a todos os repositórios configurados.
6. Se ainda tiver problemas, por favor exporte os registos do scanner e adicione-os ao seu bilhete de apoio.

**Registos de scanners de proteção de informação De exportação Azure**

1. Navegue para %localappdata%\Microsoft\MSIP no contexto do utilizador que executa o serviço de scanner.
2. Feche todos os conteúdos sob a pasta MSIP.
3. Guarde os registos à sua escolha de localização e prenda-os ao seu pedido de serviço.
4. Também pode utilizar [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Para obter informações adicionais, consulte:**
- [Implementação do scanner de proteção de informação Azure para classificar e proteger automaticamente ficheiros](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Especificar e utilizar o parâmetro Token para A Autenticação Set-AIP](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Executar um ciclo de descoberta e ver relatórios para o scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Rever documentação de proteção de informação do Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisitos para a proteção da informação do Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Baixar cliente de Proteção de Informação Azure](https://www.microsoft.com/download/details.aspx?id=53018)
