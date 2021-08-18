---
title: Não é possível ativar o Office
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
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327857"
---
# <a name="unable-to-activate-office"></a>Não é possível ativar o Office

**Nota:** se estiver a utilizar uma versão mais antiga do Windows (por exemplo, o Windows 7), certifique-se de que o TLS 1.2 está ativado como predefinição. Para obter mais informações, consulte Update [to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- Verifique se o seu estado de subscrição expirou.
- Certifique-se de que tem uma subscrição que permite licenças de clientes, como o Microsoft 365 Apps para Pequenas e Médias Empresas ou o Microsoft 365 Empresas Premium e [assegure-se de que o utilizador tem uma licença atribuída](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
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