---
title: Dia de trabalho para fornecimento de utilizadores ad vai para o estado de quarentena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481882"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="daf97-102">Dia de trabalho para fornecimento de utilizadores ad vai para o estado de quarentena</span><span class="sxs-lookup"><span data-stu-id="daf97-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="daf97-103">**Dia de trabalho para fornecimento de utilizadores ad entra em estado de quarentena e nenhum utilizador é criado em AD**</span><span class="sxs-lookup"><span data-stu-id="daf97-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="daf97-104">O trabalho de Fornecimento de utilizadores de trabalho para a AD entrou em estado de quarentena e os registos de auditoria mostram eventos de falha de exportação com a mensagem de erro **Erro: OperationsError-SvcErr: Ocorreu um erro de operação. Não foi configurada qualquer referência superior para o serviço de diretório. O serviço de diretório é, portanto, incapaz de emitir referências a objetos fora desta floresta.**</span><span class="sxs-lookup"><span data-stu-id="daf97-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="daf97-105">Este erro geralmente aparece se o Contentor do Diretório Ativo OU não estiver corretamente definido ou se houver problemas com o Mapeamento de Expressão utilizado para **o nome de pais.**</span><span class="sxs-lookup"><span data-stu-id="daf97-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="daf97-106">Verifique o parâmetro padrão da **UA** para obter tipografias.</span><span class="sxs-lookup"><span data-stu-id="daf97-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="daf97-107">Certifique-se de que a OU especificada já existe no seu AD.</span><span class="sxs-lookup"><span data-stu-id="daf97-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="daf97-108">Se estiver a utilizar **o nome parentalDistinguishedname** no mapeamento do atributo, certifique-se de que avalia sempre um recipiente conhecido dentro do domínio AD.</span><span class="sxs-lookup"><span data-stu-id="daf97-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="daf97-109">Consulte o evento Exportação nos registos de auditoria para ver o valor gerado.</span><span class="sxs-lookup"><span data-stu-id="daf97-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="daf97-110">Para obter mais informações sobre a configuração do dia de trabalho para o provisionamento automatizado, consulte [Tutorial: Configure Workday para o provisionamento automático do utilizador](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="daf97-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

