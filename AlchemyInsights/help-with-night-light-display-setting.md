---
title: Ajuda com a definição de visualização de luz noturna
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405177"
---
# <a name="help-with-the-night-light-display-setting"></a>Ajuda com a definição de visualização de luz noturna

Para saber mais sobre as definições do visor noturno, consulte [definir o seu visor para a noite no Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Se as opções de luz noturna estiverem acinzentadas nas Definições, verifique o controlador de visualização: 

1. Clique na caixa de pesquisa na sua barra de tarefas e escreva **o Gestor de Dispositivos** e, em seguida, selecione **o Gestor de Dispositivos** nos resultados da pesquisa.
1. Expandir **os adaptadores do Ecrã**. 

Infelizmente, a função de luz noturna não está disponível se o seu dispositivo utilizar um controlador DisplayLink ou um controlador de exibição básico.

A função de luz noturna utiliza a tecnologia gráfica recente, pelo que poderá ter de atualizar o controlador de ecrã:  

- Verifique se há atualizações indo para **iniciar**  >  a atualização **de definições**  >  **&** verificação da atualização do Windows de segurança  >    >  **para obter atualizações**.  

OU

- Visite o site de suporte do fabricante de hardware para descarregar manualmente e instalar os controladores de exibição mais recentes.

## <a name="reset-night-light-in-the-registry"></a>Repor a luz noturna no registo

Se a atualização do controlador de visualização não funcionar, poderá ter de repor a luz noturna no registo.  

**Atenção:** Este passo de resolução de problemas é recomendado apenas para utilizadores avançados. Podem ocorrer problemas graves se modificar o registo incorretamente. Para uma proteção adicional, faça uma responsabilidade no registo antes de o modificar para que possa restaurá-lo em caso de problemas.

1. Na caixa de pesquisa, **escreva regedit** e, em seguida, selecione **Editor de Registo** nos resultados da pesquisa.

1. Aceda à seguinte chave de registo: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exportar e, em seguida, eliminar o seguinte sub-teísta:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exporte e, em seguida, elimine o seguinte sub-chave:$$windows.data.bluelightreduction.settings

1. Reinicie o Windows e verifique se as opções de luz noturna estão disponíveis.


