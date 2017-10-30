---
title: 'Gewusst wie: Exportieren von GDPdU-Daten'
description: "Sie können Finanz- und Steuerdatenaten entsprechend dem Prozess für Datenzugriff und Testbarkeit von digitalen Dokumenten (GDPdU), der auf deutschen Steuergesetzen basiert, exportieren. Zudem können verschiedene Optionen in eine XML-Datei eingeschlossen werden."
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
ms.openlocfilehash: d329daf531ac7c3a0679e762b7aa3e6011ee2bd5
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-gdpdu-data"></a><span data-ttu-id="7badd-104">Gewusst wie: Exportieren von GDPdU-Daten</span><span class="sxs-lookup"><span data-stu-id="7badd-104">How to: Export GDPdU Data</span></span>
<span data-ttu-id="7badd-105">Sie können Finanz- und Steuerdatenaten entsprechend dem Prozess für Datenzugriff und Testbarkeit von digitalen Dokumenten (GDPdU), der auf deutschen Steuergesetzen basiert, exportieren.</span><span class="sxs-lookup"><span data-stu-id="7badd-105">You can export financial data and tax data according to the process for data access and testability of digital documents (GDPdU).</span></span> <span data-ttu-id="7badd-106">Zudem können verschiedene Optionen in eine XML-Datei eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="7badd-106">You can also select various options to be included in an XML file.</span></span>  
  
 <span data-ttu-id="7badd-107">Falls es keine Daten zum Exportieren gibt, erstellt [!INCLUDE[navnow](../../includes/navnow_md.md)] leere Dateien.</span><span class="sxs-lookup"><span data-stu-id="7badd-107">If there is no data to export, [!INCLUDE[navnow](../../includes/navnow_md.md)] creates empty files.</span></span>  
  
### <a name="to-export-gdpdu-data"></a><span data-ttu-id="7badd-108">So exportieren Sie GDPdU-Daten</span><span class="sxs-lookup"><span data-stu-id="7badd-108">To export GDPdU data</span></span>  
  
1.  <span data-ttu-id="7badd-109">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen")und geben **Geschäftsdaten exportieren** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="7badd-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export Business Data**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="7badd-110">Füllen Sie im Stapelverarbeitungsauftrag **GDPdU Export** im Inforegister **Optionen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="7badd-110">In the **GDPdU Export** window, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="7badd-111">ADD INCLUDE<!--[!INCLUDE[bp_tableoption](../../includes/bp_tabledescription_md.md)]--></span><span class="sxs-lookup"><span data-stu-id="7badd-111">ADD INCLUDE<!--[!INCLUDE[bp_tableoption](../../includes/bp_tabledescription_md.md)]--></span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="7badd-112">**Startdatum**</span><span class="sxs-lookup"><span data-stu-id="7badd-112">**Starting Date**</span></span>|<span data-ttu-id="7badd-113">Gibt das Startdatum des Berichts für den Datenexport an.</span><span class="sxs-lookup"><span data-stu-id="7badd-113">Specifies the start date for the data export.</span></span><br /><br /> <span data-ttu-id="7badd-114">**HINWEIS:** Wenn die Datenenexportquell- ../../includes- Periodenfelder, das Startdatum und dem Enddatum als Filterwert für die Periodenfelder verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="7badd-114">**NOTE:** If the data export source ../../includes period fields, the start date and the end date are used as filter values for the period fields.</span></span>|  
    |<span data-ttu-id="7badd-115">**Enddatum**</span><span class="sxs-lookup"><span data-stu-id="7badd-115">**Ending Date**</span></span>|<span data-ttu-id="7badd-116">Gibt das Enddatum des Berichts für den Datenexport an.</span><span class="sxs-lookup"><span data-stu-id="7badd-116">Specifies the end date for the data export.</span></span>|  
    |<span data-ttu-id="7badd-117">**Abschlussdatum einschließen**</span><span class="sxs-lookup"><span data-stu-id="7badd-117">**Include Closing Date**</span></span>|<span data-ttu-id="7badd-118">Gibt an, ob der Datenexport das Ultimodatum der Periode enthalten soll.</span><span class="sxs-lookup"><span data-stu-id="7badd-118">Specifies if the data export must include the closing date for the period.</span></span>|  
  
3.  <span data-ttu-id="7badd-119">Wählen Sie im Inforegister **Datenexport - Datensatzdefinition** die entsprechenden Filter aus, um den Datenexport zu identifizieren und Daten exportieren Datensatztyp.</span><span class="sxs-lookup"><span data-stu-id="7badd-119">On the **Data Export Record Definition** FastTab, select the appropriate filters to identify the data export and data export record type.</span></span> <span data-ttu-id="7badd-120">Weitere Informationen finden Sie unter [Prozess für Datenzugriff und zur Prüfbarkeit digitaler Unterlagen (GDPdU)](process-for-data-access-and-testability-of-digital-documents-gdpdu-.md)</span><span class="sxs-lookup"><span data-stu-id="7badd-120">For more information, see [Process for Data Access and Testability of Digital Documents (GDPdU)](process-for-data-access-and-testability-of-digital-documents-gdpdu-.md).</span></span>  
  
4.  <span data-ttu-id="7badd-121">Um Daten zu exportieren, wählen Sie die Schaltfläche **OK**, um den Export zu starten.</span><span class="sxs-lookup"><span data-stu-id="7badd-121">To export the data, choose the **OK** button.</span></span>  
  
    > [!WARNING]  
    >  <span data-ttu-id="7badd-122">Während des Exports werden alle vorhandenen Dateien, einschließlich der Protokolldatei, überschrieben.</span><span class="sxs-lookup"><span data-stu-id="7badd-122">During the export, any existing files, including the log file, will be overwritten.</span></span> <span data-ttu-id="7badd-123">Wenn Sie identische Daten mehrfach exportieren, werden die Dateien aus dem ersten Export überschrieben</span><span class="sxs-lookup"><span data-stu-id="7badd-123">If you export the same data twice, the files from the first export are overwritten</span></span>  
  
 <span data-ttu-id="7badd-124">Sie werden informiert, wenn der Export abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="7badd-124">You will be notified when the export completes.</span></span> <span data-ttu-id="7badd-125">Wenn Sie den Export abbrechen oder das Fenster schließen, werden Sie informiert, dass der Export abgeschlossen ist, aber der Protokollordner bleibt leer.</span><span class="sxs-lookup"><span data-stu-id="7badd-125">If you cancel the export, or if you close the window, you will also be notified that the export has completed, but the log folder will be empty.</span></span> <span data-ttu-id="7badd-126">Abhängig von Ihrer Konfiguration, wurden eventuell einige Dateien exportiert, aber der Export ist möglicherweise noch nicht abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="7badd-126">However, depending on your configuration, some files may have been exported, but the export might not be complete.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="7badd-127">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7badd-127">See Also</span></span>  
 [<span data-ttu-id="7badd-128">Prozess für Datenzugriff und zur Prüfbarkeit digitaler Unterlagen (GDPdU)</span><span class="sxs-lookup"><span data-stu-id="7badd-128">Process for Data Access and Testability of Digital Documents (GDPdU)</span></span>](process-for-data-access-and-testability-of-digital-documents-gdpdu-.md)
