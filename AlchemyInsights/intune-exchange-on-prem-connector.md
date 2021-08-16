---
title: Intune Exchange Conector no local
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013975"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange Conector no local

Para obter detalhes sobre como configurar o conector entre o Intune e Exchange que está alonhado no local, consulte a seguinte documentação:

[Configurar o conector de rede local do Intune Exchange no Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

P: Vejo um erro como "A versão do conector de Exchange não é suportada" ao tentar configurar o conector Exchange rede. Qual poderá ser a causa?

A: A conta que está a utilizar é licenciada de forma adequada - tem de ter uma licença do Intune ativa

P: É possível ter múltiplas conexões Exchange rede?

A: Só pode configurar um conector Exchange por inquilino do Intune por cada Exchange organização. O conector só pode ser instalado num servidor numa organização multi server exchange.

Além disso, não pode ter conectores configurados para Exchange no local e Exchange Online configurados no mesmo inquilino.

P: A conexão pode utilizar uma matriz CAS como a sua ligação a Exchange?

A: Especificar uma matriz de CAS não é uma configuração suportada na configuração do conector. Só deve ser especificado um único servidor e estar hardcoded no ficheiro de configuração do conector no qual se pode encontrar

dados de programa\microsoft\microsoft Intune no local Exchange conector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Localize a seguinte ```<ExchangeWebServiceURL />``` entrada e substitua o URL pelo servidor exchange.

**Exemplo:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consulte a seguinte documentação para obter remoção de problemas adicionais: Remoção de problemas do conector de rede [Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) no local

**Ativar o registo Verboso para o conector Exchange dados**

1. Abra o ficheiro Exchange de configuração de rastreamento do Conector para edição.  
O ficheiro encontra-se em : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exemplo:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Localize a TraceSourceLine com a seguinte chave: OnPremisesExchangeConnectorService  
  
3. Alterar o valor do nó de NívelDe Origem de Rastreamento de Atividade de Informações (a predefinição) para Rastreamento de Atividade Verboso  

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
4. Reiniciar o Microsoft Intune Exchange Serviço  
5. Sincronização completa no Portal do Intune até terminar e, em seguida, altere o XML novamente para "Rastreamento de Atividade de Informações" e reinicie o Microsoft Intune Exchange Serviço.  
6. A localização dos registos é: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`