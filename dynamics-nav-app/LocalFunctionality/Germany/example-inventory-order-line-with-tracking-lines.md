---
title: Beispiel - Inventurauftragszeile mit Nachverfolgungszeilen
description: 'Eine Inventurauftragszeile muss die folgenden bestimmten Daten enthalten:'
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: b52e6dad09392033de229839dbd65ed87b46b4b9
ms.contentlocale: de-de
ms.lasthandoff: 12/01/2017

---
# <a name="example---inventory-order-line-with-tracking-lines"></a><span data-ttu-id="28ddb-103">Beispiel - Inventurauftragszeile mit Nachverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="28ddb-103">Example - Inventory Order Line with Tracking Lines</span></span>
<span data-ttu-id="28ddb-104">Eine Inventurauftragszeile enthält die folgenden buchungsrelevanten Daten:</span><span class="sxs-lookup"><span data-stu-id="28ddb-104">The physical inventory order line should contain the following data:</span></span>  

- <span data-ttu-id="28ddb-105">Artikelnr.: 80216-V</span><span class="sxs-lookup"><span data-stu-id="28ddb-105">Item No.: 80216-V</span></span>  
- <span data-ttu-id="28ddb-106">Lagerortcode: BLAU</span><span class="sxs-lookup"><span data-stu-id="28ddb-106">Location Code: BLUE</span></span>  
- <span data-ttu-id="28ddb-107">Die Felder "Variantencode" und "Lagerplatzcode" sind beide leer.</span><span class="sxs-lookup"><span data-stu-id="28ddb-107">The fields Variant Code and Bin Code may be blank.</span></span>  

<span data-ttu-id="28ddb-108">Das Kontrollkästchen Verfolgungszeilen verwenden der Inventurauftragszeile wurde aktiviert, und der Artikel 80216-V wird entsprechend seines Artikelverfolgungscodes stets unter Angabe der Chargennummern gebucht.</span><span class="sxs-lookup"><span data-stu-id="28ddb-108">There is a check mark in the field Use Tracking Lines on the physical inventory order line and the item 80216-V should be posted all time with lot nos. according to the item tracking code.</span></span>  

<span data-ttu-id="28ddb-109">Das Buchungsdatum des Inventurauftragskopfes ist der 31.12.2002.</span><span class="sxs-lookup"><span data-stu-id="28ddb-109">The posting date on the physical inventory order header should be 12/31/2002.</span></span>  

<span data-ttu-id="28ddb-110">Die erwartete Menge des Artikels 80216-V am Lagerort BLAU zum 31.12.2001 beträgt 120 Stück.</span><span class="sxs-lookup"><span data-stu-id="28ddb-110">The expected quantity of the item 80216-V at the location BLUE on 12/31/2001 should be 120 pieces.</span></span>  

<span data-ttu-id="28ddb-111">Der Lagerbestand setzt sich aus den folgenden Chargen zusammen:</span><span class="sxs-lookup"><span data-stu-id="28ddb-111">The quantity on stock consists of the following lots:</span></span>  

## <a name="the-expected-item-tracking-lines"></a><span data-ttu-id="28ddb-112">Die erwarteten Artikelverfolgungszeilen:</span><span class="sxs-lookup"><span data-stu-id="28ddb-112">The expected Item Tracking Lines:</span></span>  

|<span data-ttu-id="28ddb-113">**Chargennr.**</span><span class="sxs-lookup"><span data-stu-id="28ddb-113">**Lot No.**</span></span>|<span data-ttu-id="28ddb-114">**Menge**</span><span class="sxs-lookup"><span data-stu-id="28ddb-114">**Quantity**</span></span>|  
|-----------------|------------------|  
|<span data-ttu-id="28ddb-115">CH1001</span><span class="sxs-lookup"><span data-stu-id="28ddb-115">CH1001</span></span>|<span data-ttu-id="28ddb-116">80</span><span class="sxs-lookup"><span data-stu-id="28ddb-116">80</span></span>|  
|<span data-ttu-id="28ddb-117">CH1003</span><span class="sxs-lookup"><span data-stu-id="28ddb-117">CH1003</span></span>|<span data-ttu-id="28ddb-118">30</span><span class="sxs-lookup"><span data-stu-id="28ddb-118">30</span></span>|  
|<span data-ttu-id="28ddb-119">CH1006</span><span class="sxs-lookup"><span data-stu-id="28ddb-119">CH1006</span></span>|<span data-ttu-id="28ddb-120">10</span><span class="sxs-lookup"><span data-stu-id="28ddb-120">10</span></span>|  
|<span data-ttu-id="28ddb-121">**Summe**</span><span class="sxs-lookup"><span data-stu-id="28ddb-121">**Total**</span></span>|<span data-ttu-id="28ddb-122">**120**</span><span class="sxs-lookup"><span data-stu-id="28ddb-122">**120**</span></span>|  

<span data-ttu-id="28ddb-123">Es wurden folgende Inventurerfassungszeilen für Artikel 80216-V, Lagerortcode BLAU, erfasst:</span><span class="sxs-lookup"><span data-stu-id="28ddb-123">There had been recorded the following physical inventory recording lines for the item 80216-V, location code BLUE:</span></span>  

## <a name="recorded-lot-nos-on-the-physical-inventory-recording-lines"></a><span data-ttu-id="28ddb-124">Erfasste Chargennummern in den Inventurerfassungszeilen:</span><span class="sxs-lookup"><span data-stu-id="28ddb-124">Recorded Lot Nos. on the Physical Inventory Recording Lines:</span></span>  

|<span data-ttu-id="28ddb-125">**Chargennr.**</span><span class="sxs-lookup"><span data-stu-id="28ddb-125">**Lot No.**</span></span>|<span data-ttu-id="28ddb-126">**Menge**</span><span class="sxs-lookup"><span data-stu-id="28ddb-126">**Quantity**</span></span>|  
|-----------------|------------------|  
|<span data-ttu-id="28ddb-127">CH1001</span><span class="sxs-lookup"><span data-stu-id="28ddb-127">CH1001</span></span>|<span data-ttu-id="28ddb-128">80</span><span class="sxs-lookup"><span data-stu-id="28ddb-128">80</span></span>|  
|<span data-ttu-id="28ddb-129">CH1002</span><span class="sxs-lookup"><span data-stu-id="28ddb-129">CH1002</span></span>|<span data-ttu-id="28ddb-130">12</span><span class="sxs-lookup"><span data-stu-id="28ddb-130">12</span></span>|  
|<span data-ttu-id="28ddb-131">CH1003</span><span class="sxs-lookup"><span data-stu-id="28ddb-131">CH1003</span></span>|<span data-ttu-id="28ddb-132">20</span><span class="sxs-lookup"><span data-stu-id="28ddb-132">20</span></span>|  
|<span data-ttu-id="28ddb-133">**Summe**</span><span class="sxs-lookup"><span data-stu-id="28ddb-133">**Total**</span></span>|<span data-ttu-id="28ddb-134">**112**</span><span class="sxs-lookup"><span data-stu-id="28ddb-134">**112**</span></span>|  

<span data-ttu-id="28ddb-135">Bei Abschluss des Inventurauftrags berechnet die Anwendung für den Artikel 80216-V am Lagerort BLAU einen zu buchenden Abgang von 8 Stück und erstellt folgende Posten</span><span class="sxs-lookup"><span data-stu-id="28ddb-135">When finishing the physical inventory order the program will calculate for the item 80216-V at the location BLUE a negative adjustment of 8 pieces and will create the following entries:</span></span>  

## <a name="item-tracking-lines-to-post"></a><span data-ttu-id="28ddb-136">Zu buchende Artikelverfolgungszeilen:</span><span class="sxs-lookup"><span data-stu-id="28ddb-136">Item Tracking lines to post:</span></span>  

|<span data-ttu-id="28ddb-137">**Chargennr.**</span><span class="sxs-lookup"><span data-stu-id="28ddb-137">**Lot No.**</span></span>|<span data-ttu-id="28ddb-138">**Erwartete Menge**</span><span class="sxs-lookup"><span data-stu-id="28ddb-138">**Expected Quantity**</span></span>|<span data-ttu-id="28ddb-139">**Erfasste Menge**</span><span class="sxs-lookup"><span data-stu-id="28ddb-139">**Recorded Quantity**</span></span>|<span data-ttu-id="28ddb-140">**Zu buchende Menge**</span><span class="sxs-lookup"><span data-stu-id="28ddb-140">**Quantity to post**</span></span>|  
|-----------------|---------------------------|---------------------------|--------------------------|  
|<span data-ttu-id="28ddb-141">CH1001</span><span class="sxs-lookup"><span data-stu-id="28ddb-141">CH1001</span></span>|<span data-ttu-id="28ddb-142">80</span><span class="sxs-lookup"><span data-stu-id="28ddb-142">80</span></span>|<span data-ttu-id="28ddb-143">80</span><span class="sxs-lookup"><span data-stu-id="28ddb-143">80</span></span>|<span data-ttu-id="28ddb-144">0</span><span class="sxs-lookup"><span data-stu-id="28ddb-144">0</span></span>|  
|<span data-ttu-id="28ddb-145">CH1002</span><span class="sxs-lookup"><span data-stu-id="28ddb-145">CH1002</span></span>|<span data-ttu-id="28ddb-146">0</span><span class="sxs-lookup"><span data-stu-id="28ddb-146">0</span></span>|<span data-ttu-id="28ddb-147">12</span><span class="sxs-lookup"><span data-stu-id="28ddb-147">12</span></span>|<span data-ttu-id="28ddb-148">+12</span><span class="sxs-lookup"><span data-stu-id="28ddb-148">+ 12</span></span>|  
|<span data-ttu-id="28ddb-149">CH1003</span><span class="sxs-lookup"><span data-stu-id="28ddb-149">CH1003</span></span>|<span data-ttu-id="28ddb-150">30</span><span class="sxs-lookup"><span data-stu-id="28ddb-150">30</span></span>|<span data-ttu-id="28ddb-151">20</span><span class="sxs-lookup"><span data-stu-id="28ddb-151">20</span></span>|<span data-ttu-id="28ddb-152">-10</span><span class="sxs-lookup"><span data-stu-id="28ddb-152">- 10</span></span>|  
|<span data-ttu-id="28ddb-153">CH1006</span><span class="sxs-lookup"><span data-stu-id="28ddb-153">CH1006</span></span>|<span data-ttu-id="28ddb-154">10</span><span class="sxs-lookup"><span data-stu-id="28ddb-154">10</span></span>|<span data-ttu-id="28ddb-155">0</span><span class="sxs-lookup"><span data-stu-id="28ddb-155">0</span></span>|<span data-ttu-id="28ddb-156">-10</span><span class="sxs-lookup"><span data-stu-id="28ddb-156">- 10</span></span>|  
|<span data-ttu-id="28ddb-157">**Summe**</span><span class="sxs-lookup"><span data-stu-id="28ddb-157">**Total**</span></span>|<span data-ttu-id="28ddb-158">**120**</span><span class="sxs-lookup"><span data-stu-id="28ddb-158">**120**</span></span>|<span data-ttu-id="28ddb-159">**112**</span><span class="sxs-lookup"><span data-stu-id="28ddb-159">**112**</span></span>|<span data-ttu-id="28ddb-160">**-8**</span><span class="sxs-lookup"><span data-stu-id="28ddb-160">**- 8**</span></span>|  

## <a name="see-also"></a><span data-ttu-id="28ddb-161">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="28ddb-161">See Also</span></span>  
 [<span data-ttu-id="28ddb-162">Inventurauftragszeilen mit Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="28ddb-162">Physical Inventory Order Lines With Item Tracking Lines</span></span>](physical-inventory-order-lines-with-item-tracking-lines.md)  
 [<span data-ttu-id="28ddb-163">Vorgehensweise: Arbeiten mit Chargennummern und Seriennummern</span><span class="sxs-lookup"><span data-stu-id="28ddb-163">How to: Work with Serial and Lot Numbers</span></span>](../../inventory-how-work-item-tracking.md)

