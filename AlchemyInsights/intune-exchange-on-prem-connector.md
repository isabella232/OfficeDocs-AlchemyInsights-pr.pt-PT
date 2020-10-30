---
title: Conector intune Exchange no local
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808145"
---
# <a name="intune-exchange-on-premise-connector"></a>Conector intune Exchange no local

Para obter informações sobre a configuração do conector entre Intune e Exchange, que está hospedado no local, consulte a seguinte documentação:

[Configurar o conector de troca intune no Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Perguntas Frequentes:**

P: Vejo um erro como "A versão Do Conector de Câmbio não é suportada" ao tentar configurar o conector Exchange. Qual pode ser a causa?

R: A conta que está a usar é licenciada adequadamente - deve ter uma licença Intune ativa

P: É possível ter vários conectores exchange?

R: Só pode configurar um conector exchange per Intune por organização Exchange. O conector só pode ser instalado num servidor numa organização de troca de vários servidores.

Além disso, não é possível configurar conectores tanto para o Exchange on-in como para o Exchange Online configurados no mesmo inquilino.

P: O conector pode utilizar uma matriz CAS como ligação ao Exchange?

R: Especificar uma matriz CAS não é uma configuração suportada na configuração do conector. Apenas um único servidor deve ser especificado e deve ser codificado no ficheiro de configuração do conector que pode ser encontrado em

dados do programa\microsoft\microsoft Intune no conector de troca de premissa\ OnpremiseExchangeConnectorServiceConfiguration.xml

Localize a seguinte entrada ```<ExchangeWebServiceURL />``` e substitua o URL pelo servidor de troca.

**Exemplo:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consulte a seguinte documentação para uma resolução adicional de [problemas: Resolução de problemas no conector de troca de Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Habilitação de registo verboso para o conector Exchange**

1. Abra o ficheiro de configuração de rastreio do conector de troca para edição.  
O ficheiro está localizado em: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exemplo:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Localizar o TraceSourceLine com a seguinte tecla: OnPremisesExchangeConnectorService  
  
3. Alterar o valor do nó SourceLevel de Atividade de InformaçãoTracing (o padrão) para Atividade verboseTracing  

**Exemplo:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Reiniciar o Serviço de Intercâmbio Microsoft Intune  
5. Sincronizar completamente no Portal Intune até terminar e, em seguida, alterar o XML de volta para "Information ActivityTracing" e reiniciar o Microsoft Intune Exchange Service.  
6. A localização dos registos é: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`