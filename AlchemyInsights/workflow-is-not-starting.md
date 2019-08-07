---
title: Não está a iniciar o fluxo de trabalho
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171803"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="acda6-102">Não está a iniciar o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="acda6-102">Workflow is not starting</span></span>

- <span data-ttu-id="acda6-103">Fluxos de trabalho do SharePoint 2010 e 2013 do SharePoint não estão a iniciar.</span><span class="sxs-lookup"><span data-stu-id="acda6-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    <span data-ttu-id="acda6-104">Se não estiver a iniciar o fluxo de trabalho, poderá existir um problema de serviço temporária onde os utilizadores poderão verificar atrasos intermitentes com o progresso de fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="acda6-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="acda6-105">Verifique se o [Serviço de saúde Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se a sua organização é afectada.</span><span class="sxs-lookup"><span data-stu-id="acda6-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    <span data-ttu-id="acda6-106">Se tiverem passado mais de 24 horas desde que a visualizou pela primeira vez a este problema, inicie uma permissão de suporte.</span><span class="sxs-lookup"><span data-stu-id="acda6-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="acda6-107">Em muitos casos, a Microsoft já estiver a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="acda6-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="acda6-108">Forneça pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="acda6-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="acda6-109">Fluxos de trabalho do SharePoint 2010 atrasada no início.</span><span class="sxs-lookup"><span data-stu-id="acda6-109">SharePoint 2010 workflows delayed on start.</span></span>

    <span data-ttu-id="acda6-110">Isto ocorre se o fluxo de trabalho é accionado em grandes lotes.</span><span class="sxs-lookup"><span data-stu-id="acda6-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="acda6-111">(por exemplo, quando vários itens são adicionados ao mesmo tempo).</span><span class="sxs-lookup"><span data-stu-id="acda6-111">(for example, when several items are added at once).</span></span>

    <span data-ttu-id="acda6-112">Fluxos de trabalho não foram concebidos para funcionar em tempo real, por isso um atraso é o comportamento de design.</span><span class="sxs-lookup"><span data-stu-id="acda6-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

    <span data-ttu-id="acda6-113">Se o fluxo de trabalho complexos Extensible objecto Markup Language (XMOL), compilação pode ser lenta.</span><span class="sxs-lookup"><span data-stu-id="acda6-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="acda6-114">Consulte [Este](https://support.microsoft.com/en-us/kb/3043697) artigo.</span><span class="sxs-lookup"><span data-stu-id="acda6-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    <span data-ttu-id="acda6-115">Deve simplificar o fluxo de trabalho ou adaptá-lo utilizando o tipo de plataforma de fluxo de trabalho do Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="acda6-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    <span data-ttu-id="acda6-116">Além disso, se tiver aumentado o histórico de fluxo de trabalho, poderá pretender remover os itens ou criar uma nova lista do histórico.</span><span class="sxs-lookup"><span data-stu-id="acda6-116">Also, if your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

    <span data-ttu-id="acda6-117">Obter mais informações: [Limpar o histórico de fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="acda6-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="acda6-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="acda6-118">Related topics</span></span>
<span data-ttu-id="acda6-119">Pretende tentar fluxo reabertos no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="acda6-119">Want to try Micrsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="acda6-120">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="acda6-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="acda6-121">Fluxo e do SharePoint</span><span class="sxs-lookup"><span data-stu-id="acda6-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

