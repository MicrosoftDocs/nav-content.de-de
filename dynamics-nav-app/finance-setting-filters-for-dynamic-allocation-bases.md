---
title: "Setzen von Filtern für dynamische Zuteilungsgrundlagen"
description: "Die Methode der dynamischen Zuteilung basiert auf veränderbaren Werten. Zum Beispiel die Anzahl der Mitarbeiter in einer Kostenstelle oder die Artikel eines Kostenträgers, die in einem bestimmten Zeitraum verkauft wurden. Es gibt neun vordefinierte Zuteilungsgrundlagen und zwölf dynamische Datumsbereiche. Die verschiedenen Filter werden basierend auf der Zuteilungsgrundlage eingestellt."
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
ms.openlocfilehash: 8372f855cfaa19456ab597e163006ae20411defd
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="setting-filters-for-dynamic-allocation-bases"></a><span data-ttu-id="210d1-106">Setzen von Filtern für dynamische Zuteilungsgrundlagen</span><span class="sxs-lookup"><span data-stu-id="210d1-106">Setting Filters for Dynamic Allocation Bases</span></span>
<span data-ttu-id="210d1-107">Die Methode der dynamischen Zuteilung basiert auf veränderbaren Werten.</span><span class="sxs-lookup"><span data-stu-id="210d1-107">The dynamic allocation method is based on changeable values.</span></span> <span data-ttu-id="210d1-108">Zum Beispiel die Anzahl der Mitarbeiter in einer Kostenstelle oder die Artikel eines Kostenträgers, die in einem bestimmten Zeitraum verkauft wurden.</span><span class="sxs-lookup"><span data-stu-id="210d1-108">For example, the number of employees in a cost center or the items sold of a cost object in a specific time period.</span></span> <span data-ttu-id="210d1-109">Es gibt neun vordefinierte Zuteilungsgrundlagen und zwölf dynamische Datumsbereiche.</span><span class="sxs-lookup"><span data-stu-id="210d1-109">There are nine pre-defined allocation bases and twelve dynamic date ranges.</span></span> <span data-ttu-id="210d1-110">Die verschiedenen Filter werden basierend auf der Zuteilungsgrundlage eingestellt.</span><span class="sxs-lookup"><span data-stu-id="210d1-110">You set different filters based on the allocation base.</span></span>  

## <a name="setting-filters-for-dynamic-allocation-bases"></a><span data-ttu-id="210d1-111">Setzen von Filtern für dynamische Zuteilungsgrundlagen</span><span class="sxs-lookup"><span data-stu-id="210d1-111">Setting Filters for Dynamic Allocation Bases</span></span>  
 <span data-ttu-id="210d1-112">Die nachstehende Tabelle zeigt, welche Filter für verschiedene Zuteilungsgrundlagen möglich sind und welche Werte in den Feldern **Filter-Nr.** und **Gruppenfilter** gültig sind.</span><span class="sxs-lookup"><span data-stu-id="210d1-112">The following table shows which filters are possible for different allocation bases and which values are valid in the **No. Filter** and **Group Filter** fields.</span></span> <span data-ttu-id="210d1-113">Drücken Sie F1 im Feld **Datenfiltercode**, um detaillierte Beschreibungen zu lesen.</span><span class="sxs-lookup"><span data-stu-id="210d1-113">Press F1 in the **Date Filter Code** field to read detailed descriptions.</span></span>  

|<span data-ttu-id="210d1-114">**Bemessungsgrundlage**</span><span class="sxs-lookup"><span data-stu-id="210d1-114">**Base**</span></span>|<span data-ttu-id="210d1-115">**Nr. Filter**</span><span class="sxs-lookup"><span data-stu-id="210d1-115">**No. Filter**</span></span>|<span data-ttu-id="210d1-116">**Datumsfiltercode**</span><span class="sxs-lookup"><span data-stu-id="210d1-116">**Date Filter Code**</span></span>|<span data-ttu-id="210d1-117">**Kostenstellenfilter**</span><span class="sxs-lookup"><span data-stu-id="210d1-117">**Cost Center Filter**</span></span>|<span data-ttu-id="210d1-118">**Kostenträgerfilter**</span><span class="sxs-lookup"><span data-stu-id="210d1-118">**Cost Object Filter**</span></span>|<span data-ttu-id="210d1-119">**Gruppenfilter**</span><span class="sxs-lookup"><span data-stu-id="210d1-119">**Group Filter**</span></span>|  
|--------------|----------------------------------------|----------------------------------------------|------------------------------------------------|------------------------------------------------|------------------------------------------|  
|<span data-ttu-id="210d1-120">Sachposten</span><span class="sxs-lookup"><span data-stu-id="210d1-120">G/L Entries</span></span>|<span data-ttu-id="210d1-121">Sachkonto</span><span class="sxs-lookup"><span data-stu-id="210d1-121">G/L Account</span></span>|<span data-ttu-id="210d1-122">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-122">Yes</span></span>|<span data-ttu-id="210d1-123">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-123">Yes</span></span>|<span data-ttu-id="210d1-124">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-124">Yes</span></span>|<span data-ttu-id="210d1-125">N/Z</span><span class="sxs-lookup"><span data-stu-id="210d1-125">N/A</span></span>|  
|<span data-ttu-id="210d1-126">Finanzbudgetposten</span><span class="sxs-lookup"><span data-stu-id="210d1-126">G/L Budget Entries</span></span>|<span data-ttu-id="210d1-127">Sachkonto</span><span class="sxs-lookup"><span data-stu-id="210d1-127">G/L Account</span></span>|<span data-ttu-id="210d1-128">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-128">Yes</span></span>|<span data-ttu-id="210d1-129">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-129">Yes</span></span>|<span data-ttu-id="210d1-130">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-130">Yes</span></span>|<span data-ttu-id="210d1-131">Finanzbudgetname</span><span class="sxs-lookup"><span data-stu-id="210d1-131">G/L Budget Name</span></span>|  
|<span data-ttu-id="210d1-132">Kostenartposten</span><span class="sxs-lookup"><span data-stu-id="210d1-132">Cost Type Entries</span></span>|<span data-ttu-id="210d1-133">Einstandspreisberechnung</span><span class="sxs-lookup"><span data-stu-id="210d1-133">Cost Type</span></span>|<span data-ttu-id="210d1-134">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-134">Yes</span></span>|<span data-ttu-id="210d1-135">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-135">Yes</span></span>|<span data-ttu-id="210d1-136">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-136">Yes</span></span>|<span data-ttu-id="210d1-137">N/Z</span><span class="sxs-lookup"><span data-stu-id="210d1-137">N/A</span></span>|  
|<span data-ttu-id="210d1-138">Kostenbudgetposten</span><span class="sxs-lookup"><span data-stu-id="210d1-138">Cost Budget Entries</span></span>|<span data-ttu-id="210d1-139">Einstandspreisberechnung</span><span class="sxs-lookup"><span data-stu-id="210d1-139">Cost Type</span></span>|<span data-ttu-id="210d1-140">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-140">Yes</span></span>|<span data-ttu-id="210d1-141">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-141">Yes</span></span>|<span data-ttu-id="210d1-142">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-142">Yes</span></span>|<span data-ttu-id="210d1-143">Budgetname</span><span class="sxs-lookup"><span data-stu-id="210d1-143">Budget Name</span></span>|  
|<span data-ttu-id="210d1-144">Anzahl Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="210d1-144">No of Employees</span></span>|<span data-ttu-id="210d1-145">N/Z</span><span class="sxs-lookup"><span data-stu-id="210d1-145">N/A</span></span>|<span data-ttu-id="210d1-146">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-146">Yes</span></span>|<span data-ttu-id="210d1-147">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-147">Yes</span></span>|<span data-ttu-id="210d1-148">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-148">Yes</span></span>|<span data-ttu-id="210d1-149">N/Z</span><span class="sxs-lookup"><span data-stu-id="210d1-149">N/A</span></span>|  
|<span data-ttu-id="210d1-150">Verkaufte Artikel (Menge)</span><span class="sxs-lookup"><span data-stu-id="210d1-150">Items Sold (Qty)</span></span>|<span data-ttu-id="210d1-151">Artikelnr.</span><span class="sxs-lookup"><span data-stu-id="210d1-151">Item No.</span></span>|<span data-ttu-id="210d1-152">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-152">Yes</span></span>|<span data-ttu-id="210d1-153">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-153">Yes</span></span>|<span data-ttu-id="210d1-154">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-154">Yes</span></span>|<span data-ttu-id="210d1-155">Lagerbuchungsgruppe</span><span class="sxs-lookup"><span data-stu-id="210d1-155">Inventory Posting Group</span></span>|  
|<span data-ttu-id="210d1-156">Erworbene Artikel (Menge)</span><span class="sxs-lookup"><span data-stu-id="210d1-156">Items Purchased (Qty)</span></span>|<span data-ttu-id="210d1-157">Artikelnr.</span><span class="sxs-lookup"><span data-stu-id="210d1-157">Item No.</span></span>|<span data-ttu-id="210d1-158">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-158">Yes</span></span>|<span data-ttu-id="210d1-159">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-159">Yes</span></span>|<span data-ttu-id="210d1-160">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-160">Yes</span></span>|<span data-ttu-id="210d1-161">Lagerbuchungsgruppe</span><span class="sxs-lookup"><span data-stu-id="210d1-161">Inventory Posting Group</span></span>|  
|<span data-ttu-id="210d1-162">Verkaufte Artikel (Betrag)</span><span class="sxs-lookup"><span data-stu-id="210d1-162">Items Sold (Amount)</span></span>|<span data-ttu-id="210d1-163">Artikelnr.</span><span class="sxs-lookup"><span data-stu-id="210d1-163">Item No.</span></span>|<span data-ttu-id="210d1-164">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-164">Yes</span></span>|<span data-ttu-id="210d1-165">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-165">Yes</span></span>|<span data-ttu-id="210d1-166">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-166">Yes</span></span>|<span data-ttu-id="210d1-167">Lagerbuchungsgruppe</span><span class="sxs-lookup"><span data-stu-id="210d1-167">Inventory Posting Group</span></span>|  
|<span data-ttu-id="210d1-168">Erworbene Artikel (Betrag)</span><span class="sxs-lookup"><span data-stu-id="210d1-168">Items Purchased (Amount)</span></span>|<span data-ttu-id="210d1-169">Artikelnummer</span><span class="sxs-lookup"><span data-stu-id="210d1-169">Item No.</span></span>|<span data-ttu-id="210d1-170">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-170">Yes</span></span>|<span data-ttu-id="210d1-171">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-171">Yes</span></span>|<span data-ttu-id="210d1-172">Ja</span><span class="sxs-lookup"><span data-stu-id="210d1-172">Yes</span></span>|<span data-ttu-id="210d1-173">Lagerbuchungsgruppe</span><span class="sxs-lookup"><span data-stu-id="210d1-173">Inventory Posting Group</span></span>|  

## <a name="see-also"></a><span data-ttu-id="210d1-174">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="210d1-174">See Also</span></span>  
 <span data-ttu-id="210d1-175">[Szenario-Beispiel: Definieren von dynamischen Zuteilungen auf der Basis der verkauften Artikel](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span><span class="sxs-lookup"><span data-stu-id="210d1-175">[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span></span>  
 <span data-ttu-id="210d1-176">[Vorgehensweise: Einrichten von Zuteilungsquellen und -zielen](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="210d1-176">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 [<span data-ttu-id="210d1-177">Definieren und Zuweisen von Kosten</span><span class="sxs-lookup"><span data-stu-id="210d1-177">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)
