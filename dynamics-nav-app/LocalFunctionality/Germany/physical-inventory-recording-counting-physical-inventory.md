---
title: "Inventurerfassung – Inventurzählung"
description: "Nach dem Erstellen eines Inventurauftrags und nach der Eingabe der Inventurauftragszeilen kann die eigentliche Inventur durchgeführt werden. In diesem Zusammenhang können die Inventurerfassungsbelege verwendet werden."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 742bebfa7a2fabab87e643b57251db592945eda6
ms.contentlocale: de-de
ms.lasthandoff: 10/26/2017

---
# <a name="physical-inventory-recording---counting-physical-inventory"></a><span data-ttu-id="fd385-104">Inventurerfassung – Inventurzählung</span><span class="sxs-lookup"><span data-stu-id="fd385-104">Physical Inventory Recording - Counting Physical Inventory</span></span>
<span data-ttu-id="fd385-105">Nach dem Erstellen eines Inventurauftrags und nach der Eingabe der Inventurauftragszeilen kann die eigentliche Inventur durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="fd385-105">After you have created a physical inventory order and after you have entered the physical inventory order lines, you can take the physical inventory.</span></span> <span data-ttu-id="fd385-106">In diesem Zusammenhang können die Inventurerfassungsbelege verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="fd385-106">Therefore you can use the physical inventory recording documents.</span></span>  

<span data-ttu-id="fd385-107">Eine Inventurerfassung bezieht sich immer nur auf einen Inventurauftrag.</span><span class="sxs-lookup"><span data-stu-id="fd385-107">A physical inventory recording is related to only one physical inventory order.</span></span> <span data-ttu-id="fd385-108">Ein Inventurauftrag kann hingegen mit mehr als einer Inventurerfassung verknüpft sein.</span><span class="sxs-lookup"><span data-stu-id="fd385-108">A physical inventory order may have relations to more than one physical inventory recordings.</span></span>  

<span data-ttu-id="fd385-109">Jede Inventurerfassung setzt sich aus einem Inventurerfassungskopf und einer Reihe von Inventurerfassungszeilen zusammen.</span><span class="sxs-lookup"><span data-stu-id="fd385-109">A physical inventory recoding consists of a physical inventory recording header and a number of physical inventory recording lines.</span></span> <span data-ttu-id="fd385-110">Der Inventurerfassungskopf enthält die Informationen, die für alle Inventurerfassungszeilen gültig sind.</span><span class="sxs-lookup"><span data-stu-id="fd385-110">The physical inventory recording header contains the information, that are common for all physical inventory recording lines.</span></span>  

<span data-ttu-id="fd385-111">Die Zeilen enthalten die Artikel, die Lagerorte, die Lagerplätze und die erfassten Mengen.</span><span class="sxs-lookup"><span data-stu-id="fd385-111">This lines contain the items, locations, bins and the recorded quantities.</span></span>  

<span data-ttu-id="fd385-112">Diese können manuell oder von der Anwendung automatisch erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="fd385-112">You can create lines manually or you can have the program to create new physical inventory recordings automatically.</span></span> <span data-ttu-id="fd385-113">Es können Inventurerfassungslisten gedruckt werden.</span><span class="sxs-lookup"><span data-stu-id="fd385-113">You can print physical inventory recording lists.</span></span>  

<span data-ttu-id="fd385-114">Durch Festlegen des Status auf "Beendet" teilen Sie der Anwendung mit, dass die aktuelle Inventurerfassung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="fd385-114">By setting the Status to finished, you tell the program, that the current physical inventory recording has been finished.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fd385-115">Beim Abschluss der aktuellen Inventurerfassung weist die Anwendung jeder Inventurerfassungszeile eine Zeile des zugehörigen Inventurauftrags zu.</span><span class="sxs-lookup"><span data-stu-id="fd385-115">When you finish the current physical inventory recording, the program assigns every physical inventory recording line to one line of the related physical inventory order.</span></span> <span data-ttu-id="fd385-116">Die Anwendung weist jeweils Inventurauftragszeilen mit den gleichen Werten in den 4 Feldern  Artikelnr.,  Variantencode,  Lagerortcode und  Lagerplatzcode wie in der Inventurerfassungszeile zu.</span><span class="sxs-lookup"><span data-stu-id="fd385-116">The program assigns this physical inventory order lines with the same values in the 4 fields Item No., Variant Code, Location Code and Bin Code like in the physical inventory recording line.</span></span>  
>   
>  <span data-ttu-id="fd385-117">Wenn keine entsprechende Inventurauftragszeile vorhanden ist, fügt die Anwendung beim Abschluss der Inventurerfassung automatisch eine neue Zeile hinzu.</span><span class="sxs-lookup"><span data-stu-id="fd385-117">If there is no such physical inventory order line the program will automatically insert a new line when finishing the physical inventory recording.</span></span> <span data-ttu-id="fd385-118">Die Anwendung kennzeichnet diese Zeile durch Aktivierung des Kontrollkästchens Ohne Auftrag erfasst in der jeweiligen Inventurauftragszeile.</span><span class="sxs-lookup"><span data-stu-id="fd385-118">The program will note this by placing a check mark in the field Recorded without Order on the physical inventory order line.</span></span>  
>   
>  <span data-ttu-id="fd385-119">Ist mehr als eine entsprechende Inventurauftragszeile vorhanden, wird eine Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fd385-119">If there are more than one such physical inventory order lines, an error message appears.</span></span> <span data-ttu-id="fd385-120">In diesem Fall können Sie die Anwendung anweisen, die doppelten Zeilen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="fd385-120">You can have the program to show you the duplicate lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fd385-121">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fd385-121">See Also</span></span>  
 <span data-ttu-id="fd385-122">[So erstellen Sie eine physische Inventurerfassung](how-to-create-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="fd385-122">[How to: Create a Physical Inventory Recording](how-to-create-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="fd385-123">[Gewusst wie: So schließen Sie eine Inventurerfassung ab](how-to-finish-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="fd385-123">[How to: Finish a Physical Inventory Recording](how-to-finish-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="fd385-124">[So zeigen Sie doppelte Inventurauftragszeilen an](how-to-view-duplicate-physical-inventory-order-lines.md) </span><span class="sxs-lookup"><span data-stu-id="fd385-124">[How to: View Duplicate Physical Inventory Order Lines](how-to-view-duplicate-physical-inventory-order-lines.md) </span></span>  
 [<span data-ttu-id="fd385-125">Inventurauftragszeilen mit Artikelverfolgungszeilen</span><span class="sxs-lookup"><span data-stu-id="fd385-125">Physical Inventory Order Lines With Item Tracking Lines</span></span>](physical-inventory-order-lines-with-item-tracking-lines.md)

