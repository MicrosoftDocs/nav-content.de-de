---
title: "Gewusst wie: So schließen Sie eine Inventurerfassung ab"
description: "Nachdem alle Daten einer Inventurerfassung vollständig eingegeben wurden, können Sie die Erfassung abschließen, indem Sie das Feld **Status** auf **Beendet** setzen."
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
ms.openlocfilehash: 781462c1eb758c14acbe47dd04f36d82646bf489
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-finish-a-physical-inventory-recording"></a><span data-ttu-id="2aeb1-103">Gewusst wie: So schließen Sie eine Inventurerfassung ab</span><span class="sxs-lookup"><span data-stu-id="2aeb1-103">How to: Finish a Physical Inventory Recording</span></span>
<span data-ttu-id="2aeb1-104">Nachdem alle Daten einer Inventurerfassung vollständig eingegeben wurden, können Sie die Erfassung abschließen, indem Sie das Feld **Status** auf **Beendet** setzen.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-104">After you have entered all data for a physical inventory recording, you can finish the recording by setting the **Status** field to **Finished**.</span></span>  
  
 <span data-ttu-id="2aeb1-105">Dies ist nur möglich, wenn das Kontrollkästchen **Erfasst** für alle Inventurerfassungszeilen der aktuellen Inventurerfassung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-105">You can only do this, if the **Recorded** field is selected for all physical inventory recording lines for the current physical inventory recording.</span></span>  
  
### <a name="to-finish-a-physical-inventory-recording"></a><span data-ttu-id="2aeb1-106">So schließen Sie eine Inventurerfassung ab</span><span class="sxs-lookup"><span data-stu-id="2aeb1-106">To finish a physical inventory recording</span></span>  
  
1.  <span data-ttu-id="2aeb1-107">Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Physische Inventurliste** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Phys. Inventory Recording List**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="2aeb1-108">Öffnen Sie den Inventurauftrag, dessen Statistiken Sie anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-108">Open the physical inventory recording that you want to finish.</span></span>  
  
3.  <span data-ttu-id="2aeb1-109">Wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **Beenden** aus.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-109">On the **Home** tab, in the **Process** group, choose **Finish**.</span></span>  
  
     <span data-ttu-id="2aeb1-110">Das Feld Status wird auf **Beendet** gesetzt.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-110">The status is set to **Finished**.</span></span> <span data-ttu-id="2aeb1-111">Sie können den Inventurerfassungskopf oder die Inventurerfassungszeilen nun nicht mehr ändern.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-111">You can no longer change the physical inventory header or the physical inventory lines.</span></span>  
  
 <span data-ttu-id="2aeb1-112">Beim Abschluss der aktuellen Inventurerfassung weist die Anwendung jeder Inventurerfassungszeile eine Zeile des zugehörigen Inventurauftrags zu.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-112">When you finish the current physical inventory recording, every physical inventory recording line is assigned to one line of the related physical inventory order.</span></span> <span data-ttu-id="2aeb1-113">Die Anwendung weist jeweils Inventurauftragszeilen mit den gleichen Werten in den 4 Feldern  **Artikelnr.**,  **Variantencode**, **Lagerortcode** und **Lagerplatzcode** wie in der Inventurerfassungszeile zu.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-113">The physical inventory order lines are assigned with the same values in the fields **Item No.**, **Variant Code**, **Location Code**, and **Bin Code** as the physical inventory recording line has.</span></span>  
  
 <span data-ttu-id="2aeb1-114">Wenn keine entsprechende Inventurauftragszeile vorhanden ist und wenn das Feld **Erfassung ohne Auftrag erlaubt** im Inventurerfassungskopf aktiviert ist, wird automatisch eine neue Zeile eingefügt und das **Ohne Auftrag erfasst** der Inventurauftragszeile aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-114">If no such physical inventory order line exists, and if the **Recording without order permit** field is selected on the physical inventory recording header, a new line is inserted automatically and the **Recorded without Order** field on the physical inventory order line is selected.</span></span> <span data-ttu-id="2aeb1-115">Andernfalls wird eine Fehlermeldung angezeigt, und der Prozess wird abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-115">Otherwise, an error message is displayed and the process is canceled.</span></span> <span data-ttu-id="2aeb1-116">Auch wenn es mehr als eine zugehörige Inventurauftragszeile gibt, wird eine Fehlermeldung angezeigt und die Verarbeitung gestoppt.</span><span class="sxs-lookup"><span data-stu-id="2aeb1-116">If there are more than one such physical inventory order lines, an error message is displayed and the process is canceled.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2aeb1-117">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2aeb1-117">See Also</span></span>  
 <span data-ttu-id="2aeb1-118">[So erstellen Sie eine physische Inventurerfassung](how-to-create-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="2aeb1-118">[How to: Create a Physical Inventory Recording](how-to-create-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="2aeb1-119">[So erstellen Sie eine physische Inventurerfassung](how-to-create-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="2aeb1-119">[How to: Create a Physical Inventory Recording](how-to-create-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="2aeb1-120">[So zeigen Sie doppelte Inventurauftragszeilen an](how-to-view-physical-inventory-order-lines.md) </span><span class="sxs-lookup"><span data-stu-id="2aeb1-120">[How to: View Duplicate Physical Inventory Order Lines](how-to-view-physical-inventory-order-lines.md) </span></span>  
 <span data-ttu-id="2aeb1-121">[Gewusst wie: Analysieren von Inventurdifferenzen](how-to-analyze-physical-inventory-differences.md) </span><span class="sxs-lookup"><span data-stu-id="2aeb1-121">[How to: Analyze Physical Inventory Differences](how-to-analyze-physical-inventory-differences.md) </span></span>  
 [<span data-ttu-id="2aeb1-122">Inventurauftragszeilen mit Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="2aeb1-122">Physical Inventory Order Lines With Item Tracking Lines</span></span>](physical-inventory-order-lines-with-item-tracking-lines.md)
