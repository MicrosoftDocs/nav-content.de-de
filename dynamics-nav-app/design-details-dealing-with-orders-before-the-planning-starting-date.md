---
title: "Designdetails – Umgang mit Aufträgen vor dem Planungs-Startdatum"
description: "In diesem Thema werden die Regeln beschrieben, die Planung für Aufträge in der fixierten Zone anwendet."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: planning, frozen, design serial, lot
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: be20503b92b92448eceb1f388649d9f4022836ca
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-dealing-with-orders-before-the-planning-starting-date"></a><span data-ttu-id="64179-103">Designdetails: Umgang mit Aufträgen vor dem Planungs-Startdatum</span><span class="sxs-lookup"><span data-stu-id="64179-103">Design Details: Dealing with Orders Before the Planning Starting Date</span></span>
<span data-ttu-id="64179-104">Um zu vermeiden, dass ein Beschaffungsplan unmöglichen und daher unbrauchbare Vorschläge anzeigt, berücksichtigt das Planungssystem die Periode bis zum Startdatum als fixierte Zone, für die nichts geplant wird.</span><span class="sxs-lookup"><span data-stu-id="64179-104">To avoid that a supply plan shows impossible and therefore useless suggestions, the planning system regards the period up until the planning starting date a frozen zone where nothing is planned for.</span></span> <span data-ttu-id="64179-105">Die folgende Regel gilt für die fixierte Zone:</span><span class="sxs-lookup"><span data-stu-id="64179-105">The following rule applies to the frozen zone:</span></span>  
  
<span data-ttu-id="64179-106">Alle Vorräte und Bedarfe vor dem Startdatum der Planungsperiode gelten als Teil des Lagerbestands oder als geliefert.</span><span class="sxs-lookup"><span data-stu-id="64179-106">All supply and demand before the starting date of the planning period will be considered a part of inventory or shipped.</span></span>  
  
<span data-ttu-id="64179-107">Entsprechend schlägt das Planungssystem, mit wenigen Ausnahmen, keine Änderungen an Beschaffungsaufträgen in der fixierten Zone vor, und keine Auftragsnachverfolgungsverknüpfungen werden für diese Periode erstellt oder gespeichert.</span><span class="sxs-lookup"><span data-stu-id="64179-107">Accordingly, the planning system will not, with a few exceptions, suggest any changes to supply orders in the frozen zone, and no order tracking links are created or maintained for that period.</span></span>  
  
<span data-ttu-id="64179-108">Die Ausnahmen dieser Regel sind die folgenden:</span><span class="sxs-lookup"><span data-stu-id="64179-108">The exceptions to this rule are as follows:</span></span>  
  
* <span data-ttu-id="64179-109">Wenn der voraussichtlich verfügbare Lagerbestand, einschließlich die Summe von Bedarf und Vorrat in der fixierten Zone, geringer als Null ist.</span><span class="sxs-lookup"><span data-stu-id="64179-109">If the projected available inventory, including the sum of supply and demand in the frozen zone, is below zero.</span></span>  
* <span data-ttu-id="64179-110">Wenn Serien-/Chargennummern auf den zurückdatierten Aufträgen erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="64179-110">If serial/lot numbers are required on the backdated order(s).</span></span>  
* <span data-ttu-id="64179-111">Wenn der Vorrat-Bedarf-Satz durch eine Auftrag-zu-Auftrag-Richtlinie verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="64179-111">If the supply-demand set is linked by an order-to-order policy.</span></span>  
  
<span data-ttu-id="64179-112">Wenn der anfänglich verfügbare Lagerbestand geringer als Null ist, schlägt das Planungssystem einen Notfallbeschaffungsauftrag am Tag vor der Planperiode vor, um die fehlende Menge zu decken.</span><span class="sxs-lookup"><span data-stu-id="64179-112">If the initial available inventory is below zero, the planning system suggests an emergency supply order on the day before the planning period to cover the missing quantity.</span></span> <span data-ttu-id="64179-113">Deshalb ist der voraussichtliche und der verfügbare Lagerbestand immer mindestens Null, wenn die Planung für die zukünftige Periode beginnt.</span><span class="sxs-lookup"><span data-stu-id="64179-113">Consequently, the projected and available inventory will always be at least zero when planning for the future period begins.</span></span> <span data-ttu-id="64179-114">Die Planungszeile für diesen Beschaffungsauftrag zeigt ein Notwarnsymbol an , und zusätzliche Informationen werden beim Lookup angezeigt.</span><span class="sxs-lookup"><span data-stu-id="64179-114">The planning line for this supply order will display an Emergency warning icon and additional information is provided upon lookup.</span></span>  
  
## <a name="seriallot-numbers-and-order-to-order-links-are-exempt-from-the-frozen-zone"></a><span data-ttu-id="64179-115">Serien-/Chargennummern und Auftrag-zu-Auftrag-Links sind von der fixierten Zone ausgenommen</span><span class="sxs-lookup"><span data-stu-id="64179-115">Serial/Lot Numbers and Order-to-Order Links are Exempt from the Frozen Zone</span></span>  
<span data-ttu-id="64179-116">Wenn Serien-/Chargennummern erforderlich sind, oder ein Auftrag-zu-Auftrag-Link vorhanden ist, beachtet das Planungssystem die fixierte Zone nicht und berücksichtigt solche Mengen, die vom dem Startdatum zurückdatiert sind und möglicherweise Korrekturmaßnahmen erfordern, wenn bedarf und Vorrat nicht synchronisiert sind.</span><span class="sxs-lookup"><span data-stu-id="64179-116">If serial/lot numbers are required or an order-to-order link exists, the planning system will disregard the frozen zone and incorporate such quantities that are back-dated from the starting date and potentially suggest corrective actions if demand and supply is not synchronized.</span></span> <span data-ttu-id="64179-117">Der Geschäftsgrund für dieses Prinzip ist, dass solche bestimmten bedarf-Vorrat-Sätze übereinstimmen müssen, um sicherzustellen, dass dieser bestimmte Bedarf erfüllt wird.</span><span class="sxs-lookup"><span data-stu-id="64179-117">The business reason for this principle is that such specific demand-supply sets must match to ensure that this specific demand is fulfilled.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="64179-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="64179-118">See Also</span></span>  
<span data-ttu-id="64179-119">[Designdetails: Ausgleich von Bedarf und Vorrat](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="64179-119">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="64179-120">[Designdetails: Zentrale Konzepte des Planungssystems](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="64179-120">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="64179-121">Designdetails: Vorratsplanung</span><span class="sxs-lookup"><span data-stu-id="64179-121">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)