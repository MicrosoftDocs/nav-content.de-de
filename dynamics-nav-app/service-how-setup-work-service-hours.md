---
title: 'Vorgehensweise: Einrichten von Arbeits- und Servicezeiten'
description: "Sie können die üblichen Arbeitszeiten in Ihrer Firma festlegen. Anhand von diesen Servicezeiten werden die Reaktionszeiten (Datum und Zeit) für Serviceaufträge und -angebote berechnet und Reaktionszeitwarnungen ausgegeben."
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
ms.openlocfilehash: 7b4d813f734fbaa53bc185e2477ca73705872097
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-work-hours-and-service-hours"></a><span data-ttu-id="d1e68-104">Vorgehensweise: Einrichten von Arbeits- und Servicezeiten</span><span class="sxs-lookup"><span data-stu-id="d1e68-104">How to: Set Up Work Hours and Service Hours</span></span>
<span data-ttu-id="d1e68-105">Normalerweise verfolgt ein Servicemanagementsystem Ressourcenstunden und den Serviceauftragsstatus, um die Arbeitsauslastung und Serviceanforderungen zu prognostizieren.</span><span class="sxs-lookup"><span data-stu-id="d1e68-105">Typically, a service management system tracks resource hours and service order status in order to forecast workloads and service needs.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="d1e68-106"> verfügt über integrierte Tools, die so angepasst werden können, dass diese Arten von Informationen erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="d1e68-106"> has built-in tools that you can customize to record this kind of information.</span></span>  
  
<span data-ttu-id="d1e68-107">Nach dem Festlegen der standardmäßigen Servicestunden des Unternehmens können Antwortzeiten für Serviceaufträge berechnet oder Warnhinweise gesendet werden, wenn Serviceanrufe eingehen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-107">After you set the default service hours of your company, you can calculate response times for service orders or send warnings or alerts when service calls come in.</span></span> <span data-ttu-id="d1e68-108">Die Warnfunktion wird in Verbindung mit dem Objektaufrufplaner implementiert.</span><span class="sxs-lookup"><span data-stu-id="d1e68-108">The alert feature is implemented together with the job scheduler.</span></span>   
  
<span data-ttu-id="d1e68-109">Da Sie an einem Serviceauftrag arbeiten, werden Sie den Status aktualisieren wollen, sodass Sie den Fortschritt überwachen können.</span><span class="sxs-lookup"><span data-stu-id="d1e68-109">As you work on a service order, you will want to update it's status so that you can monitor progress.</span></span> <span data-ttu-id="d1e68-110">Der Serviceauftragsstatus spiegelt den Reparaturstatus aller Serviceartikel des Serviceauftrags wider.</span><span class="sxs-lookup"><span data-stu-id="d1e68-110">The service order status reflects the repair status of all the service items in the service order.</span></span> <span data-ttu-id="d1e68-111">Weitere Informationen finden Sie unter [Serviceauftrag und Reparaturstatus verstehen](service-order-repair-status.md).</span><span class="sxs-lookup"><span data-stu-id="d1e68-111">For more information, see [Understanding Service Order and Repair Status](service-order-repair-status.md).</span></span> 

## <a name="to-set-up-default-service-hours"></a><span data-ttu-id="d1e68-112">So richten Sie Servicestandardzeiten ein</span><span class="sxs-lookup"><span data-stu-id="d1e68-112">To set up default service hours</span></span>  
<span data-ttu-id="d1e68-113">Verwenden Sie das Fenster **Standardservicezeiten**, um die üblichen Arbeitszeiten in Ihrer Firma festzulegen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-113">You use the **Default Service Hours** window to set up the usual service working hours in your company.</span></span> <span data-ttu-id="d1e68-114">Anhand von diesen Servicezeiten werden die Reaktionszeiten (Datum und Zeit) für Serviceaufträge und -angebote berechnet und Reaktionszeitwarnungen ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1e68-114">These service hours are used to calculate the response date and time for service orders and quotes and to send response time warnings.</span></span> <span data-ttu-id="d1e68-115">Wenn Sie keine vertragsspezifischen Servicezeiten in Verträgen einrichten, werden die Standardservicezeiten für den Servicevertrag verwendet.</span><span class="sxs-lookup"><span data-stu-id="d1e68-115">The default service hours are used for service contracts unless you specify special service hours for a contract.</span></span>  
  
1. <span data-ttu-id="d1e68-116">Wählen Sie in der rechten oberen Ecke ![Nach Seite oder Bericht suchen]das Symbol (media/ui-search/search_small.png "")Nach Seite oder Bericht suchen und geben **Standard-Servicestunden** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d1e68-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Default Service Hours**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d1e68-117">Füllen Sie die Felder je nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="d1e68-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!IMPORTANT]  
>  <span data-ttu-id="d1e68-118">Wenn Sie die Zeilen im Fenster **Standardservicezeiten** leer lassen, ist der Vorgabewert "24 Stunden" nur für Werktage gültig.</span><span class="sxs-lookup"><span data-stu-id="d1e68-118">If you leave the lines in the **Default Service Hours** window empty, the default value is 24 hours, valid only for calendar working days.</span></span>  
  
## <a name="to-set-up-work-hour-templates"></a><span data-ttu-id="d1e68-119">Um Arbeitszeitvorlagen einzurichten</span><span class="sxs-lookup"><span data-stu-id="d1e68-119">To set up work-hour templates</span></span>
<span data-ttu-id="d1e68-120">Sie können das Fenster **Arbeitszeitvorlagen** verwenden, um Vorlagen einzurichten, die die typischen Arbeitszeiten Ihrer Firma enthalten.</span><span class="sxs-lookup"><span data-stu-id="d1e68-120">You can use the **Work-Hour Template** window to set up templates that contain the typical working hours in your company.</span></span> <span data-ttu-id="d1e68-121">Sie können z. B. Vorlagen für Techniker in Vollzeit oder in Teilzeit einrichten.</span><span class="sxs-lookup"><span data-stu-id="d1e68-121">For example, you can create templates for full time technicians and part time technicians.</span></span> <span data-ttu-id="d1e68-122">Sie können Arbeitszeitvorlagen verwenden, wenn Sie Ressourcenkapazitäten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-122">You can use work-hour templates when you add capacity to resources.</span></span>  
  
1. <span data-ttu-id="d1e68-123">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Arbeitsstundenvorlage** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d1e68-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Hour Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d1e68-124">Füllen Sie die Felder je nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="d1e68-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!Note]
> <span data-ttu-id="d1e68-125">Nachdem Sie Arbeitsstunden für jeden Tag eingeben, wird der Wert im Feld **Stunden pro Woche** berechnet.</span><span class="sxs-lookup"><span data-stu-id="d1e68-125">After you enter work hours for each day, the value in the **Total per Week** field is calculated automatically.</span></span>  

## <a name="to-set-up-contract-specific-service-hours"></a><span data-ttu-id="d1e68-126">So richten Sie vertragsspezifische Servicezeiten ein</span><span class="sxs-lookup"><span data-stu-id="d1e68-126">To set up contract specific service hours</span></span>  
<span data-ttu-id="d1e68-127">Das Fenster **Servicezeiten** können Sie verwenden, um spezifische Servicezeiten für den Debitor dieser Serviceverträge einzurichten.</span><span class="sxs-lookup"><span data-stu-id="d1e68-127">You can use the **Service Hours** window to set up specific service hours for the customer that owns the service contract.</span></span> <span data-ttu-id="d1e68-128">Anhand von Servicezeiten werden die Reaktionszeiten (Datum und Zeit) für Serviceaufträge und -angebote berechnet, die zu dem Servicevertrag gehören.</span><span class="sxs-lookup"><span data-stu-id="d1e68-128">Service hours are used to calculate the response date and time for service orders and quotes that belong to the service contract.</span></span>  
  
<span data-ttu-id="d1e68-129">Wenn Sie keine vertragsspezifischen Servicezeiten in Verträgen einrichten, werden die Servicestandardzeiten für den Servicevertrag verwendet.</span><span class="sxs-lookup"><span data-stu-id="d1e68-129">If you do not set up specific service hours for the service contract, the default service hours for service contracts are used.</span></span>  
  
1. <span data-ttu-id="d1e68-130">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Servcievertrag** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d1e68-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contracts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d1e68-131">Öffnen Sie den relevanten  **Servicevertrag**, für den Sie bestimmte Servicezeiten einrichten möchten.</span><span class="sxs-lookup"><span data-stu-id="d1e68-131">Open the service contract you want to set up specific service hours for, and choose **Service Hours**.</span></span>  
4. <span data-ttu-id="d1e68-132">Um Servicezeiten basierend auf den Servicestandardzeiten einzurichten, wählen Sie die Aktion **Servicestandardzeiten kopieren**.</span><span class="sxs-lookup"><span data-stu-id="d1e68-132">To set up service hours based on default service hours, choose the **Copy Default Service Hours** action.</span></span>  
5. <span data-ttu-id="d1e68-133">Bearbeiten Sie die Felder in den Servicezeiteneinträgen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-133">Edit the fields in the service hours entries.</span></span> <span data-ttu-id="d1e68-134">Löschen Sie Einträge oder fügen Sie sie ein, um die Servicezeiten für den Vertrag einzurichten.</span><span class="sxs-lookup"><span data-stu-id="d1e68-134">Insert or delete entries to set up the service hours for the contract.</span></span> <span data-ttu-id="d1e68-135">Beachten Sie, dass die Felder **Tag**, **Startzeit** und **Endzeit** für jede Zeile ausgefüllt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-135">Note that the fields **Day**, **Starting Time** and **Ending Time** are required for each line.</span></span>  
6. <span data-ttu-id="d1e68-136">Wenn Sie möchten, dass die Servicezeiten ab einem bestimmten Datum gelten, müssen Sie das Feld **Startdatum** ausfüllen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-136">If you want the service hours to be valid from a specific date, fill in the **Starting Date** field.</span></span>  
7. <span data-ttu-id="d1e68-137">Wenn die Servicezeiten auch an Feiertagen gelten sollen, dann versehen Sie das Feld **An Feiertagen gültig** mit einem Häkchen.</span><span class="sxs-lookup"><span data-stu-id="d1e68-137">If you want the service hours to be valid on holidays, select the check box in the **Valid on Holidays** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d1e68-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d1e68-138">See Also</span></span>  
[<span data-ttu-id="d1e68-139">Zuordnungsstatus und Reparaturstatus</span><span class="sxs-lookup"><span data-stu-id="d1e68-139">Understanding Allocation Status and Repair Status</span></span>](service-allocation-status-and-repair-status.md)  
[<span data-ttu-id="d1e68-140">Einrichten der Serviceverwaltung</span><span class="sxs-lookup"><span data-stu-id="d1e68-140">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="d1e68-141">Serviceauftrags- und Reparaturstatus</span><span class="sxs-lookup"><span data-stu-id="d1e68-141">Understanding Service Order and Repair Status</span></span>](service-order-repair-status.md)  
