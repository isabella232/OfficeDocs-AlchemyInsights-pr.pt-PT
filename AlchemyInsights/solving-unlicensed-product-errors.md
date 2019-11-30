---
title: Resolvendo erros de produto não licenciados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 178811c81775b22676a0106283be4e516d40a95b
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628037"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Sugestões para resolver erros de "produto não licenciado"

Para resolver erros sobre um "produto não licenciado", experimente o seguinte:

- Verifique se o status da assinatura expirou.
- Certifique-se de ter uma assinatura que permite licenças de clientes, como office 365 Business ou Business Premium, e [garantir que o usuário tenha uma licença atribuída](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users). 
- Certifique-se de que o usuário está inscrevendo no Office com a mesma conta que tem a licença atribuída.
- Verifique a página de saúde do [Serviço 365](https://docs.microsoft.com/office365/enterprise/view-service-health) do Escritório para ver se há algum problema conhecido com o serviço.
- Verifique seu firewall, software antivírus e configurações de proxy para confirmar que eles não estão bloqueando o acesso de aplicativos do Office à Internet. Veja [o Office 365 URLs e as faixas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)de endereço IP.

Você também pode tentar as seguintes ações de solução de problemas: 

- Abra um aplicativo do Office e [inscreva-se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) em todas as contas de usuário existentes. [Remover](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) e [reatribuir](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [entrar no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.
- Executar o [troubleshooter ativação](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Redefinir o estado de ativação do Escritório](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Realizar um reparo on-line do escritório](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Para soluções adicionais de solução de problemas, veja: 

- [Erros não licenciados do produto e da ativação no escritório](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["Desculpe, não podemos nos conectar à sua conta. Por favor, tente novamente mais tarde" erro quando você ativar office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)