---
title: Vorgehensweise beim Korrigieren von MwSt.-Berichten
description: "Wenn Sie einen Korrektur-MwSt-Bericht übermitteln müssen oder einen übermittelten MwSt-Bericht löschen müssen, müssen Sie einen neuen MwSt-Bericht erstellen. Entsprechend der Gesetzgebung muss ein Korrekturbericht innerhalb eines Monats nach dem ursprünglichen Bericht übermittelt werden."
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
ms.openlocfilehash: f8c15e675019565e1caa2ad095000fb75f5b982b
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-correct-vat-reports"></a><span data-ttu-id="b283f-104">Gewusst wie: Korrigieren von MwSt-Berichten</span><span class="sxs-lookup"><span data-stu-id="b283f-104">How to: Correct VAT Reports</span></span>
<span data-ttu-id="b283f-105">Wenn Sie einen Korrektur-MwSt-Bericht übermitteln müssen oder einen übermittelten MwSt-Bericht löschen müssen, müssen Sie einen neuen MwSt-Bericht erstellen.</span><span class="sxs-lookup"><span data-stu-id="b283f-105">If you have to submit a corrective VAT report or delete a submitted VAT report, you must create a new VAT report.</span></span> <span data-ttu-id="b283f-106">Entsprechend der Gesetzgebung muss ein Korrekturbericht innerhalb eines Monats nach dem ursprünglichen Bericht übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="b283f-106">According to the legislation, a corrective report must be submitted within a month of the initial report.</span></span>  
  
 <span data-ttu-id="b283f-107">Wenn Sie einen Korrekturbericht erstellen, enthält die Erklärung zwei Zeilenarten pro korrigierter Zeile.</span><span class="sxs-lookup"><span data-stu-id="b283f-107">When you create a corrective report, the report will contain two line types per corrected line.</span></span> <span data-ttu-id="b283f-108">In einer Zeilenart, „Stornierung”, wird der Basiswert der MwSt. als Stornierung aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="b283f-108">In one line type, Cancellation, the base value of the VAT is reported as a cancellation.</span></span> <span data-ttu-id="b283f-109">Alle anderen Informationen bleiben dieselben und können nicht bearbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="b283f-109">All other information remains the same, and cannot be edited.</span></span> <span data-ttu-id="b283f-110">In einer neuen Zeile, Korrekturtyp, können Sie nach Bedarf Korrekturen am MwSt.-Betrag vornehmen.</span><span class="sxs-lookup"><span data-stu-id="b283f-110">On a new line, Correction type, you can make corrections as needed to the VAT amount.</span></span> <span data-ttu-id="b283f-111">Bei der Aktion **Zeilen vorschlagen** wird jedoch der richtige Betrag, basierend auf den Filtern und gebuchten Belegen, vorgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="b283f-111">The **Suggest Lines** action, however, will suggest the correct amount based on the filters and posted documents.</span></span> <span data-ttu-id="b283f-112">Sie können die **USt-IdNr.** nicht korrigieren oder ändern. Jede Periode, die korrigiert wird, benötigt ihren eigenen Korrekturbericht.</span><span class="sxs-lookup"><span data-stu-id="b283f-112">You cannot correct or modify the **VAT Registration No.** Each period being corrected needs its own corrective report.</span></span>  
  
 <span data-ttu-id="b283f-113">Bei der Aktion **Zeilen vorschlagen**, werden die zu meldenden Werte neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="b283f-113">The **Suggest Lines** action recalculates the values to report.</span></span> <span data-ttu-id="b283f-114">Die Aktion **Zeilen korrigieren** wird verwendet, um manuelle Änderungen vorzunehmen.</span><span class="sxs-lookup"><span data-stu-id="b283f-114">The **Correct Lines** action is used to make manual changes.</span></span> <span data-ttu-id="b283f-115">Sie können die Auswirkungen der zwei Aktionen kombinieren, um den Bericht zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="b283f-115">You can combine the effects of the two actions to correct your report.</span></span>  
  
 <span data-ttu-id="b283f-116">**Beispielkorrekturszenarien**</span><span class="sxs-lookup"><span data-stu-id="b283f-116">**Example corrections scenarios**</span></span>  
  
1.  <span data-ttu-id="b283f-117">Wenn Sie zusätzliche MwSt-Posten buchen, nachdem Sie den Standardbericht im Berichtszeitraum übermitteln, wählen Sie **Zeilen vorschlagen** in der Gruppe **Verarbeiten** aus, um die aktualisierten Beträge zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="b283f-117">If you post additional VAT entries after you submit the Standard report in the report period, choose **Suggest Lines** in the **Process** group to get the updated amounts.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="b283f-118">Wenn Sie den Betrag für einen Debitor oder Keditor manuell geändert haben, wird dieser Betrag überschrieben, wenn zusätzliche MwSt-Posten gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="b283f-118">If you manually changed the amount for a customer or vendor, this amount will be overwritten when additional VAT entries are posted.</span></span> <span data-ttu-id="b283f-119">Aktualisieren Sie den Betrag entsprechend.</span><span class="sxs-lookup"><span data-stu-id="b283f-119">Update the amount accordingly.</span></span>  
  
2.  <span data-ttu-id="b283f-120">Wenn Sie den Betrag einer Berichtszeile ändern möchten, die bereits übermittelt wurde und keine neuen MwSt-Posten gebucht werden, wählen Sie **Zeilen korrigieren** in der Gruppe **Verarbeiten** aus.</span><span class="sxs-lookup"><span data-stu-id="b283f-120">If you want to change the amount of a report line that has already been submitted and no new VAT entries are posted, choose **Correct Lines** in the **Process** group.</span></span> <span data-ttu-id="b283f-121">Das Fenster **MwSt-Berichtszeilen** wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="b283f-121">The **VAT Report Lines** window opens.</span></span> <span data-ttu-id="b283f-122">Wählen Sie die Zeilen aus, die Sie korrigieren möchten.</span><span class="sxs-lookup"><span data-stu-id="b283f-122">Select the lines that you want to correct.</span></span> <span data-ttu-id="b283f-123">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="b283f-123">Choose the **OK** button.</span></span>  
  
     <span data-ttu-id="b283f-124">Für jeden Posten werden zwei Zeilen angezeigt: Stornierung oder Korrektur.</span><span class="sxs-lookup"><span data-stu-id="b283f-124">For each entry, two lines are displayed: Cancellation and Correction.</span></span> <span data-ttu-id="b283f-125">Sie können jetzt den Betrag der Korrekturzeile ändern.</span><span class="sxs-lookup"><span data-stu-id="b283f-125">You can now change the amount on the Correction line.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="b283f-126">Die Aktion **Zeilen korrigieren** schlägt den Betrag nicht vor, der auf MwSt-Posten basiert.</span><span class="sxs-lookup"><span data-stu-id="b283f-126">The **Correct Lines** action will not suggest the amount based in VAT entries.</span></span> <span data-ttu-id="b283f-127">Wenn Sie neue MwSt-Posten für den Debitor oder Kreditor haben, verwenden Sie stattdessen **Zeilen vorschlagen**.</span><span class="sxs-lookup"><span data-stu-id="b283f-127">If you have new VAT entries for the customer or vendor, instead use **Suggest Lines**.</span></span>  
  
3.  <span data-ttu-id="b283f-128">Wenn Sie die falschen Filter verwendet haben, wie beispielsweise die falsche MwSt-Produktbuchungsgruppe, wählen Sie **Zeilen vorschlagen** in der Gruppe **Verarbeiten** aus, und legen Sie dann die Filter nach Bedarf fest.</span><span class="sxs-lookup"><span data-stu-id="b283f-128">If you used the wrong filters, for example, the wrong VAT Product Posting Group, choose **Suggest Lines** in the **Process** group and set the filters as needed.</span></span>  
  
     <span data-ttu-id="b283f-129">**Zeilen vorschlagen** erstellt Posten, um die Differenz zwischen den Filter zu widerzuspiegeln.</span><span class="sxs-lookup"><span data-stu-id="b283f-129">**Suggest Lines** will create entries to account for the difference between the filters.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="b283f-130">Wenn die aktualisierten Filter einen Debitor oder einen Kreditor ausschließen, erstellt [!INCLUDE[navnow](../../includes/navnow_md.md)] eine Stornierungszeile für den vorherigen berichteten Betrag und einen Korrekturposten mit Betrag 0.</span><span class="sxs-lookup"><span data-stu-id="b283f-130">If the updated filters exclude a customer or vendor, [!INCLUDE[navnow](../../includes/navnow_md.md)] creates a Cancellation line for the previous reported amount and a Correction entry with amount 0.</span></span>  
  
### <a name="to-correct-a-vat-report"></a><span data-ttu-id="b283f-131">So wird ein MwSt-Bericht korrigiert</span><span class="sxs-lookup"><span data-stu-id="b283f-131">To correct a VAT report</span></span>  
  
1.  <span data-ttu-id="b283f-132">Erstellen Sie einen neuen MwSt-Bericht.</span><span class="sxs-lookup"><span data-stu-id="b283f-132">Create a new VAT report.</span></span> <span data-ttu-id="b283f-133">Weitere Informationen finden Sie unter [Gewusst wie: MwSt-Berichte erstellen](how-to-create-vat-reports.md).</span><span class="sxs-lookup"><span data-stu-id="b283f-133">For more information, see [How to: Create VAT Reports](how-to-create-vat-reports.md).</span></span>  
  
2.  <span data-ttu-id="b283f-134">Füllen Sie die Felder im Inforegister **Allgemein** aus, und legen Sie das Feld **MwSt-Berichtstyp** auf „Korrigiert” fest.</span><span class="sxs-lookup"><span data-stu-id="b283f-134">Fill in the fields in the **General** FastTab, and set the **VAT Report Type** field to Corrective.</span></span>  
  
3.  <span data-ttu-id="b283f-135">In der **Originalberichtsnr.**</span><span class="sxs-lookup"><span data-stu-id="b283f-135">In the **Original Report No.**</span></span> <span data-ttu-id="b283f-136">Feld, wählen Sie den Bericht aus, die Sie korrigieren möchten.</span><span class="sxs-lookup"><span data-stu-id="b283f-136">field, select the report that you want to correct.</span></span> <span data-ttu-id="b283f-137">Sie können nur Berichte vom Typ „Standard” auswählen, die als „Übermittelt” markiert sind.</span><span class="sxs-lookup"><span data-stu-id="b283f-137">You can only select reports of type Standard that have been marked as Submitted.</span></span>  
  
4.  <span data-ttu-id="b283f-138">Erstellen Sie Ihre Korrektur-MwSt-Berichts-Zeilenposten.</span><span class="sxs-lookup"><span data-stu-id="b283f-138">Create your correction VAT Report Line entries.</span></span>  
  
     <span data-ttu-id="b283f-139">Wählen Sie auf der Registerkarte **Aktionen** die Option **Vorschlagszeilen** aus.</span><span class="sxs-lookup"><span data-stu-id="b283f-139">On the **Actions** tab, choose **Suggest Lines**.</span></span> <span data-ttu-id="b283f-140">Legen Sie die Filter gemäß Bedarf fest.</span><span class="sxs-lookup"><span data-stu-id="b283f-140">Set the filters as needed.</span></span>  
  
     <span data-ttu-id="b283f-141">In jeder Zeile können Sie einen Drilldown zu den Beträgen durchführen, um anzuzeigen, aus welchen MwSt-Posten sich der Betrag zusammensetzt.</span><span class="sxs-lookup"><span data-stu-id="b283f-141">On each line you can drill down on the amounts to see which VAT entries make up the amount.</span></span> <span data-ttu-id="b283f-142">Ändern Sie den Betrag nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="b283f-142">Change the amount if needed.</span></span> <span data-ttu-id="b283f-143">Sie können die **USt-IdNr.** jedoch nicht bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="b283f-143">You cannot edit, however, the **VAT Registration No.**.</span></span>  
  
5.  <span data-ttu-id="b283f-144">Wenn die **Vorschlagszeilen** Aktion nicht Vorschläge bietet, die Beträge zu korrigieren, die erforderlich, die **Zeilen korrigieren** Aktion verwenden, und Stornierungs- Korrekturzeilen für den Debitor oder Kreditor einzufügen.</span><span class="sxs-lookup"><span data-stu-id="b283f-144">If the **Suggest Lines** action does not provide suggestions to correct the amounts that you intended, use the **Correct Lines** action to insert Cancellation and Correction lines for the customer or vendor.</span></span>  
  
6.  <span data-ttu-id="b283f-145">Fahren Sie mit dem MwSt-Berichterstellungsprozess fort und geben Sie den Bericht frei.</span><span class="sxs-lookup"><span data-stu-id="b283f-145">Continue with the VAT report creation process, and release the report.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="b283f-146">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b283f-146">See Also</span></span>  
 [<span data-ttu-id="b283f-147">Vorgehensweise: Einrichten von MwSt.-Berichten</span><span class="sxs-lookup"><span data-stu-id="b283f-147">How to: Set Up VAT Reports</span></span>](how-to-set-up-vat-reports.md)
