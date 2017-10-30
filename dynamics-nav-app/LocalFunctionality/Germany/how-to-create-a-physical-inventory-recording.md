---
title: So erstellen Sie eine physische Inventurerfassung
description: "Nachdem Sie einen Inventurauftrag und die zugehörigen Zeilen erstellt haben, können Sie eine neue Inventurauftragserfassung für diese Inventur erstellen."
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
ms.openlocfilehash: c4e53ff7d6ad350720e3e577c9aa18f52c14ca33
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-a-physical-inventory-recording"></a><span data-ttu-id="deed1-103">So erstellen Sie eine physische Inventurerfassung</span><span class="sxs-lookup"><span data-stu-id="deed1-103">How to: Create a Physical Inventory Recording</span></span>
<span data-ttu-id="deed1-104">Nachdem Sie einen Inventurauftrag und die zugehörigen Zeilen erstellt haben, können Sie eine neue Inventurauftragserfassung für diese Inventur erstellen.</span><span class="sxs-lookup"><span data-stu-id="deed1-104">After you have created a physical inventory order and its lines you can create a new physical inventory recording for taking the inventory.</span></span>  
  
 <span data-ttu-id="deed1-105">Sie können manuell eine physische Inventurerfassung erstellen. Dies erweist sich ggf. als nützlich, wenn die Verwendung von Inventurlisten nicht erforderlich ist und/oder wenn die Lagerbestandsdaten mithilfe eines Scanners ermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="deed1-105">You can create a physical inventory recording manually if it is not necessary to use physical inventory lists or if the physical inventory data will be taken by a scanner.</span></span> <span data-ttu-id="deed1-106">Sie können eine Inventurerfassung auch dann manuell erstellen, wenn der zugehörige Inventurauftrag keine Zeilen aufweist.</span><span class="sxs-lookup"><span data-stu-id="deed1-106">You can also create a physical inventory recording manually even if the related physical recording order does not contain any line.</span></span> <span data-ttu-id="deed1-107">Nach Abschluss der Inventurerfassung erzeugt die Anwendung die erforderlichen Inventurauftragszeilen automatisch.</span><span class="sxs-lookup"><span data-stu-id="deed1-107">After finishing the physical inventory, the required physical inventory order lines are created automatically.</span></span> <span data-ttu-id="deed1-108">Dies kann beispielsweise bei permanenten Inventuren nützlich sein.</span><span class="sxs-lookup"><span data-stu-id="deed1-108">This may be useful, for instance, in the case of a permanent physical inventory.</span></span>  
  
 <span data-ttu-id="deed1-109">In den meisten Fällen verwenden Sie jedoch einen Batchauftrag, um Lagerbestand zu erfassen.</span><span class="sxs-lookup"><span data-stu-id="deed1-109">However, in most cases, you use a batch job to record inventory.</span></span> <span data-ttu-id="deed1-110">Basierend auf der Inventurerfassung können Sie eine Liste drucken, um die Inventur durchzuführen und die Ergebnisse zu notieren.</span><span class="sxs-lookup"><span data-stu-id="deed1-110">Based on the physical inventory recording, you can print a list for taking the inventory and writing the results down.</span></span> <span data-ttu-id="deed1-111">Anschließend können die Ergebnisse vom Papier in die Inventurerfassungszeilen übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="deed1-111">After that, you can transfer the results from paper to the physical inventory recording lines.</span></span>  
  
### <a name="to-create-a-physical-inventory-recording"></a><span data-ttu-id="deed1-112">So erstellen Sie eine Inventurerfassung</span><span class="sxs-lookup"><span data-stu-id="deed1-112">To create a physical inventory recording</span></span>  
  
1.  <span data-ttu-id="deed1-113">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”"), geben Sie **Bestandsauftrag** ein, und wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Phys. Inventory Order**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="deed1-114">Wählen Sie den Inventurauftrag aus, für den Sie eine Inventurerfassung erstellen möchten, klicken Sie auf **Startseite** und anschließend auf **Bearbeiten**.</span><span class="sxs-lookup"><span data-stu-id="deed1-114">Select the physical inventory order that you want to create an inventory recording for, and then, on the **Home** tab, choose **Edit**.</span></span>  
  
3.  <span data-ttu-id="deed1-115">Um eine Inventurerfassung, auf der Registerkarte **Startseite**, in der Gruppe **Verarbeiten** zu erstellen, wählen Sie **Neue Erfassung erstellen**.</span><span class="sxs-lookup"><span data-stu-id="deed1-115">To create a physical inventory recording, on the **Home** tab, in the **Process** group, choose **Make New Recording**.</span></span>  
  
4.  <span data-ttu-id="deed1-116">Füllen Sie im Fenster **Neue Inventurerfassung erst.** im Inforegister **Optionen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-116">In the **Make New Phys. Invt. Recording** window, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="deed1-117">Feld</span><span class="sxs-lookup"><span data-stu-id="deed1-117">Field</span></span>|<span data-ttu-id="deed1-118">Description</span><span class="sxs-lookup"><span data-stu-id="deed1-118">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="deed1-119">**Nur nicht erfasste Zeilen**</span><span class="sxs-lookup"><span data-stu-id="deed1-119">**Only Lines Not In Recordings**</span></span>|<span data-ttu-id="deed1-120">Wählen Sie diese Option aus, um nur dann eine neue Inventurerfassungszeile zu generieren, falls die Daten in keiner anderen Inventurerfassungszeile vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="deed1-120">Select to generate a new physical inventory recording line only if the data do not exist in any other physical inventory recording line.</span></span>|  
    |<span data-ttu-id="deed1-121">**Erfassung ohne Auftrag erlaubt**</span><span class="sxs-lookup"><span data-stu-id="deed1-121">**Recording Without Order Permit**</span></span>|<span data-ttu-id="deed1-122">Wählen Sie diese Option aus, um eine neue Inventurerfassungszeile zu generieren.</span><span class="sxs-lookup"><span data-stu-id="deed1-122">Select to generate a new physical inventory recording line.</span></span>|  
  
5.  <span data-ttu-id="deed1-123">Klicken Sie auf die Schaltfläche **OK**, um den Batchauftrag zu starten.</span><span class="sxs-lookup"><span data-stu-id="deed1-123">Choose the **OK** button to start the batch job.</span></span>  
  
6.  <span data-ttu-id="deed1-124">Wählen Sie auf der Registerkarte **Navigieren** die Option **Aufzeichnen** aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-124">On the **Navigate** tab, choose **Recordings**.</span></span> <span data-ttu-id="deed1-125">Das Fenster "Inventurerfassung" wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="deed1-125">The physical inventory recording window appears.</span></span> <span data-ttu-id="deed1-126">Wählen Sie die neu erstellte Inventurerfassung aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-126">Select the new created physical inventory recording.</span></span>  
  
     <span data-ttu-id="deed1-127">Sie können nun die Inventurliste basierend auf den Daten der aktuellen Inventurerfassung drucken.</span><span class="sxs-lookup"><span data-stu-id="deed1-127">You can now print a physical inventory list based on the data on the current physical inventory recording.</span></span>  
  
7.  <span data-ttu-id="deed1-128">Wählen Sie auf der Registerkarte **Bericht** wählen Sie **Inventurerfassung** aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-128">On the **Report** tab, choose **Physical Inventory Recording**.</span></span>  
  
8.  <span data-ttu-id="deed1-129">Im Fenster **Phys. Invt. Erfassung** legen Sie die entsprechenden Filter fest, und wählen Sie die Schaltfläche **Drucken** aus oder wählen Sie die Schaltfläche **Vorschau** aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-129">In the **Phys. Invt. Recording** window, set the appropriate filters, and then choose the **Print** button or choose the **Preview** button.</span></span>  
  
     <span data-ttu-id="deed1-130">Optional können Sie die Funktion Physische Stabelverarbeitungs-Inventur verwenden, um die Serien- oder Chargennummern zu erfassen.</span><span class="sxs-lookup"><span data-stu-id="deed1-130">Optionally, you can use the Copy Phys. Invt. Rec. Line batch job to record serial numbers or lot numbers.</span></span>  
  
9. <span data-ttu-id="deed1-131">Im Fenster **Physische Inventurerfassung** wählen Sie die Inventurerfassungszeile aus, wählen Sie **Funktionen** und dann **Zeile kopieren**.</span><span class="sxs-lookup"><span data-stu-id="deed1-131">In the **Phys. Inventory Recording** window, select the physical inventory recording line, choose **Functions**, and then choose **Copy Line**.</span></span>  
  
10. <span data-ttu-id="deed1-132">Im Fenster **Physische Inventurerfassung kopieren** geben Sie die Anzahl der Kopien an, die von der ausgewählten Zeile erstellt werden sollen, und wählen Sie dann die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-132">In the **Copy Phys. Invt. Rec. Line** window, specify the number of copies to make of the selected line, and then choose the **OK** button.</span></span>  
  
 <span data-ttu-id="deed1-133">Sie können die gedruckte physische Inventurerfassung verwenden, um die tatsächliche Menge des am angegebenen Lagerort verfügbaren Artikels zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="deed1-133">You can use the printed physical inventory recording to update the actual quantity of the item available in the specified location.</span></span> <span data-ttu-id="deed1-134">Zum Abschließen des Erfassungsprozesses muss das Kontrollkästchen **Erfasst** für alle Inventurerfassungszeilen aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="deed1-134">To complete the recording process, the **Recorded** check box must be selected for all physical inventory recording lines.</span></span>  
  
 <span data-ttu-id="deed1-135">Damit ersichtlich ist, dass die Inventurerfassung abgeschlossen wurde, muss der **Status** im Inventurerfassungskopf mithilfe der entsprechenden Funktion auf **Beendet** gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="deed1-135">To show that you have finished the physical inventory recording, you have to set the **Status** on the inventory recording header to **Finished**.</span></span> <span data-ttu-id="deed1-136">Weitere Informationen finden Sie unter [Vorgehensweise: Führen Sie physische Inventuren aus](how-to-finish-a-physical-inventory-recording.md).</span><span class="sxs-lookup"><span data-stu-id="deed1-136">For more information, see [How to: Finish a Physical Inventory Recording](how-to-finish-a-physical-inventory-recording.md).</span></span>  
  
### <a name="to-complete-a-physical-inventory-recording"></a><span data-ttu-id="deed1-137">So schließen Sie eine Inventurerfassung ab</span><span class="sxs-lookup"><span data-stu-id="deed1-137">To complete a physical inventory recording</span></span>  
  
1.  <span data-ttu-id="deed1-138">Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Physische Inventur durchführen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-138">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Phys. Inventory Recording**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="deed1-139">Wählen Sie den Inventurauftrag aus, für den Sie eine Inventurerfassung erstellen möchten, klicken Sie auf **Startseite** und anschließend auf **Bearbeiten**.</span><span class="sxs-lookup"><span data-stu-id="deed1-139">Select the physical inventory recording that you want to complete, and then, on the **Home** tab, choose **Edit**.</span></span>  
  
3.  <span data-ttu-id="deed1-140">Geben Sie im Fenster **Inventurerfassung** im Inforegister **Zeilen** im Feld **Menge** für jede Zeile die tatsächliche Artikelmenge ein.</span><span class="sxs-lookup"><span data-stu-id="deed1-140">In the **Phys. Invt. Recording** window, on the **Lines** FastTab, in the **Quantity** field for each line, enter the actual item quantity.</span></span>  
  
4.  <span data-ttu-id="deed1-141">Aktivieren Sie für jede Zeile das Kontrollkästchen **Erfasst**.</span><span class="sxs-lookup"><span data-stu-id="deed1-141">Select the **Recorded** check box for each line.</span></span>  
  
5.  <span data-ttu-id="deed1-142">Füllen Sie im Inforegister **Allgemein** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="deed1-142">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="deed1-143">Feld</span><span class="sxs-lookup"><span data-stu-id="deed1-143">Field</span></span>|<span data-ttu-id="deed1-144">Description</span><span class="sxs-lookup"><span data-stu-id="deed1-144">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="deed1-145">**Erfasst von**</span><span class="sxs-lookup"><span data-stu-id="deed1-145">**Person Recorded**</span></span>|<span data-ttu-id="deed1-146">Die Person, von der der Lagerbestand erfasst wurde.</span><span class="sxs-lookup"><span data-stu-id="deed1-146">The person who recorded the inventory.</span></span>|  
    |<span data-ttu-id="deed1-147">**Erfassungsdatum**</span><span class="sxs-lookup"><span data-stu-id="deed1-147">**Date Recorded**</span></span>|<span data-ttu-id="deed1-148">Das Datum, an dem die Inventur erfasst wurde.</span><span class="sxs-lookup"><span data-stu-id="deed1-148">The date on which the physical inventory was recorded.</span></span>|  
    |<span data-ttu-id="deed1-149">**Erfassungszeit**</span><span class="sxs-lookup"><span data-stu-id="deed1-149">**Time Recorded**</span></span>|<span data-ttu-id="deed1-150">Die Zeit, zu der die Inventur erfasst wurde.</span><span class="sxs-lookup"><span data-stu-id="deed1-150">The time at which the physical inventory was recorded.</span></span>|  
  
 <span data-ttu-id="deed1-151">Sie können die Inventur jetzt beenden.</span><span class="sxs-lookup"><span data-stu-id="deed1-151">You can now finish the physical inventory recording.</span></span> <span data-ttu-id="deed1-152">Weitere Informationen finden Sie unter [Vorgehensweise: Führen Sie physische Inventuren aus](how-to-finish-a-physical-inventory-recording.md).</span><span class="sxs-lookup"><span data-stu-id="deed1-152">For more information, see [How to: Finish a Physical Inventory Recording](how-to-finish-a-physical-inventory-recording.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="deed1-153">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="deed1-153">See Also</span></span>  
 <span data-ttu-id="deed1-154">[Inventurerfassung – Inventurzählung](physical-inventory-recording-counting-physical-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="deed1-154">[Physical Inventory Recording - Counting Physical Inventory](physical-inventory-recording-counting-physical-inventory.md) </span></span>  
 <span data-ttu-id="deed1-155">[Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="deed1-155">[How to: Enter Physical Inventory Orders](how-to-enter-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="deed1-156">[Gewusst wie: Berechnen der verfügbaren Menge für einen Inventurauftrag](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md) </span><span class="sxs-lookup"><span data-stu-id="deed1-156">[How to: Calculate Quantity On Hand for a Physical Inventory Order](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md) </span></span>  
 <span data-ttu-id="deed1-157">[Gewusst wie: So schließen Sie eine Inventurerfassung ab](how-to-finish-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="deed1-157">[How to: Finish a Physical Inventory Recording](how-to-finish-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="deed1-158">Neue Inventurerfassung erst.</span><span class="sxs-lookup"><span data-stu-id="deed1-158">Make New Phys. Invt. Recording</span></span>   
 <span data-ttu-id="deed1-159">Inventurerfassung</span><span class="sxs-lookup"><span data-stu-id="deed1-159">Phys. Invt. Recording</span></span>
