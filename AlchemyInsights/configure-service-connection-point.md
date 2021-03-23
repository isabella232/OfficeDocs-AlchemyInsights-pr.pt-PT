---
title: Configure ponto de ligação de serviço (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037285"
---
# <a name="configure-service-connection-point-scp"></a>Configure ponto de ligação de serviço (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Razão**: Incapaz de ler o objeto SCP e obter a informação do inquilino da AD AZure
- **Resolução**: Consulte a secção [Configurar um Ponto de Ligação de Serviço](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Plano de ação**

- Verifique se o dispositivo recebeu o GPO para a validação controlada.
- Certifique-se de que o GPO criou as chaves de registo.
- Certifique-se de que tem 2 teclas criadas com o seu ID do Diretório e o domínio onmicrosoft.

**Configurar a definição de registo do lado do cliente para o SCP**

Utilize o exemplo seguinte para criar um Objeto de Política de Grupo (GPO) para implementar uma definição de registo que configura uma entrada SCP no registo dos seus dispositivos.

1. Abra uma consola de Gestão de Políticas de Grupo e crie um novo GPO no seu domínio.
     - Forneça ao seu gpo recém-criado um nome (por exemplo, ClientSideSCP)

2. Editar o GPO e localizar o seguinte caminho: **Configuração do computador > Preferências > Definições do Windows > Registo**.

3. Clique com o botão direito no **Registo** e selecione **New > Registry Item**.

4. No separador **Geral,** configure o seguinte:
  
- **Ação**: Atualização
    
- **Colmeia**: HKEY_LOCAL_MACHINE
    
- **Caminho chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nome de valor**: TenantId
    
- **Tipo de valor**: REG_SZ
    
- **Dados de valor**: O ID GUID ou Diretório da sua instância AD Azure (Este valor pode ser encontrado no **portal Azure > Azure Ative Directy > Properties > Diretório ID)**
 
- Clique em **OK**.
 
5. Clique com o botão direito no **Registo** e selecione **New > Registry Item**.

6. No separador **Geral,** configure o seguinte:
  
- **Ação**: Atualização
    
- **Colmeia**: HKEY_LOCAL_MACHINE
    
- **Caminho chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nome de valor**: Nome do Inquilino
    
- **Tipo de valor**: REG_SZ
    
- **Dados de valor**: O seu nome de domínio verificado se estiver a utilizar ambientes federados, como AD FS. O seu nome de domínio verificado ou o seu nome de domínio onmicrosoft.com (por exemplo, contoso.onmicrosoft).com se estiver a utilizar ambiente gerido

- Clique em **OK**.

7. Feche o editor para o recém-criado GPO.

8. Ligue o GPO recém-criado ao or desejado contendo computadores ligados ao domínio que pertencem à sua população de implantação controlada.

Para mais informações, consulte [a validação controlada da ad híbrida Azure - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) e  [Troubleshoot híbrido Azure Ative Directory juntou dispositivos | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









