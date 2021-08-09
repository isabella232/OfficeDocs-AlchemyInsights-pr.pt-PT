---
title: Conceitos de autenticação avançados aplicáveis às Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934376"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Conceitos de autenticação avançados aplicáveis às Microsoft Edge

Seguem-se os conceitos de autenticação avançados aplicáveis às Microsoft Edge:

**Autenticação Proativa**

Quando ativar a política [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) o Microsoft Edge tentará autenticar de forma proativa os utilizadores com acesso serviços Microsoft. Em intervalos regulares, utilizará um serviço online para procurar um manifesto atualizado que contenha a configuração que governa a Autenticação Proativa.

Vantagens: a Autenticação Proativa permite a autenticação para serviços principais, Office Nova Página de Separador. Além disso, se Bing for utilizado como motor de busca, a Autenticação Proativa melhora o desempenho da barra de endereço e ajuda a gerar resultados de pesquisa personalizados para as necessidades do seu negócio.

**Windows Hello CredUI para Autenticação NTLM**

Se o SSO (single sign on) não estiver disponível quando um site tentar iniciá-lo no utilizador através do mecanismo NTLM ou Negotiate, esta funcionalidade permitirá ao utilizador partilhar as credenciais do SO com o site e satisfazer o desafio da autenticação através da IU do Windows Hello. Este fluxo de acesso só será apresentado no Windows 10 e apenas para os utilizadores que não o obterem durante um NTLM ou um desafio de Negociação.

**Utilizar palavras-passe guardadas para assinar automaticamente**

Os utilizadores que guardam palavras-passe Microsoft Edge podem ativar o lote automático em sites onde as credenciais foram guardadas. Os utilizadores podem ativar ou destivar esta funcionalidade no edge://settings/passwords e pode configure-a nas políticas do gestor [de palavras-passe.](https://go.microsoft.com/fwlink/?linkid=2134622)
