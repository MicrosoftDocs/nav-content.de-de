---
title: "Gewusst wie: Einen Inventurauftrag abschließen"
description: "Nach Abschluss des Inventurauftrags können Sie die Inventurdifferenzen analysieren."
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
ms.openlocfilehash: acd7007597664c06786c18475e7c4177788880f9
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-finish-a-physical-inventory-order"></a><span data-ttu-id="13364-103">Gewusst wie: Einen Inventurauftrag abschließen</span><span class="sxs-lookup"><span data-stu-id="13364-103">How to: Finish a Physical Inventory Order</span></span>
<span data-ttu-id="13364-104">Nach Abschluss des Inventurauftrags können Sie die Inventurdifferenzen analysieren.</span><span class="sxs-lookup"><span data-stu-id="13364-104">After you have entered all data for the physical inventory order, you can finish the physical inventory order.</span></span>  
  
 <span data-ttu-id="13364-105">Ein Inventurauftrag kann nur abgeschlossen werden, wenn Folgendes zutrifft:</span><span class="sxs-lookup"><span data-stu-id="13364-105">It is only possible to finish the physical inventory order if the following is true:</span></span>  
  
-   <span data-ttu-id="13364-106">Alle zugehörigen Inventurerfassungen müssen den **Status** "Beendet" aufweisen.</span><span class="sxs-lookup"><span data-stu-id="13364-106">For all related physical inventory recordings, the Status field is set to **Finished**.</span></span>  
  
-   <span data-ttu-id="13364-107">In allen Inventurauftragszeilen wurde die erwartete Menge berechnet.</span><span class="sxs-lookup"><span data-stu-id="13364-107">In all physical inventory order lines, the quantity expected has been calculated.</span></span>  
  
     [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="13364-108">Die Anwendung kennzeichnet dies durch Aktivierung des Kontrollkästchens  In Erfassungszeilen enthalten für die jeweilige Inventurauftragszeile.</span><span class="sxs-lookup"><span data-stu-id="13364-108"> shows this by setting a check mark in the field Qty. Exp. Calculated of the physical inventory order line.</span></span>  
  
-   <span data-ttu-id="13364-109">Jede Inventurauftragszeile wurde mit mindestens einer Inventurerfassungszeile gezählt.</span><span class="sxs-lookup"><span data-stu-id="13364-109">Every physical inventory order line has been counted by at least one inventory recording line.</span></span>  
  
     <span data-ttu-id="13364-110">Dies wird angegeben, indem Sie im Feld Aufzeichnungs-Zeilen das Gebiet der Inventurauftragszeile auswählen.</span><span class="sxs-lookup"><span data-stu-id="13364-110">This is indicated by selecting the In Recording Lines field of the physical inventory order line.</span></span> <span data-ttu-id="13364-111">Für eine Inventurauftragszeile können Sie eine Liste der Inventurerfassungszeilen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="13364-111">For a physical inventory order line, you can view a list of the physical inventory recording lines.</span></span>  
  
### <a name="to-finish-a-physical-inventory-order"></a><span data-ttu-id="13364-112">So schließen Sie einen Inventurauftrag ab</span><span class="sxs-lookup"><span data-stu-id="13364-112">To finish a physical inventory order</span></span>  
  
1.  <span data-ttu-id="13364-113">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”"), geben Sie **Bestandsauftrag** ein, und wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="13364-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Phys. Inventory Order**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="13364-114">Öffnen Sie den Inventurauftrag, dessen Statistiken Sie anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="13364-114">Open the physical inventory order that you want to finish.</span></span>  
  
3.  <span data-ttu-id="13364-115">Wählen Sie auf der Registerkarte **Start** in der Gruppe **Funktionen** die Option **Beenden** aus.</span><span class="sxs-lookup"><span data-stu-id="13364-115">On the **Home** tab, in the **Functions** group, choose **Finish**.</span></span>  
  
     <span data-ttu-id="13364-116">Die Anwendung setzt den Status im Inventurauftragskopf auf **Beendet**.</span><span class="sxs-lookup"><span data-stu-id="13364-116">The status of the physical inventory header is set to **Finished**.</span></span> <span data-ttu-id="13364-117">Sie können den Inventurauftragskopf oder die Inventurauftragszeilen nun nicht mehr ändern.</span><span class="sxs-lookup"><span data-stu-id="13364-117">You can no longer change the physical inventory order header or the physical inventory order lines.</span></span>  
  
 <span data-ttu-id="13364-118">Beim Abschluss des Inventurauftrags vergleicht die Anwendung die erwartete Menge und die erfassten Mengen des Inventurauftragskopfes und berechnet die Abweichungen.</span><span class="sxs-lookup"><span data-stu-id="13364-118">When finishing the physical inventory order, the expected quantity and the recorded quantities of the physical inventory header are compared and the differences calculated.</span></span>  
  
 <span data-ttu-id="13364-119">Sie müssen den Status im Inventurauftragskopf erst auf "Beendet" setzen, bevor Sie Differenzen auswerten und den Inventurauftrag buchen können.</span><span class="sxs-lookup"><span data-stu-id="13364-119">You have to finish the physical inventory order header first before you can evaluate differences and before you can post the physical inventory order.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="13364-120">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="13364-120">See Also</span></span>  
 <span data-ttu-id="13364-121">[Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="13364-121">[How to: Enter Physical Inventory Orders](how-to-enter-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="13364-122">[Gewusst wie: Buchen von Inventuraufträgen](how-to-post-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="13364-122">[How to: Post Physical Inventory Orders](how-to-post-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="13364-123">[Gewusst wie: Berechnen der verfügbaren Menge für einen Inventurauftrag](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md) </span><span class="sxs-lookup"><span data-stu-id="13364-123">[How to: Calculate Quantity On Hand for a Physical Inventory Order](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md) </span></span>  
 <span data-ttu-id="13364-124">[Gewusst wie: So schließen Sie eine Inventurerfassung ab](how-to-finish-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="13364-124">[How to: Finish a Physical Inventory Recording](how-to-finish-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="13364-125">[Gewusst wie: Analysieren von Inventurdifferenzen](how-to-analyze-physical-inventory-differences.md) </span><span class="sxs-lookup"><span data-stu-id="13364-125">[How to: Analyze Physical Inventory Differences](how-to-analyze-physical-inventory-differences.md) </span></span>  
 [<span data-ttu-id="13364-126">Inventurauftragszeilen mit Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="13364-126">Physical Inventory Order Lines With Item Tracking Lines</span></span>](physical-inventory-order-lines-with-item-tracking-lines.md)
