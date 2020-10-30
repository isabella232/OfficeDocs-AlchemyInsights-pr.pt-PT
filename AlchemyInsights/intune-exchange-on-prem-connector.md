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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="bb830-102">Conector intune Exchange no local</span><span class="sxs-lookup"><span data-stu-id="bb830-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="bb830-103">Para obter informações sobre a configuração do conector entre Intune e Exchange, que está hospedado no local, consulte a seguinte documentação:</span><span class="sxs-lookup"><span data-stu-id="bb830-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="bb830-104">Configurar o conector de troca intune no Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="bb830-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="bb830-105">**Perguntas Frequentes:**</span><span class="sxs-lookup"><span data-stu-id="bb830-105">**FAQ:**</span></span>

<span data-ttu-id="bb830-106">P: Vejo um erro como "A versão Do Conector de Câmbio não é suportada" ao tentar configurar o conector Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb830-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="bb830-107">Qual pode ser a causa?</span><span class="sxs-lookup"><span data-stu-id="bb830-107">What could be the cause?</span></span>

<span data-ttu-id="bb830-108">R: A conta que está a usar é licenciada adequadamente - deve ter uma licença Intune ativa</span><span class="sxs-lookup"><span data-stu-id="bb830-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="bb830-109">P: É possível ter vários conectores exchange?</span><span class="sxs-lookup"><span data-stu-id="bb830-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="bb830-110">R: Só pode configurar um conector exchange per Intune por organização Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb830-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="bb830-111">O conector só pode ser instalado num servidor numa organização de troca de vários servidores.</span><span class="sxs-lookup"><span data-stu-id="bb830-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="bb830-112">Além disso, não é possível configurar conectores tanto para o Exchange on-in como para o Exchange Online configurados no mesmo inquilino.</span><span class="sxs-lookup"><span data-stu-id="bb830-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="bb830-113">P: O conector pode utilizar uma matriz CAS como ligação ao Exchange?</span><span class="sxs-lookup"><span data-stu-id="bb830-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="bb830-114">R: Especificar uma matriz CAS não é uma configuração suportada na configuração do conector.</span><span class="sxs-lookup"><span data-stu-id="bb830-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="bb830-115">Apenas um único servidor deve ser especificado e deve ser codificado no ficheiro de configuração do conector que pode ser encontrado em</span><span class="sxs-lookup"><span data-stu-id="bb830-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="bb830-116">dados do programa\microsoft\microsoft Intune no conector de troca de premissa\ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="bb830-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="bb830-117">Localize a seguinte entrada ```<ExchangeWebServiceURL />``` e substitua o URL pelo servidor de troca.</span><span class="sxs-lookup"><span data-stu-id="bb830-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="bb830-118">**Exemplo:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="bb830-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="bb830-119">Consulte a seguinte documentação para uma resolução adicional de [problemas: Resolução de problemas no conector de troca de Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="bb830-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="bb830-120">**Habilitação de registo verboso para o conector Exchange**</span><span class="sxs-lookup"><span data-stu-id="bb830-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="bb830-121">Abra o ficheiro de configuração de rastreio do conector de troca para edição.</span><span class="sxs-lookup"><span data-stu-id="bb830-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="bb830-122">O ficheiro está localizado em: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="bb830-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="bb830-123">**Exemplo:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="bb830-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="bb830-124">Localizar o TraceSourceLine com a seguinte tecla: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="bb830-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="bb830-125">Alterar o valor do nó SourceLevel de Atividade de InformaçãoTracing (o padrão) para Atividade verboseTracing</span><span class="sxs-lookup"><span data-stu-id="bb830-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="bb830-126">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="bb830-126">**Example:**</span></span>
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
4. <span data-ttu-id="bb830-127">Reiniciar o Serviço de Intercâmbio Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bb830-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="bb830-128">Sincronizar completamente no Portal Intune até terminar e, em seguida, alterar o XML de volta para "Information ActivityTracing" e reiniciar o Microsoft Intune Exchange Service.</span><span class="sxs-lookup"><span data-stu-id="bb830-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="bb830-129">A localização dos registos é: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="bb830-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>