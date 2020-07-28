---
title: Apple MDM Push Certificate ainda não foi criado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440014"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="88f54-102">Apple MDM Push Certificate ainda não foi criado</span><span class="sxs-lookup"><span data-stu-id="88f54-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="88f54-103">Um Certificado de Pressão MD da Apple (também conhecido como certificado apple push notification service (APNS) não foi configurado para a sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="88f54-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="88f54-104">Sem um Certificado de Pressão Apple MDM configurado, não é possível inscrever e gerir dispositivos iOS e Mac OS.</span><span class="sxs-lookup"><span data-stu-id="88f54-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="88f54-105">Depois de adicionar o certificado ao Intune, os utilizadores podem instalar a aplicação Portal da Empresa para inscrever os seus dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="88f54-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="88f54-106">**Selecione "Concordo".**</span><span class="sxs-lookup"><span data-stu-id="88f54-106">Select **"I agree."**</span></span> <span data-ttu-id="88f54-107">para dar permissão à Microsoft para enviar dados para a Apple.</span><span class="sxs-lookup"><span data-stu-id="88f54-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="88f54-108">Selecione **Descarregue o seu** pedido de assinatura de certificado Intune necessário para criar um certificado de pressão Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="88f54-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="88f54-109">O ficheiro é utilizado para solicitar um certificado de relação fiduciuada do Portal dos Certificados Apple Push.</span><span class="sxs-lookup"><span data-stu-id="88f54-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="88f54-110">Selecione **Crie o seu certificado de push MDM** para ir ao Portal dos Certificados apple push.</span><span class="sxs-lookup"><span data-stu-id="88f54-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="88f54-111">Inscreva-se com a sua empresa Apple ID e, em seguida, **selecione Criar um Certificado**.</span><span class="sxs-lookup"><span data-stu-id="88f54-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="88f54-112">Selecione **Choose File,** navegue no ficheiro de pedido de assinatura de certificado e, em seguida, escolha **Upload**.</span><span class="sxs-lookup"><span data-stu-id="88f54-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="88f54-113">Na página Confirmação, escolha **Descarregar** para descarregar o ficheiro certificado (.pem) e guardar o ficheiro localmente.</span><span class="sxs-lookup"><span data-stu-id="88f54-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="88f54-114">**Nota:** O certificado está associado ao Apple ID utilizado para criá-lo.</span><span class="sxs-lookup"><span data-stu-id="88f54-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="88f54-115">Como uma boa prática, use uma empresa Apple ID para tarefas de gestão, e certifique-se de que a caixa de correio é monitorizada por mais de uma pessoa ou usando uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="88f54-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="88f54-116">Nunca utilize um Apple ID pessoal.</span><span class="sxs-lookup"><span data-stu-id="88f54-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="88f54-117">Use o mesmo Apple ID para renovar o Apple Push Certificate a cada 12 meses.</span><span class="sxs-lookup"><span data-stu-id="88f54-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="88f54-118">Introduza o Apple ID usado para criar o seu certificado de push Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="88f54-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="88f54-119">Grave este ID como um lembrete para quando precisar de renovar o certificado.</span><span class="sxs-lookup"><span data-stu-id="88f54-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="88f54-120">Vá ao arquivo de certificado (.pem), escolha **Open**e, em seguida, escolha **Upload**.</span><span class="sxs-lookup"><span data-stu-id="88f54-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="88f54-121">Com o certificado push, o Intune pode inscrever-se e gerir dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="88f54-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>