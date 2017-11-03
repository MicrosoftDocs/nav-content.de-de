---
title: "Designdetails – Umgang mit Wiederbeschaffungsrichtlinien"
description: "Übersicht über Aufgaben für das Definieren einer Wiederbestellungsrichtlinie in die Beschaffungsplanung."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2cd1d0e770e5fd7daa92e98486038aefdb678c5a
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-handling-reordering-policies"></a><span data-ttu-id="9ff8c-103">Designdetails: Umgang mit Wiederbeschaffungsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="9ff8c-103">Design Details: Handling Reordering Policies</span></span>
<span data-ttu-id="9ff8c-104">Damit ein Artikel an der Beschaffungsplanung teilnehmen kann, muss eine Wiederbeschaffungsrichtlinie festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="9ff8c-104">For an item to participate in supply planning, a reorder policy must be defined.</span></span> <span data-ttu-id="9ff8c-105">Die folgenden vier Wiederbeschaffungsrichtlinien sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="9ff8c-105">The following four reordering policies exist:</span></span>  
  
* <span data-ttu-id="9ff8c-106">Feste Bestellmenge</span><span class="sxs-lookup"><span data-stu-id="9ff8c-106">Fixed Reorder Qty.</span></span>  
* <span data-ttu-id="9ff8c-107">Auffüllen auf Maximalbestand</span><span class="sxs-lookup"><span data-stu-id="9ff8c-107">Maximum Qty.</span></span>  
* <span data-ttu-id="9ff8c-108">Bestellung</span><span class="sxs-lookup"><span data-stu-id="9ff8c-108">Order</span></span>  
* <span data-ttu-id="9ff8c-109">Los-für-Los</span><span class="sxs-lookup"><span data-stu-id="9ff8c-109">Lot-for-Lot</span></span>  
  
<span data-ttu-id="9ff8c-110">Feste Bestellmenge und Höchstmenge, Richtlinien für die Bestandsplanung.</span><span class="sxs-lookup"><span data-stu-id="9ff8c-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span></span> <span data-ttu-id="9ff8c-111">Obwohl die Bestandsplanung eigentlich einfacher als das Ausgleichsverfahren ist, müssen diese Richtlinien gemeinsam mit dem schrittweisen Ausgleich der Nachverfolgung von Vorrat und Bedarf bestehen.</span><span class="sxs-lookup"><span data-stu-id="9ff8c-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span></span> <span data-ttu-id="9ff8c-112">Um die Integration zwischen den beiden zu steuern, und Einsehbarkeit in die beteiligte Planungslogik bereitzustellen, steuern strenge Prinzipien, wie Wiederbeschaffungsverfahren angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="9ff8c-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="9ff8c-113">In diesem Abschnitt</span><span class="sxs-lookup"><span data-stu-id="9ff8c-113">In This Section</span></span>  
[<span data-ttu-id="9ff8c-114">Designdetails: Die Rolle des Minimalbestands</span><span class="sxs-lookup"><span data-stu-id="9ff8c-114">Design Details: The Role of the Reorder Point</span></span>](design-details-the-role-of-the-reorder-point.md)  
[<span data-ttu-id="9ff8c-115">Designdetails: Überwachen der Ebene des voraussichtlichen Lagerbestands und des Minimalbestands</span><span class="sxs-lookup"><span data-stu-id="9ff8c-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[<span data-ttu-id="9ff8c-116">Designdetails: Die Rolle des Zeitrahmens</span><span class="sxs-lookup"><span data-stu-id="9ff8c-116">Design Details: The Role of the Time Bucket</span></span>](design-details-the-role-of-the-time-bucket.md)  
[<span data-ttu-id="9ff8c-117">Designdetails: Unter dem Überlauflevel bleiben</span><span class="sxs-lookup"><span data-stu-id="9ff8c-117">Design Details: Staying under the Overflow Level</span></span>](design-details-staying-under-the-overflow-level.md)  
[<span data-ttu-id="9ff8c-118">Designdetails: Umgang mit voraussichtlichem negativem Lagerbestand</span><span class="sxs-lookup"><span data-stu-id="9ff8c-118">Design Details: Handling Projected Negative Inventory</span></span>](design-details-handling-projected-negative-inventory.md)  
[<span data-ttu-id="9ff8c-119">Designdetails: Wiederbeschaffungsverfahren</span><span class="sxs-lookup"><span data-stu-id="9ff8c-119">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)  
  
## <a name="see-also"></a><span data-ttu-id="9ff8c-120">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9ff8c-120">See Also</span></span>  
<span data-ttu-id="9ff8c-121">[Designdetails: Planungsparameter](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="9ff8c-121">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="9ff8c-122">[Designdetails: Planungs-Zuordnungstabelle](design-details-planning-assignment-table.md) </span><span class="sxs-lookup"><span data-stu-id="9ff8c-122">[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md) </span></span>  
<span data-ttu-id="9ff8c-123">[Designdetails: Zentrale Konzepte des Planungssystems](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="9ff8c-123">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
<span data-ttu-id="9ff8c-124">[Designdetails: Ausgleich von Bedarf und Vorrat](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="9ff8c-124">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
[<span data-ttu-id="9ff8c-125">Designdetails: Vorratsplanung</span><span class="sxs-lookup"><span data-stu-id="9ff8c-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)