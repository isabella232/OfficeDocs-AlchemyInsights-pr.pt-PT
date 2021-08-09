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
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934268"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scanner AIP: instalação e configuração

**Para instalar o scanner AIP, siga as diretrizes recomendadas:**

1. Se estiver a atualizar e não tiver uma instalação limpa, certifique-se de que seguiu as diretrizes para atualizar o [scanner Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e o cliente de etiquetagem unificado, consulte atualizar o [scanner Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Verifique se está em conformidade com todos os requisitos de [definições de infraestrutura de rede e Firewalls.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Certifique-se de [que as suas políticas estão](https://docs.microsoft.com/azure/information-protection/configure-policy) definidas para etiquetagem automática ou que têm uma etiqueta predefinida na política.
4. Certifique-se de que o tipo de ficheiro relevante está configurado para etiqueta/proteção conforme descrito em Tipos de ficheiro suportados pelo cliente [Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Além disso, se quiser alterar o comportamento predefinido, siga estas diretrizes: Alterar o nível de proteção [predefinido dos ficheiros.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Verifique se a conta de utilizador configurada para executar o serviço de scanner tem permissões para aceder a todos os repositórios configurados.
6. Se continuar a ter problemas, exporte os registos do scanner e adicione-os ao seu bilhete de suporte.

**Exportar registos do Azure Information Protection Scanner**

1. Navegue até %localappdata%\Microsoft\MSIP no contexto do utilizador que executa o serviço de scanner.
2. Zipar todos os conteúdos na pasta MSIP.
3. Guarde os registos numa localização à sua escolha e anexe-os ao seu pedido de serviço.
4. Também pode utilizar [Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Para obter informações adicionais, consulte:**
- [Implementar o scanner do Azure Information Protection para classificar e proteger ficheiros automaticamente](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Especificar e utilizar o parâmetro Token para Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Executar um ciclo de deteção e ver relatórios para o scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Rever a documentação do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisitos do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Transferir cliente do Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
