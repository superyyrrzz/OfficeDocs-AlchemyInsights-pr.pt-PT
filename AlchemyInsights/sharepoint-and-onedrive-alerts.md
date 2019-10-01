---
title: Não receber alertas do SharePoint e do OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205545"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="c44c2-102">Não receber alertas do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="c44c2-102">Not receiving SharePoint and OneDrive alerts</span></span>

<span data-ttu-id="c44c2-103">Primeiro, verifique a pasta junk ou spam no seu e-mail.</span><span class="sxs-lookup"><span data-stu-id="c44c2-103">First check the Junk or Spam folder in your email.</span></span>

<span data-ttu-id="c44c2-104">Em seguida, determine se **todos os alertas não são entregues** ou se **um alerta individual** de um arquivo ou biblioteca específico não é entregue.</span><span class="sxs-lookup"><span data-stu-id="c44c2-104">Then determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="c44c2-105">Se **todos os alertas de vários arquivos ou bibliotecas não forem entregues**, visite o [painel de integridade do serviço](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) para verificar se há avisos/incidentes que possam estar ocorrendo com o SharePoint ou o Exchange.</span><span class="sxs-lookup"><span data-stu-id="c44c2-105">If **all alerts from multiple files or libraries are not delivered**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="c44c2-106">O problema pode estar com o recurso de alerta do SharePoint ou atrasos nos emails por meio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c44c2-106">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="c44c2-107">Observe também se outro e-mail está sendo entregue — se não, o problema é provavelmente com atrasos do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c44c2-107">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="c44c2-108">Se **um alerta individual de um arquivo ou biblioteca específico não for entregue**, tente excluí-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="c44c2-108">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="c44c2-109">Consulte [gerenciar, exibir ou excluir alertas do SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="c44c2-109">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="c44c2-110">Os alertas não podem ser enviados para um grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c44c2-110">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="c44c2-111">Somente os grupos de segurança e O365 são suportados.</span><span class="sxs-lookup"><span data-stu-id="c44c2-111">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="c44c2-112">Não é possível personalizar modelos de email de alerta.</span><span class="sxs-lookup"><span data-stu-id="c44c2-112">You cannot customize alert email templates.</span></span> <span data-ttu-id="c44c2-113">Você deve usar o fluxo de trabalho do Microsoft Flow ou do SharePoint Designer para alcançá-los.</span><span class="sxs-lookup"><span data-stu-id="c44c2-113">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>