---
title: 'Scanner AIP: instalação e configuração'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821674"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scanner AIP: instalação e configuração

**Para instalar o scanner AIP, siga as orientações recomendadas:**

1. Se estiver a atualizar e não realizar uma instalação limpa, certifique-se de que seguiu as orientações para [atualizar o scanner de Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e para o cliente de rotulagem unificado, consulte a [atualização do scanner de Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Verifique se cumpre todos os [requisitos de definição de firewalls e infraestruturas de rede](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Certifique-se de que as suas [políticas estão definidas](https://docs.microsoft.com/azure/information-protection/configure-policy) para a rotulagem automática ou tem um rótulo predefinido na política.
4. Certifique-se de que o tipo de ficheiro relevante está configurado para etiqueta/proteção, conforme descrito nos [tipos de ficheiros suportados pelo cliente Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Além disso, se pretender alterar o comportamento predefinido, siga estas diretrizes: [Alterar o nível de proteção predefinido dos ficheiros](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verifique se a conta de utilizador configurada para executar o serviço de scanner tem permissões para aceder a todos os repositórios configurados.
6. Se ainda tiver problemas, por favor exporte os registos do scanner e adicione-os ao seu bilhete de apoio.

**Exportar registos de scanners de proteção de informação Azure**

1. Navegue para %localappdata%\Microsoft\MSIP no contexto do utilizador que executa o serviço de scanner.
2. Feche todos os conteúdos sob a pasta MSIP.
3. Guarde os registos numa localização à sua escolha e anexe-os ao seu pedido de serviço.
4. Também pode utilizar [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Para obter informações adicionais, consulte:**
- [Implantação do scanner de Proteção de Informação Azure para classificar e proteger automaticamente ficheiros](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Especifique e utilize o parâmetro Token para Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Executar um ciclo de descoberta e ver relatórios para o scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Rever a documentação do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisitos do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Transferir cliente do Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
