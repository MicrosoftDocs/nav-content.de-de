---
title: Inventurauftragszeilen mit Artikelverfolgungszeilen
description: "Artikelverfolgungszeilen werden verwendet, um Seriennummern und Chargennummern für Inventurauftragszeilen einzugeben."
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
ms.openlocfilehash: 31739940b4191d4105f646c4fab6b2bab8f03395
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="physical-inventory-order-lines-with-item-tracking-lines"></a><span data-ttu-id="2ea5a-103">Inventurauftragszeilen mit Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="2ea5a-103">Physical Inventory Order Lines With Item Tracking Lines</span></span>
<span data-ttu-id="2ea5a-104">Artikelverfolgungszeilen werden verwendet, um Seriennummern und Chargennummern für Inventurauftragszeilen einzugeben.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-104">Item tracking lines are used to enter serial nos. and lot nos. for physical inventory order lines.</span></span>  
  
 <span data-ttu-id="2ea5a-105">Die Anwendung berücksichtigt Artikelverfolgungszeilen nur dann, wenn das Kontrollkästchen  Verfolgungszeilen verwenden der Inventurauftragszeile aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-105">The program will obey the item tracking lines only if there is a check mark in the field Use Tracking Lines of the physical inventory order line.</span></span>  
  
 <span data-ttu-id="2ea5a-106">Diese Option wird je nach Einstellung für den Artikelverfolgungscode in der Artikeltabelle automatisch durch die Anwendung aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-106">The program places the checkmark automatically depending on the settings for the item tracking code from the item table.</span></span> <span data-ttu-id="2ea5a-107">Sie können das Kontrollkästchen auch manuell aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-107">You can also set or delete the check mark in the check box manually.</span></span> <span data-ttu-id="2ea5a-108">Eine Aktivierung ist jedoch nur dann möglich, wenn der Artikel in der aktuellen Inventurauftragszeile ausschließlich unter Verwendung von Seriennummern oder Chargennummern gebucht wurde.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-108">Placing a check mark here is only possible, if the item of the current physical inventory order line has been posted all the time using serial nos. or lot nos.</span></span>  
  
 <span data-ttu-id="2ea5a-109">Wenn dieses Kontrollkästchen aktiviert ist, können sich Verfolgungsinformationen an drei Stellen innerhalb der Anwendung befinden:</span><span class="sxs-lookup"><span data-stu-id="2ea5a-109">If there is a check mark in this check box the program uses 3 places, where tracking information can be found:</span></span>  
  
-   <span data-ttu-id="2ea5a-110">Erwartete Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="2ea5a-110">expected item tracking lines</span></span>  
  
-   <span data-ttu-id="2ea5a-111">Zählmengen mit Seriennummern und Chargennummern in der Inventurerfassungszeile</span><span class="sxs-lookup"><span data-stu-id="2ea5a-111">physical counts with serial nos. and lot nos. on the physical inventory recording line.</span></span>  
  
-   <span data-ttu-id="2ea5a-112">Zu buchende Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="2ea5a-112">item tracking lines to post.</span></span>  
  
 <span data-ttu-id="2ea5a-113">**Erwartete Verfolgungszeilen:**</span><span class="sxs-lookup"><span data-stu-id="2ea5a-113">**Expected Tracking Lines:**</span></span>  
  
 <span data-ttu-id="2ea5a-114">Wenn die Anwendung das Feld Erwartete Menge (Basis) in der Inventurauftragszeile berechnen soll, wird für den aktuellen Artikel auch eine Liste der Mengen mit Seriennummern und Chargennummern berechnet, die am Lager verfügbar sein sollten.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-114">If you have the program to calculate the field Qty. Expected (Base) on the physical inventory order line, the program also calculates a list for the current item containing quantities with serial nos. and lot nos. which should be available on stock.</span></span>  
  
 <span data-ttu-id="2ea5a-115">Das Programm ../../ umfasst die Berechnung aller Artikelposten, die bis zum Buchungsdatum des Inventurauftragskopfes gebucht worden sind und die in den 4 Feldern Artikelnr., Variantencode,  Lagerortcode und Lagerplatzcode in der Inventurauftragszeile die gleichen Werte aufweisen.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-115">The program ../../includes in the calculation all item ledger entries, which have been posted until the Posting Date of the inventory order header and which have the same values on the 4 fields Item No., Variant Code, Location Code and Bin Code on the physical inventory order line.</span></span>  
  
 <span data-ttu-id="2ea5a-116">Sie können die erwarteten Verfolgungszeilen für die aktuelle Inventurauftragszeile anzeigen.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-116">You can view the expected tracking lines for the current physical inventory order line.</span></span> <span data-ttu-id="2ea5a-117">Klicken Sie auf **Zeile**, **Artikelverfolgungszeilen**, **Erwartete Verfolgungszeilen**.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-117">Click **Line**, **Item Tracking Lines**, **Expected Tracking Lines**.</span></span> <span data-ttu-id="2ea5a-118">Das Fenster Erw. Inventurverfolg. Titelliste wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-118">The window Expect. Phys. Inv. Track. List opens.</span></span>  
  
 <span data-ttu-id="2ea5a-119">**Seriennummer/Chargennummer in der Inventurerfassungszeile:**</span><span class="sxs-lookup"><span data-stu-id="2ea5a-119">**Serial No./Lot No. On The Physical Inventory Recording Line:**</span></span>  
  
 <span data-ttu-id="2ea5a-120">Wenn bei der Inventurerfassung erfasste Mengen eingegeben wurden, können auch Seriennummern und Chargennummern eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-120">If you enter the recorded quantities on the physical inventory recording, you can enter serial nos./lot nos. to.</span></span> <span data-ttu-id="2ea5a-121">Nach Abschluss der Inventurerfassung weist die Anwendung die Inventurerfassungszeilen mit Seriennummern/Chargennummern Inventurauftragszeilen zu.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-121">When finishing the physical inventory recording, the program will assign the physical inventory recording lines with serial nos./ lot nos. to physical inventory order lines.</span></span>  
  
 <span data-ttu-id="2ea5a-122">Sie können die erwarteten Verfolgungszeilen für die aktuelle Inventurauftragszeile anzeigen.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-122">You can view the counted serial nos. and lot nos. for the current physical inventory order line.</span></span> <span data-ttu-id="2ea5a-123">Klicken Sie auf **Zeile**, **Erfassungszeilen**.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-123">Click **Line**, **Recording Lines**.</span></span> <span data-ttu-id="2ea5a-124">Das Fenster " Inventurerfassungszeilen. Erst. Die Erfassung von Zeilen wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-124">The window Phys. Invt. Recording Lines opens.</span></span>  
  
 <span data-ttu-id="2ea5a-125">**Zu buchende Artikelverfolgungszeilen:**</span><span class="sxs-lookup"><span data-stu-id="2ea5a-125">**Item Tracking Lines To Post:**</span></span>  
  
 <span data-ttu-id="2ea5a-126">Beim Abschluss des Inventurauftrags vergleicht die Anwendung die erwartete Menge und die erfasste (gezählte) Menge und berechnet die Abweichung.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-126">When finishing the physical inventory order, the program compares the expected quantity and the recorded (counted) quantity and calculates the difference.</span></span> <span data-ttu-id="2ea5a-127">Beim Abschluss des Inventurauftrags vergleicht die Anwendung die erwartete Menge und die erfasste (gezählte) Menge und berechnet die Abweichung. Wenn die Anwendung auch Artikelverfolgungszeilen berücksichtigen soll (das Kontrollkästchen  Verfolgungszeilen verwenden der Inventurerfassungszeile ist aktiviert), berechnet die Anwendung auch die Differenzen zwischen erwarteten Seriennummern und Chargennummern und erfassten Seriennummern und Chargennummern. Die Liste der berechneten Differenzen wird von der Anwendung beim Buchen des Inventurauftrags verwendet.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-127">If you have the program also to obey item tracking lines (by placing a check mark on the field Use Tracking Lines of the physical inventory order line), the program also calculates the differences between the expected serial nos. and lot nos. and the recorded serial nos. and lot nos. The list of the calculated differences will be used by the program when posting the physical inventory order.</span></span>  
  
 <span data-ttu-id="2ea5a-128">Sie können die erwarteten Verfolgungselemente für die aktuelle Inventurauftragszeile anzeigen.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-128">You can view the item tracking lines to post for the current physical inventory order line.</span></span> <span data-ttu-id="2ea5a-129">Klicken Sie auf **Zeile**, **Artikelverfolgungszeilen**, **Erwartete Verfolgungszeilen Differenzen**.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-129">Click **Line**, **Item Tracking Lines**, **All Diff. Tracking Lines**.</span></span> <span data-ttu-id="2ea5a-130">Das Fenster **Erw. Inventurverfolg. Titelliste** wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-130">The window **Phys. Invt. Item Track. List** opens.</span></span>  
  
 <span data-ttu-id="2ea5a-131">Weitere Informationen finden Sie unter [Beispiel - Inventurauftragszeile mit Nachverfolgungszeilen](example-inventory-order-line-with-tracking-lines.md).</span><span class="sxs-lookup"><span data-stu-id="2ea5a-131">For more information, see [Example - Inventory Order Line with Tracking Lines](example-inventory-order-line-with-tracking-lines.md).</span></span>  
  
 <span data-ttu-id="2ea5a-132">Wenn der Bericht Inventurauftr.-Diff.-Übersicht für die Inventurauftragszeilen gedruckt wird, können Sie bei Bedarf ebenfalls die Artikelverfolgungszeilen ausgeben lassen.</span><span class="sxs-lookup"><span data-stu-id="2ea5a-132">You can have the program to print the item tracking lines optional when printing the report Phys. Invt. Order Diff. List for the inventory order lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2ea5a-133">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2ea5a-133">See Also</span></span>  
 <span data-ttu-id="2ea5a-134">[Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="2ea5a-134">[How to: Enter Physical Inventory Orders](how-to-enter-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="2ea5a-135">[Gewusst wie: Berechnen der verfügbaren Menge für einen Inventurauftrag](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md) </span><span class="sxs-lookup"><span data-stu-id="2ea5a-135">[How to: Calculate Quantity On Hand for a Physical Inventory Order](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md) </span></span>  
 <span data-ttu-id="2ea5a-136">[Inventurerfassung – Inventurzählung](physical-inventory-recording-counting-physical-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="2ea5a-136">[Physical Inventory Recording - Counting Physical Inventory](physical-inventory-recording-counting-physical-inventory.md) </span></span>  
 <span data-ttu-id="2ea5a-137">[Gewusst wie: So schließen Sie eine Inventurerfassung ab](how-to-finish-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="2ea5a-137">[How to: Finish a Physical Inventory Recording](how-to-finish-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="2ea5a-138">[Gewusst wie: Einen Inventurauftrag abschließen](how-to-finish-a-physical-inventory-order.md) </span><span class="sxs-lookup"><span data-stu-id="2ea5a-138">[How to: Finish a Physical Inventory Order](how-to-finish-a-physical-inventory-order.md) </span></span>  
 [<span data-ttu-id="2ea5a-139">Gewusst wie: Analysieren von Inventurdifferenzen</span><span class="sxs-lookup"><span data-stu-id="2ea5a-139">How to: Analyze Physical Inventory Differences</span></span>](how-to-analyze-physical-inventory-differences.md)
