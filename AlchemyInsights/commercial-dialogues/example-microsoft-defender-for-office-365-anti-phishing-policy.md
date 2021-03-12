---
title: Exemplo Microsoft Defender para a política anti-phishing do Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750793"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exemplo Microsoft Defender para a política anti-phishing do Office 365

Estas definições permitem uma política chamada *Domínio e CEO*. Esta política fornece proteção de utilizador e de domínio contra a personificação e, em seguida, aplica a política a todos os e-mails recebidos pelos utilizadores dentro do domínio. Em primeiro lugar, adicione as seguintes informações para criar a política:

- **Nome**: **Descrição** do domínio e do CEO : Garante que o CEO e o seu domínio não estão a ser personificados.
  **Aplicado a**: Selecione **O domínio do destinatário é**. Em **qualquer um destes**, selecione **Escolha** e, em seguida, selecione um domínio. Selecione **+ Adicionar**. Selecione a caixa de verificação ao lado do nome do domínio na lista (por exemplo, *contoso.com*), e, em seguida, selecione **Adicionar**. Selecione **Feito**.
- Após a criação da apólice, pode afinar a política utilizando as seguintes opções:
  - **Adicione utilizadores para proteger:** Para este exemplo, adicione o endereço de e-mail do CEO, no mínimo.
  - **Adicionar domínios para proteger:** Adicione o domínio organizacional que inclui o escritório do CEO.
  - **Escolha as ações**: Para **se o e-mail for enviado por um utilizador personificado,** selecione **Redirecionar a mensagem para outro endereço de e-mail** e, em seguida, insira o endereço de e-mail do administrador de segurança (por exemplo, *securityadmin@contoso.com).* Para **se o e-mail for enviado por um domínio personificado,** selecione **Quarantine a mensagem**.
  - **Inteligência da caixa de** correio : Por padrão, esta opção é selecionada quando cria uma nova política anti-phishing. Deixe esta definição **On** para obter os melhores resultados.
  - **Adicionar remetentes e domínios fidedignos:** Para este exemplo, não defina nenhuma sobreposição.
- Depois de rever as definições, **selecione Criar esta política** ou **Guardar,** conforme apropriado.

Para saber mais, consulte [as políticas anti-phishing na Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
