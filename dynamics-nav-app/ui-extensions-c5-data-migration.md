---
title: C5 -Datenmigrations-Erweiterung nutzen
description: Verwenden Sie diese Erweiterung, um Debitoren, Kreditoren, Artikel und Sachkonten von Microsoft Dynamics C5 2012 zu Dynamics NAV zu migrieren.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 09/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2307849566a44bb49a5db6965ec3056b1a39684b
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---

# <a name="the-c5-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="66e4a-103">Die C5-Datenmigrations-Erweiterung nutzen in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="66e4a-103">The C5 Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="66e4a-104">Verwenden Sie diese Erweiterung, um Debitoren, Kreditoren, Artikel und Sachkonten von Microsoft Dynamics C5 2012 zu [!INCLUDE[d365fin](includes/d365fin_md.md)] zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="66e4a-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> 

> [!Note] 
> <span data-ttu-id="66e4a-105">Der Mandant darf in [!INCLUDE[d365fin](includes/d365fin_md.md)] keine Daten in enthalten.</span><span class="sxs-lookup"><span data-stu-id="66e4a-105">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="66e4a-106">Nachdem Sie mit der Migration begonnen haben, erstellen Sie keine Debitoren, Kreditoren, Artikel oder Konten, bis die Migration beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="66e4a-106">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="66e4a-107">Um Daten zu migrieren</span><span class="sxs-lookup"><span data-stu-id="66e4a-107">To migrate data</span></span>
<span data-ttu-id="66e4a-108">Es gibt nur einige wenige Schritte, um die Daten aus C5 zu exportieren und sie in [!INCLUDE[d365fin](includes/d365fin_md.md)] zu importieren:</span><span class="sxs-lookup"><span data-stu-id="66e4a-108">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span> 

1. <span data-ttu-id="66e4a-109">In C5 verwenden Sie die Funktion **Datenbank exportieren**, um die Daten zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="66e4a-109">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="66e4a-110">Senden Sie dann den Exportordner an einen komprimierten (gezippten) Ordner.</span><span class="sxs-lookup"><span data-stu-id="66e4a-110">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="66e4a-111">Wählen Sie dann in [!INCLUDE[d365fin](includes/d365fin_md.md)] das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben Sie **Datenmigration** ein und wählen dann **Datenmigration**.</span><span class="sxs-lookup"><span data-stu-id="66e4a-111">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>
3. <span data-ttu-id="66e4a-112">Schliessen Sie die Schritte im unterstützten Setup ab.</span><span class="sxs-lookup"><span data-stu-id="66e4a-112">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="66e4a-113">Stellen Sie sicher, dass Sie**Importieren aus Microsoft Dynamcis C5 2012** als die Datenquelle auswählen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-113">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note] 
> <span data-ttu-id="66e4a-114">Mandanten fügen häufig Felder hinzu, um C5 für ihren jeweiligen Geschäftsbereich anzupassen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-114">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="66e4a-115"> migriert nicht Daten vom benutzerdefinierten Feldern.</span><span class="sxs-lookup"><span data-stu-id="66e4a-115"> does not migrate data from custom fields.</span></span> <span data-ttu-id="66e4a-116">Die Migration schlägt fehl, wenn Sie mehr als 10 benutzerdefinierte Felder haben.</span><span class="sxs-lookup"><span data-stu-id="66e4a-116">Also, migration will fail if you have more than 10 custom fields.</span></span> 

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="66e4a-117">Zeigt den Status der Datenmigration an</span><span class="sxs-lookup"><span data-stu-id="66e4a-117">Viewing the Status of the Migration</span></span>
<span data-ttu-id="66e4a-118">Verwenden Sie die Seite **Datenmigrations-Übersicht**, um den Erfolg der Migration zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-118">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="66e4a-119">Die Seite zeigt Informationen wie die Anzahl von Einheiten, die migriert wurde, den Status der Migration und die Anzahl von Artikeln an, die migriert wurden und ob sie erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="66e4a-119">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="66e4a-120">Sie zeigt auch die Anzahl von Fehlern, Sie können überprüfen, was schief ging und macht es wenn möglich einfach, zur Einheit zu gehen und das Problem zu lösen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-120">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="66e4a-121">Weitere Informationen finden Sie im nächsten Abschnitt dieses Themas.</span><span class="sxs-lookup"><span data-stu-id="66e4a-121">For more information, see the next section in this topic.</span></span> 

> [!Note] 
> <span data-ttu-id="66e4a-122">Während Sie auf die Ergebnisse der Migration warten, müssen Sie die Seite aktualisieren, um die Ergebnisse anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-122">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="correcting-errors"></a><span data-ttu-id="66e4a-123">Nachbesserung</span><span class="sxs-lookup"><span data-stu-id="66e4a-123">Correcting Errors</span></span>
<span data-ttu-id="66e4a-124">Falls etwas schief geht und ein Fehler auftritt, wird das **Status** Feld **Abgeschlossen mit Fehlern** angezeigt und das Feld **Fehlerzahl** zeigt an, wie viele es sind.</span><span class="sxs-lookup"><span data-stu-id="66e4a-124">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="66e4a-125">Um eine Liste der Fehler anzuzeigen, können Sie die Seite öffnen indem Sie **Datenmigrations-Fehler** auswählen:</span><span class="sxs-lookup"><span data-stu-id="66e4a-125">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>

* <span data-ttu-id="66e4a-126">Die Nummer im Feld **Fehlerzahl** für die Einheit.</span><span class="sxs-lookup"><span data-stu-id="66e4a-126">The number in the **Error Count** field for the entity.</span></span> 
* <span data-ttu-id="66e4a-127">Die Einheit und dann die Aktion **Fehler anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="66e4a-127">The entity, and then the **Show Errors** action.</span></span> 

<span data-ttu-id="66e4a-128">Um auf der Seite **Datenmigrations-Fehler** einen Fehler zu korrigieren, können Sie eine Fehlermeldung auswählen, und dann **Datensatz bearbeiten** auswählen, um die Seite zu öffnen, welche de Daten für die migrierte Einheit enthält.</span><span class="sxs-lookup"><span data-stu-id="66e4a-128">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="66e4a-129">Nachdem Sie eines oder mehrere Fehler korrigiert haben, können Sie **Migrieren von** wählen, um nur die Einheiten zu migrieren, die Sie korrigierten, ohne die Migration vollständig erneut durchführen zu müssen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-129">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="66e4a-130">Wenn Sie mehr als einen Fehler korrigiert haben, können Sie die Funktion **Weitere auswählen** verwenden, um mehrere Zeilen auszuwählen, um diese zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="66e4a-130">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="66e4a-131">Wenn es Fehler gibt, die nicht zur Korrektur wichtig sind, können Sie diese auswählen und dann **Auswahl überspringen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-131">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="66e4a-132">Wenn Sie Artikel haben, die in der Stückliste enthalten sind, müssen Sie diese mehrmals migrieren, wenn der ursprüngliche Artikel nicht vor den Varianten erstellt wird, auf die sie verweist.</span><span class="sxs-lookup"><span data-stu-id="66e4a-132">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="66e4a-133">Wenn eine Artikelvariante zuerst erzeugt wird, kann die Referenz zum ursprünglichen Artikel eine Fehlermeldung verursachen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-133">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="66e4a-134">Prüfen von Daten nach dem Migrieren</span><span class="sxs-lookup"><span data-stu-id="66e4a-134">Verifying Data After Migrating</span></span> 
<span data-ttu-id="66e4a-135">Wenn Sie sicherstellen möchten, dass Ihre Daten ordnungsgemäß migriert werden, können Sie die nächste Seiten in C5 und in [!INCLUDE[d365fin](includes/d365fin_md.md)]anzeigen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-135">If you want to verify that your data migrated correctly, you can look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="66e4a-136">Microsoft Dynamics C5 2012</span><span class="sxs-lookup"><span data-stu-id="66e4a-136">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]|
|-----|-----|
|<span data-ttu-id="66e4a-137">Debitoreneinträge</span><span class="sxs-lookup"><span data-stu-id="66e4a-137">Customer Entries</span></span>| <span data-ttu-id="66e4a-138">Fibu Buch.-Blätter</span><span class="sxs-lookup"><span data-stu-id="66e4a-138">General Journals</span></span>|
|<span data-ttu-id="66e4a-139">Kreditoreneinträge</span><span class="sxs-lookup"><span data-stu-id="66e4a-139">Vendor Entries</span></span>| <span data-ttu-id="66e4a-140">Fibu Buch.-Blätter</span><span class="sxs-lookup"><span data-stu-id="66e4a-140">General Journals</span></span>|
|<span data-ttu-id="66e4a-141">Artikelposten</span><span class="sxs-lookup"><span data-stu-id="66e4a-141">Item Entries</span></span>| <span data-ttu-id="66e4a-142">Artikel Buch.-Blätter</span><span class="sxs-lookup"><span data-stu-id="66e4a-142">Item Journals</span></span>|

<span data-ttu-id="66e4a-143">In [!INCLUDE[d365fin](includes/d365fin_md.md)], wird der Stapel für die migrierten Daten **C5MIGRATE** genannt.</span><span class="sxs-lookup"><span data-stu-id="66e4a-143">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span></span> 

> [!Note]
> <span data-ttu-id="66e4a-144">Denken Sie daran, dass wir nur offene Posten migrieren.</span><span class="sxs-lookup"><span data-stu-id="66e4a-144">Remember that we migrate only open entries.</span></span> <span data-ttu-id="66e4a-145">Sie finden keine historischen Daten.</span><span class="sxs-lookup"><span data-stu-id="66e4a-145">You will not find any historical data.</span></span>

## <a name="stopping-data-migration"></a><span data-ttu-id="66e4a-146">Datenmigration anhalten</span><span class="sxs-lookup"><span data-stu-id="66e4a-146">Stopping Data Migration</span></span>
<span data-ttu-id="66e4a-147">Sie können Datenmigration unterbrechen, indem Sie **Automatisches Beenden alle Migrationen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="66e4a-147">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="66e4a-148">Wenn Sie dies tun, werden alle offenen Migrationen beendet.</span><span class="sxs-lookup"><span data-stu-id="66e4a-148">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="66e4a-149">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="66e4a-149">See Also</span></span>
<span data-ttu-id="66e4a-150">[Anpassen [!INCLUDE[d365fin](includes/d365fin_md.md)] Erweiterungen nutzen](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="66e4a-150">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="66e4a-151">[Willkommen bei [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="66e4a-151">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  
