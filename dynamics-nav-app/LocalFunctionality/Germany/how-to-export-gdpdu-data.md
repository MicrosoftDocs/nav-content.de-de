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
# <a name="how-to-export-gdpdu-data"></a>Gewusst wie: Exportieren von GDPdU-Daten
Sie können Finanz- und Steuerdatenaten entsprechend dem Prozess für Datenzugriff und Testbarkeit von digitalen Dokumenten (GDPdU), der auf deutschen Steuergesetzen basiert, exportieren. Zudem können verschiedene Optionen in eine XML-Datei eingeschlossen werden.  
  
 Falls es keine Daten zum Exportieren gibt, erstellt [!INCLUDE[navnow](../../includes/navnow_md.md)] leere Dateien.  
  
### <a name="to-export-gdpdu-data"></a>So exportieren Sie GDPdU-Daten  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen")und geben **Geschäftsdaten exportieren** ein. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Füllen Sie im Stapelverarbeitungsauftrag **GDPdU Export** im Inforegister **Optionen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  
  
    |ADD INCLUDE<!--[!INCLUDE[bp_tableoption](../../includes/bp_tabledescription_md.md)]-->|  
    |----------------------------------|---------------------------------------|  
    |**Startdatum**|Gibt das Startdatum des Berichts für den Datenexport an.<br /><br /> **HINWEIS:** Wenn die Datenenexportquell- ../../includes- Periodenfelder, das Startdatum und dem Enddatum als Filterwert für die Periodenfelder verwendet wird.|  
    |**Enddatum**|Gibt das Enddatum des Berichts für den Datenexport an.|  
    |**Abschlussdatum einschließen**|Gibt an, ob der Datenexport das Ultimodatum der Periode enthalten soll.|  
  
3.  Wählen Sie im Inforegister **Datenexport - Datensatzdefinition** die entsprechenden Filter aus, um den Datenexport zu identifizieren und Daten exportieren Datensatztyp. Weitere Informationen finden Sie unter [Prozess für Datenzugriff und zur Prüfbarkeit digitaler Unterlagen (GDPdU)](process-for-data-access-and-testability-of-digital-documents-gdpdu-.md)  
  
4.  Um Daten zu exportieren, wählen Sie die Schaltfläche **OK**, um den Export zu starten.  
  
    > [!WARNING]  
    >  Während des Exports werden alle vorhandenen Dateien, einschließlich der Protokolldatei, überschrieben. Wenn Sie identische Daten mehrfach exportieren, werden die Dateien aus dem ersten Export überschrieben  
  
 Sie werden informiert, wenn der Export abgeschlossen ist. Wenn Sie den Export abbrechen oder das Fenster schließen, werden Sie informiert, dass der Export abgeschlossen ist, aber der Protokollordner bleibt leer. Abhängig von Ihrer Konfiguration, wurden eventuell einige Dateien exportiert, aber der Export ist möglicherweise noch nicht abgeschlossen.  
  
## <a name="see-also"></a>Siehe auch  
 [Prozess für Datenzugriff und zur Prüfbarkeit digitaler Unterlagen (GDPdU)](process-for-data-access-and-testability-of-digital-documents-gdpdu-.md)
