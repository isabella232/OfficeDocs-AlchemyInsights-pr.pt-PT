---
title: 2681 simulador de ataque no Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305342"
---
# <a name="attack-simulator-in-office-365"></a>Simulador de ataque no Office 365

- Você está faltando simulador de ataque? O simulador de ataque requer o **office 365 Advanced Threat Protection Plan 2 (plano ATP 2)** ou o **Office 365 Enterprise E5**. O simulador de ataque **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (plano ATP 1), Office 365 Enterprise E3 ou qualquer assinatura do Office 365 Business.

- A conta que você usa para iniciar ataques simulados requer permissões de administrador global ou de segurança e autenticação multifator (MFA). Para obter mais informações sobre os requisitos do simulador de ataque, consulte [Este tópico](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Coisas importantes para saber sobre **Brute Force** simulações de ataque de senha:

  - Se a conta de destino tiver a MFA ativada e a senha foi adivinhada corretamente, a conta não será mostra como comprometida (o segundo fator de autenticação será incompleto).

  - O arquivo de senha não pode ser maior que 10 MB. Use uma senha por linha e inclua uma linha em branco (retorno de carro) após a última senha na lista.

- Coisas importantes a saber sobre simulações de **lança de phishing** :

  - Por predefinição, não pode fornecer um valor personalizado para a **URL do servidor de início de sessão de phishing**.

  - Se um destinatário usar a [opção Habilitar o suplemento relatar mensagem](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para relatar a mensagem como phishing, talvez você não receba alertas para a mensagem (porque este é um ataque simulado).

- Relatórios: após a conclusão do ataque simulado, você pode clicar em **detalhes de ataque** para ver o relatório.

- Para obter instruções detalhadas e novos recursos no simulador de ataque, consulte [simulador de ataque no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
