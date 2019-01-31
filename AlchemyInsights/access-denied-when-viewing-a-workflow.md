---
title: Acesso negado quando estiver a ver um fluxo de trabalho
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29484078"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c70d4-102">Acesso negado quando estiver a ver um fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="c70d4-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c70d4-103">Fluxos de trabalho do SharePoint 2013 que tentar enviar mensagens de correio electrónico a um grupo SharePoint pode falhar com uma mensagem de erro "Acesso negado" se os membros do grupo do SharePoint não está definido para todos os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="c70d4-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c70d4-104">**Para resolver este problema, execute estes passos:**</span><span class="sxs-lookup"><span data-stu-id="c70d4-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c70d4-105">Permitir que todas as pessoas ver os membros do grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c70d4-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="c70d4-106">Remova o grupo do SharePoint para ou CC linha da mensagem de correio electrónico.</span><span class="sxs-lookup"><span data-stu-id="c70d4-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="c70d4-107">Adicionar explicitamente os utilizadores para ou CC linha se não pode ser alterada a visibilidade de membros de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c70d4-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="c70d4-108">Para ver mais detalhes consulte [HTTP não autorizado para /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c70d4-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  
