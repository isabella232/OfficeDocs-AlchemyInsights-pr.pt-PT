---
title: Corrigir problemas comuns com o Microsoft Defender para Office 365
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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898255"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Corrigir problemas comuns com o Microsoft Defender para Office 365

Eis algumas soluções para problemas comuns com o Microsoft Defender para Office 365:

- **Atraso de mensagens:**

  Os atrasos na entrega de e-mails podem Cofre a análise de anexos de mensagens. Para obter mais informações, consulte [Cofre de política Anexos.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Comunicar resultados falsos positivos ou negativos:**

  Para obter mais informações, consulte [Comunicar mensagens e ficheiros à Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Ativar Cofre Ligação de Ligação de Segurança:**

  1. No portal Microsoft 365 Defender, em , vá para E-mail & políticas de <https://security.microsoft.com/> **colaboração** & Regras contra \>  \>  \> **ameaças Cofre Ligações**  na secção Políticas.

     Para ir diretamente para **a página Cofre ligações,** utilize <https://security.microsoft.com/safelinksv2> .

  2. Na página **Cofre,** selecione a política ao clicar no nome da política.
  3. Na lista de listas de detalhes que é exibida, eis um dos seguintes passos:
     - Para adicionar uma nova política, selecione **+ Criar.** Será iniciado um assistente que o ajudará a definir as suas definições de política.
     - Para editar uma política existente, selecione a política clicando no nome da política. Na panfleto de detalhes que é exibida, **selecione Editar** **na secção Definições de** proteção.
  4. Na página **Definições de** proteção, configure as seguintes definições:
     - Ativar **Selecione a ação para URLs potencialmente maliciosos nas mensagens.**
     - **Selecione Aplicar ligações seguras a mensagens enviadas para a organização**.

  Para obter mais informações, [consulte Configurar políticas Cofre Ligações no Microsoft Defender para Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
