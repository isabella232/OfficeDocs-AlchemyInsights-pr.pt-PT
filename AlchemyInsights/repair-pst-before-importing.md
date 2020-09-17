---
title: Reparar ficheiro .pst antes de importar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799107"
---
# <a name="repair-pst-file-before-importing"></a>Reparar ficheiro .pst antes de importar

Antes de importar um ficheiro .pst no Outlook, verifique se o ficheiro não é corrompido reparando o ficheiro:

1. Saia do Outlook.

2. Encontre e corra `Scanpst.exe` na pasta do programa Office (C:\Program Files (x86)\Microsoft Office\root\Office ou \<Version\> C:\Program Files\Microsoft Office\root\Office \<Version\> ).

3. Na **ferramenta de reparação**de caixas de entrada do Microsoft Outlook, clique em **procurar** no ficheiro .pst (por exemplo, em C:\Os utilizadores \\<nome de utilizador \> \AppData\Local\Microsoft\Outlook). Selecione o ficheiro .pst e, em seguida, clique em **Abrir**.

4. Clique **em Iniciar** a digitalização.

5. Se forem encontrados erros no ficheiro, clique em **Reparar**e clique **em OK** quando a reparação estiver concluída.

6. Tente importar o ficheiro .pst no Outlook novamente.

Para obter mais informações, consulte [os ficheiros de dados do Repair Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) e [corrija problemas de importação de um ficheiro Outlook .pst](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
