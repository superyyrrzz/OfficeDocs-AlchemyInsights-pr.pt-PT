---
title: Acesso a resolução de problemas Mensagens negadas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505390"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Acesso a resolução de problemas Mensagens negadas no Sharepoint/OneDrive Admin Center

Se estiver a receber uma mensagem de acesso negada ao tentar navegar para um Sharepoint/OneDrive Admin Center, certifique-se de que [atribui uma licença ao utilizador](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Se o utilizador tiver uma licença, deve também certificar-se de que lhes é [atribuída uma função de administrador](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) que pode aceder aos centros de administração.

Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN). A nova conta é criada utilizando um valor puid diferente (Passport Unique ID). Quando o utilizador tenta aceder a uma coleção de sites ou ao seu OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional ative directy (OU). Se os utilizadores já se inscreveram no SharePoint, e depois forem transferidos para um OU diferente e resincamados com o SharePoint, poderão experimentar este problema.

Para resolver este problema, deverá restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Nota: Se um centro de administração OneDrive ou SharePoint não estiver disponível para vários utilizadores que tenham tido acesso anteriormente, pode haver um problema de serviço temporário.  [Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)


