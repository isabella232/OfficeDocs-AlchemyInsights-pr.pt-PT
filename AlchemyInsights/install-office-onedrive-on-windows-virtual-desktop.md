---
title: Instalar Office e OneDrive Ambiente de trabalho Windows Virtual
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028627"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalar Office e OneDrive Ambiente de trabalho Windows Virtual

1. [Prepare e personalize uma imagem VHD principal.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Crie uma máquina virtual (VM) se ainda não tiver sido criada.

1. [Instale Office no modo de ativação do computador partilhado](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). A ativação do computador partilhado permite que múltiplos utilizadores acedam Office.

1. [Instale OneDrive no modo por máquina](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalmente, OneDrive é instalado por utilizador, mas aqui deve ser instalado por máquina.