---
title: Inventurbelege
description: "Sie können mithilfe der Inventurauftrags- und Inventurerfassungsbelege eine Inventur der Artikel durchführen."
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
ms.openlocfilehash: bff2b7e77c3e086ea8f46b0138554070db6a0ca5
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="physical-inventory-documents"></a><span data-ttu-id="411b8-103">Inventurbelege</span><span class="sxs-lookup"><span data-stu-id="411b8-103">Physical Inventory Documents</span></span>
<span data-ttu-id="411b8-104">Sie können mithilfe der Inventurauftrags- und Inventurerfassungsbelege eine Inventur der Artikel durchführen.</span><span class="sxs-lookup"><span data-stu-id="411b8-104">You can take inventory of your items using the physical inventory order and the physical inventory recording documents.</span></span>  
  
 <span data-ttu-id="411b8-105">Der Inventurauftrag enthält Daten für die Planung, Umsetzung und Analyse von Inventuren.</span><span class="sxs-lookup"><span data-stu-id="411b8-105">The physical inventory order contains data for planning, realizing, and analyzing physical inventory.</span></span> <span data-ttu-id="411b8-106">Artikel-, Lagerort- und Lagerplatzinformationen sind ebenfalls verfügbar.</span><span class="sxs-lookup"><span data-stu-id="411b8-106">The item, location, and bin information are also available.</span></span>  
  
## <a name="physical-inventory-recording"></a><span data-ttu-id="411b8-107">Inventurerfassung</span><span class="sxs-lookup"><span data-stu-id="411b8-107">Physical Inventory Recording</span></span>  
 <span data-ttu-id="411b8-108">Die Inventurerfassung enthält die Artikelnamen und -mengen, die bei der Inventur gezählt wurden.</span><span class="sxs-lookup"><span data-stu-id="411b8-108">The physical inventory recording contains the item names and quantities counted while taking physical inventory.</span></span> <span data-ttu-id="411b8-109">Ein Artikel kann in mehreren Inventurerfassungen gezählt werden.</span><span class="sxs-lookup"><span data-stu-id="411b8-109">An item may be counted in more than one physical inventory recording.</span></span>  
  
 <span data-ttu-id="411b8-110">Ein Inventurauftrag kann sich auf mehr als eine Inventurerfassung beziehen, doch eine Inventurerfassung kann sich nur auf einen Inventurauftrag beziehen.</span><span class="sxs-lookup"><span data-stu-id="411b8-110">A physical inventory order can be related to more than one physical inventory recording, but a physical inventory recording can be related to only one physical inventory order.</span></span> <span data-ttu-id="411b8-111">Weitere Informationen finden Sie unter [Vorgehensweise: Inventurhäufigkeiten für physische Lagererfassung einrichten](physical-inventory-recording-counting-physical-inventory.md)</span><span class="sxs-lookup"><span data-stu-id="411b8-111">For more information, see [Physical Inventory Recording - Counting Physical Inventory](physical-inventory-recording-counting-physical-inventory.md).</span></span>  
  
 <span data-ttu-id="411b8-112">Nach Abschluss der Inventurerfassungen und des Inventurauftrags kann der Inventurauftrag gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="411b8-112">After completing the physical inventory recordings and the physical inventory order, you can post the physical inventory order.</span></span> <span data-ttu-id="411b8-113">Die Informationen werden an das Inventur-Buch.-Blatt übertragen.</span><span class="sxs-lookup"><span data-stu-id="411b8-113">The information is transferred to the physical inventory journal.</span></span> <span data-ttu-id="411b8-114">Nach der Übertragung ist der Inventurauftrag als gebuchter Inventurauftrag zum späteren Abrufen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="411b8-114">After this transfer, the physical inventory order will be available as a posted physical inventory order for future retrieval.</span></span>  
  
## <a name="posted-physical-inventory-documents"></a><span data-ttu-id="411b8-115">Gebuchte physische Inventurbelege</span><span class="sxs-lookup"><span data-stu-id="411b8-115">Posted Physical Inventory Documents</span></span>  
 <span data-ttu-id="411b8-116">Nach dem Buchen wird der Inventurauftrag gelöscht, und der Beleg kann als gebuchter Inventurauftrag angezeigt und ausgewertet werden.</span><span class="sxs-lookup"><span data-stu-id="411b8-116">After posting the physical inventory order will be deleted and you can view and evaluate the document as posted physical inventory order.</span></span>  
  
 <span data-ttu-id="411b8-117">Beim Buchen von Inventuraufträgen werden auch die Inventurerfassungsköpfe und die Inventurerfassungszeilen in die gebuchten Belege übertragen.</span><span class="sxs-lookup"><span data-stu-id="411b8-117">When posting the physical inventory orders also physical inventory recording headers and physical inventory recording lines and physical inventory comment lines will be transferred to posted documents.</span></span>  
  
 <span data-ttu-id="411b8-118">Die gebuchten Inventurbelege bieten die Möglichkeit, einen vollständigen Überblick über den gesamten Inventurprozess zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="411b8-118">The posted inventory documents offer you the possibility to get a complete overview about the whole process of physical inventory.</span></span> <span data-ttu-id="411b8-119">Sie können die Daten von gebuchten Inventurauftragsköpfen und gebuchten Inventurauftragszeilen nicht ändern, da diese Belege bereits gebucht wurden.</span><span class="sxs-lookup"><span data-stu-id="411b8-119">You cannot change the data of posted physical inventory order headers and posted physical inventory order lines because the documents have been already posted.</span></span>  
  
 <span data-ttu-id="411b8-120">Wenn Sie Artikelverfolgungszeilen zum Registrieren von Seriennummern und Chargennummern verwendet haben, speichert die Anwendung die erwarteten Artikelverfolgungszeilen, die erfassten Artikelverfolgungszeilen und die gebuchten Artikelverfolgungsposten.</span><span class="sxs-lookup"><span data-stu-id="411b8-120">If you have used also item tracking lines to register serial nos. and lot nos. the program will save the expected item tracking lines, the recorded item tracking lines and the posted item tracking ledger entries.</span></span>  
  
 <span data-ttu-id="411b8-121">Es ist möglich, mithilfe der Kopierfunktion auf Basis des gebuchten Inventurauftrags neue Inventuraufträge zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="411b8-121">It is possible to use the posted physical inventory order to create new physical inventory orders using the copy function.</span></span>  
  
 <span data-ttu-id="411b8-122">Mit der Funktion "Navigate" können Inventurposten und andere zugehörige Posten eines gebuchten Inventurauftrags angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="411b8-122">You can use Navigate to view the inventory ledger entries and other related ledger entries for a posted physical inventory order.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="411b8-123">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="411b8-123">See Also</span></span>  
 <span data-ttu-id="411b8-124">[Info zu Logistik](about-warehouse-management.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-124">[About Warehouse Management](about-warehouse-management.md) </span></span>  
 <span data-ttu-id="411b8-125">[Inventurauftragszeilen mit Artikelverfolgungszeilen](physical-inventory-order-lines-with-item-tracking-lines.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-125">[Physical Inventory Order Lines With Item Tracking Lines](physical-inventory-order-lines-with-item-tracking-lines.md) </span></span>  
 <span data-ttu-id="411b8-126">[Inventurerfassung – Inventurzählung](physical-inventory-recording-counting-physical-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-126">[Physical Inventory Recording - Counting Physical Inventory](physical-inventory-recording-counting-physical-inventory.md) </span></span>  
 <span data-ttu-id="411b8-127">[Vorgehensweise: Einrichten von Inventurdokumenten](how-to-set-up-physical-inventory-documents.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-127">[How to: Set Up Physical Inventory Documents](how-to-set-up-physical-inventory-documents.md) </span></span>  
 <span data-ttu-id="411b8-128">[Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-128">[How to: Enter Physical Inventory Orders](how-to-enter-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="411b8-129">[So erstellen Sie eine physische Inventurerfassung](how-to-create-a-physical-inventory-recording.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-129">[How to: Create a Physical Inventory Recording](how-to-create-a-physical-inventory-recording.md) </span></span>  
 <span data-ttu-id="411b8-130">[Gewusst wie: Buchen von Inventuraufträgen](how-to-post-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-130">[How to: Post Physical Inventory Orders](how-to-post-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="411b8-131">Inventur Buch.-Blatt</span><span class="sxs-lookup"><span data-stu-id="411b8-131">Phys. Inventory Journal</span></span>   
 <span data-ttu-id="411b8-132">[Gewusst wie: Sperren der Lieferung bei negativem Lagerbestand](how-to-block-shipment-for-negative-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="411b8-132">[How to: Block Shipment for Negative Inventory](how-to-block-shipment-for-negative-inventory.md) </span></span>  
 [<span data-ttu-id="411b8-133">Lokale Funktion (Deutschland)</span><span class="sxs-lookup"><span data-stu-id="411b8-133">Germany Local Functionality</span></span>](germany-local-functionality.md)
