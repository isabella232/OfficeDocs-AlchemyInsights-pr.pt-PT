---
title: Criar e gerir etiquetas ou grupos de dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731964"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Criar e gerir etiquetas ou grupos de dispositivos

Adicione etiquetas em dispositivos para criar uma afiliação de grupo lógica. As etiquetas de dispositivo suportam o mapeamento adequado da rede, permitindo-lhe anexar etiquetas diferentes para capturar o contexto e permitir a criação de listas dinâmicas como parte de um incidente. As etiquetas podem ser utilizadas como um filtro na vista de lista Dispositivos ou para agrupar dispositivos. Para obter mais informações sobre o agrupamento de dispositivos, [consulte Criar e gerir etiquetas de dispositivo.](/microsoft-365/security/defender-endpoint/machine-tags)

Pode adicionar etiquetas nos dispositivos ao:

- Utilizar o portal

- Definir um valor de chave de registo
 
**Nota:** Pode haver latência entre o tempo em que uma etiqueta é adicionada a um dispositivo e a res suas disponibilidade na lista de dispositivos e na página do dispositivo.

Para adicionar etiquetas de dispositivo através da API, consulte [Adicionar ou remover API de etiquetas de dispositivo.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)

## <a name="add-and-manage-device-tags-using-the-portal"></a>Adicionar e gerir etiquetas de dispositivo utilizando o portal

1. Selecione o dispositivo em que pretende gerir as etiquetas. Pode selecionar ou procurar um dispositivo a partir de qualquer uma das seguintes vistas:

    - **Dashboard de operações de segurança** Selecione o nome do dispositivo a partir da secção Principais dispositivos com alertas ativos.
    - **Fila de alertas -** Selecione o nome do dispositivo junto ao ícone do dispositivo a partir da fila de alertas.
    - **Lista de dispositivos** – selecione o nome do dispositivo a partir da lista de dispositivos.
    - **Caixa de pesquisa** - Selecione Dispositivo a partir do menu de menu de lista e introduza o nome do dispositivo.

    Também pode chegar à página de alerta através das vistas de ficheiro e IP.

1. **Selecione Gerir Etiquetas** na linha de Ações de resposta.

1. Escreva para encontrar ou criar etiquetas.

As etiquetas são adicionadas à vista dispositivo e são refletidas na vista de lista Dispositivos. Em seguida, pode utilizar o filtro Etiquetas para ver a lista de dispositivos relevante.

Para obter mais informações, consulte [Criar e gerir etiquetas de dispositivo.](/microsoft-365/security/defender-endpoint/machine-tags)