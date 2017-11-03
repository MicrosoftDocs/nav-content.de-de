---
title: "So geben Sie Dimensionen für den Inventurauftrag ein"
description: "Nachdem Sie einen Inventurauftrag erstellt haben, können Sie Dimensionen für diesen Auftrag eingeben."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 00dcae672bd8a6a1a305f483cc0ff288a8a2d2cc
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-enter-dimensions-for-physical-inventory-orders"></a><span data-ttu-id="e1e08-103">So geben Sie Dimensionen für den Inventurauftrag ein</span><span class="sxs-lookup"><span data-stu-id="e1e08-103">How to: Enter Dimensions for Physical Inventory Orders</span></span>
<span data-ttu-id="e1e08-104">Nachdem Sie einen Inventurauftrag erstellt haben, können Sie Dimensionen für diesen Auftrag eingeben.</span><span class="sxs-lookup"><span data-stu-id="e1e08-104">After you have created a physical inventory order, you can enter dimensions for this order.</span></span>  

<span data-ttu-id="e1e08-105">Die Anwendung unterscheidet zwischen Dimensionen für den Inventurauftragskopf und Dimensionen für die Inventurauftragszeilen.</span><span class="sxs-lookup"><span data-stu-id="e1e08-105">The application distinguishes between the dimensions for the physical inventory order header and the dimensions for the physical inventory order lines.</span></span> <span data-ttu-id="e1e08-106">Die Dimensionen für den Inventurauftragskopf sind ein Muster für die Dimensionen der Inventurauftragszeilen.</span><span class="sxs-lookup"><span data-stu-id="e1e08-106">The dimensions of the physical inventory header are a pattern for the dimensions of the physical inventory order lines.</span></span> <span data-ttu-id="e1e08-107">Jedes Mal, wenn (manuell oder automatisch) eine neue Inventurauftragszeile erstellt wird, überträgt [!INCLUDE[navnow](../../includes/navnow_md.md)] die Dimensionen aus dem Kopf in die neue Zeile.</span><span class="sxs-lookup"><span data-stu-id="e1e08-107">Every time you create a new physical inventory order line manually or automatically, [!INCLUDE[navnow](../../includes/navnow_md.md)] will transfer the dimensions from the header to the new line.</span></span>  

<span data-ttu-id="e1e08-108">Aus diesem Grund sollten die Inventurauftragszeilen erst erstellt werden, nachdem die Dimensionen für den Inventurauftragskopf vollständig eingegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="e1e08-108">That is why you should create the physical inventory order lines first after complete entering the dimensions for the physical inventory order header.</span></span> <span data-ttu-id="e1e08-109">Sie können die Dimensionen für jede Inventurauftragszeile manuell ändern.</span><span class="sxs-lookup"><span data-stu-id="e1e08-109">You can manually change the dimensions for every physical inventory order line.</span></span> <span data-ttu-id="e1e08-110">Zum Buchen verwendet [!INCLUDE[navnow](../../includes/navnow_md.md)] die Dimensionen der Inventurauftragszeile.</span><span class="sxs-lookup"><span data-stu-id="e1e08-110">For posting, [!INCLUDE[navnow](../../includes/navnow_md.md)] will use the dimensions of the physical inventory order line.</span></span>  

## <a name="to-enter-dimensions-for-a-physical-inventory-order"></a><span data-ttu-id="e1e08-111">So geben Sie Dimensionen für den Inventurauftrag ein</span><span class="sxs-lookup"><span data-stu-id="e1e08-111">To enter dimensions for a physical inventory order</span></span>  

1.  <span data-ttu-id="e1e08-112">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”"), geben Sie **Bestandsauftrag** ein, und wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="e1e08-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Phys. Inventory Order**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e1e08-113">Wählen Sie den Inventurauftrag aus, für den Sie eine Inventurerfassung erstellen möchten, klicken Sie auf Aktionen und anschließend auf **Bearbeiten**.</span><span class="sxs-lookup"><span data-stu-id="e1e08-113">Select the physical inventory order that you want to create an inventory recording for, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="e1e08-114">Wählen Sie die Aktion **Dimensionen** aus.</span><span class="sxs-lookup"><span data-stu-id="e1e08-114">Choose the **Dimensions** action.</span></span>  
4.  <span data-ttu-id="e1e08-115">Im Fenster **Dimensionssatzposten bearbeiten** geben Sie die Dimensionen im Inventurauftragskopf ein.</span><span class="sxs-lookup"><span data-stu-id="e1e08-115">In the **Edit Dimension Set Entries** window, enter the dimensions for the inventory order header.</span></span>  
5.  <span data-ttu-id="e1e08-116">Erstellen Sie eine neue Inventurauftragszeile, und geben Sie die Artikelnummer ein.</span><span class="sxs-lookup"><span data-stu-id="e1e08-116">Create a new physical inventory order line and enter the item number.</span></span>  
6.  <span data-ttu-id="e1e08-117">Wählen Sie die Aktion **Position** und dann die Aktion **Dimensionen**.</span><span class="sxs-lookup"><span data-stu-id="e1e08-117">Choose the **Line** action, and then choose the **Dimensions** action.</span></span>  
7.  <span data-ttu-id="e1e08-118">Im Fenster **Dimensionssatzposten bearbeiten** geben Sie die Dimensionen im Inventurauftragskopf ein.</span><span class="sxs-lookup"><span data-stu-id="e1e08-118">In the **Edit Dimension Set Entries** window, optionally, enter the dimensions for the inventory order line.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e1e08-119">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e1e08-119">See Also</span></span>  
 <span data-ttu-id="e1e08-120">[Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="e1e08-120">[How to: Enter Physical Inventory Orders](how-to-enter-physical-inventory-orders.md) </span></span>  
 <span data-ttu-id="e1e08-121">[Gewusst wie: Buchen von Inventuraufträgen](how-to-post-physical-inventory-orders.md) </span><span class="sxs-lookup"><span data-stu-id="e1e08-121">[How to: Post Physical Inventory Orders](how-to-post-physical-inventory-orders.md) </span></span>  
 [<span data-ttu-id="e1e08-122">Dimensionssatz-Eintrags-Übersicht</span><span class="sxs-lookup"><span data-stu-id="e1e08-122">Dimension Set Entries Overview</span></span>](../../design-details-dimension-set-entries-overview.md)

