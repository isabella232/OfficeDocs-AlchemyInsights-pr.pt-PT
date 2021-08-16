---
title: Exemplo do Microsoft Defender Office 365 uma política anti phishing
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035017"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exemplo do Microsoft Defender Office 365 uma política anti phishing

Estas definições ativam uma política *denominada Domínio e CEO.* Esta política fornece proteção de utilizador e domínio contra representação e, em seguida, aplica a política a todos os e-mails recebidos pelos utilizadores no domínio. Primeiro, adicione as seguintes informações para criar a política:

- **Nome**: Descrição do domínio **e** do CEO: garante que o Diretor Geral e o seu domínio não estão a ser representação.
  **Aplicado a**: Selecione **O domínio do destinatário é**. Em **Qualquer uma destas , selecione** Escolher **e,** em seguida, selecione um domínio. **Selecione + Adicionar**. Selecione a caixa de verificação junto ao nome do domínio na lista (por *exemplo,* contoso.com ) e, em seguida, selecione **Adicionar**. **Selecione Feito**.
- Após a criação da política, pode ojustá-la ao utilizar as seguintes opções:
  - **Adicionar utilizadores para proteger:** Para este exemplo, adicione, no mínimo, o endereço de e-mail do Diretor Geral.
  - **Adicione domínios para proteger:** adicione o domínio organizacional que inclui o escritório do CEO.
  - Selecione ações: Para Se o e-mail for enviado por um utilizador representação **,** selecione **Redirecionar** mensagem para outro endereço de e-mail e, em seguida, introduza o endereço de e-mail do administrador de segurança *(por* exemplo, securityadmin@contoso.com ). Em **Se o e-mail for enviado por um domínio representação**, selecione **Quarentena a mensagem**.
  - **Informações sobre caixas** de correio: por predefinição, esta opção é selecionada quando cria uma nova política anti phishing. Deixe esta definição **Ativos para** melhores resultados.
  - **Adicionar domínios e recetores de confiança:** Para este exemplo, não defina quaisquer substituições.
- Depois de rever as suas definições, **selecione Criar esta política ou** **Guardar**, conforme adequado.

Para saber mais, consulte [o artigo Políticas anti-phishing Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
