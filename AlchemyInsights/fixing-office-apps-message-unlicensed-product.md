---
title: Não é possível ativar o Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704941"
---
# <a name="unable-to-activate-office"></a>Não é possível ativar o Office

- Verifique se o seu estado de subscrição expirou.
- Certifique-se de que tem uma subscrição que permite licenças de clientes, como o Microsoft 365 Apps para Pequenas e Médias Empresas ou o Microsoft 365 Empresas Premium e [assegure-se de que o utilizador tem uma licença atribuída](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Certifique-se de que o utilizador está a iniciar sessão no Office com a mesma conta à qual tem a licença atribuída.
- Consulte a [página do Estado de Funcionamento dos Serviços do Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver se existem problemas conhecidos com o serviço.
- Verifique as definições da firewall, software antivírus e proxy para confirmar que não estão a bloquear o acesso do Microsoft 365 Apps à internet. Consulte [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Intervalos de endereços IP e URLs do Office 365").

**Sugestão** Em computadores Windows, podemos diagnosticar e corrigir automaticamente vários problemas comuns de início de sessão do Office. Transfira e execute o **[Assistente de Recuperação e Suporte da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para utilizar a nossa ferramenta automatizada.

Utilize as seguintes ações de resolução de problemas:

- Abra uma aplicação do Office e [termine sessão](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) em quaisquer uma das contas de utilizador existentes. [Remova](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [reatribua](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [inicie sessão no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) com a conta de utilizador afetada.
- Execute a [Resolução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Redefina o estado de ativação do Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Redefinir o estado de ativação do Office")
- [Execute uma Reparação Online do Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Para soluções adicionais de resolução de problemas, consulte:  

- [Erros de Produto Não Licenciado e de ativação no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Erro "Desculpe, mas não conseguimos ligar-nos à sua conta. Tente novamente mais tarde" ao ativar o Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)