---
title: "Gewusst wie: Einrichten von Datenexporten für GDPdU"
description: "Sie müssen die Export-Datensatzquellen einrichten, um die Grundsätze zum Datenzugriff und zur Prüfbarkeit digitaler Unterlagen zu (GDPdU) exportieren. Für jeden Datenexporttyp müssen Sie eine oder mehrere Datensatzquellen definieren, wobei jede Quelle eine Tabelle darstellt, aus der Daten exportiert werden sollen."
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
ms.openlocfilehash: bc4b284b71fa3e2c79f3b66d10dbddc4e1bd3296
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-data-exports-for-gdpdu"></a>Gewusst wie: Einrichten von Datenexporten für GDPdU
Sie müssen die Export-Datensatzquellen einrichten, um die Grundsätze zum Datenzugriff und zur Prüfbarkeit digitaler Unterlagen zu (GDPdU) exportieren. Für jeden Datenexporttyp müssen Sie eine oder mehrere Datensatzquellen definieren, wobei jede Quelle eine Tabelle darstellt, aus der Daten exportiert werden sollen.  
  
### <a name="to-set-up-a-gdpdu-data-export"></a>So richten Sie einen GDPdU-Datenexport ein  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Datenexporte** ein. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie auf der Registerkarte **Start** die Option **Neu** aus.  
  
3.  Füllen Sie im Fenster **Datenexporte** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  
  
    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Geben Sie den eindeutigen Code für den Datenexport, wie **Export-1** an.|  
    |**Beschreibung**|Definieren Sie die Beschreibung für den Datenexport.|  
  
 Dem Datenexport müssen Datensatzdefinitionen hinzugefügt werden. Jede Datensatzdefinition stellt eine Tabelle dar, aus der Daten exportiert werden.  
  
### <a name="to-add-a-record-definition-to-a-gdpdu-definition-group"></a>So fügen Sie einer GDPdU-Definitionsgruppe eine Datensatzdefinition hinzu  
  
1.  Wählen Sie auf der Registerkarte **Datenexport** in der Gruppe **Start** die Option **Definitionen aufzeigen** aus.  
  
2.  Füllen Sie im Fenster **Datenexport - Berichtsartendefinition** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  
  
    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Datenexportcode**|Wählen Sie den Datenexportcode aus.<br /><br /> Wenn kein Datenenexportcode vorhanden ist, können Sie einen neuen erstellen.|  
    |**Beschreibung**|Die Beschreibung der Datensatzdefinition.|  
    |**Exportpfad**|Definieren Sie den Pfad, in dem die exportierten Dateien gespeichert werden.|  
  
     Als Nächstes müssen Sie die entsprechende .dtd-Datei, die gemäß GDPdU erforderlich ist, z. B. **gdpdu-01-08-2002.dtd** hinzufügen. Wenn Sie eine neue DTD-Datei importieren müssen, um eine vorhandene Datei zu ersetzen, müssen Sie die vorhandene DTD-Datei zuerst exportieren.  
  
3.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **DTD-Datei** die Option **Importieren** aus.  
  
4.  Wählen Sie im Fenster **Importieren** die DTD-Datei aus, die den Workflow enthält, und wählen Sie dann die Schaltfläche **Öffnen**.  
  
 Danach müssen Sie die Quelle für die zu exportierenden Daten definieren.  
  
### <a name="to-add-source-tables-to-a-data-export"></a>So fügen Sie einem Datenexport Quelltabellen hinzu  
  
1.  Wählen Sie auf der Registerkarte **Datenexport-Definitionen** in der Gruppe **Start** die Option **Quelle aufzeigen** aus.  
  
2.  Füllen Sie im Fenster **Datenexport - Berichtsquelle** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  
  
    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Tabellennr.**|Wählen Sie die Nummer der Haupttabelle aus, aus der Daten exportiert werden sollen.<br /><br /> Wenn Sie einen Wert in Feld**Tabellennr.** eingeben das Feld  **Tabellenname** wird aktualisiert.|  
    |**Tabellenname exportieren**|Optional. Ändern Sie den vorgeschlagenen Namen der in der INDEX.XML-Datei verwendet wird während dem Export.<br /><br /> Der Wert des Felds **Tabellenname exportieren** wird verwendet, um die Datei INDEX.XML während des GDPdU-Datenexports zu generieren. Der Standardname ist der Name der Tabelle ohne Sonderzeichen aufgrund der Anforderungen des Prüftools.<br /><br /> **Tipp:** In den meisten Fällen basieren die Felder **Tabellenname exportieren** und **Exportdateiname** auf dem gleichen Wert.<br /><br /> Es kann Fälle geben, in denen Sie definieren, die selbe Tabelle mehrfach zu exportieren. Sie können verschiedene Export-Tabellennamen für jeden Tabelleneintrag auswählen, und die Export-Dateiname wird automatisch angepasst. Sie können den Export-Dateinamen ändern, solange er eindeutig ist.<br /><br /> [!INCLUDE[navnow](../../includes/navnow_md.md)] benennt automatisch die Dateien wie folgt.<br /><br /> **Tabellenname** Sachkonto<br /><br /> **Tabellenname exportieren**: Sachkonto<br /><br /> **Dateiname exportieren** Sachkonto.txt<br /><br /> **Tabellenname** Sachkonto<br /><br /> **Tabellenname exportieren:**: Sachkonto1<br /><br /> **Dateiname exportieren:** Sachkonto1.txt|  
    |**Periodenfeldnr.**|Geben Sie einen Filter an, für den das Feld zum Erstellen des XML-Dokuments verwendet wird und legen Sie das Startdatum und das Enddatum des Berichts fest.<br /><br /> Wenn Sie zum Beispiel die Tabelle **Sachposten** als Quelldatei für den Datenexport auswählen, können Sie eines der Datumsfelder auswählen, die in dieser Tabelle stehen.|  
    |**Tabellenfilter**|Geben Sie ein Feld an, für das Sie einen Filter festlegen möchten.<br /><br /> Im Fenster **Tabellenfilter** geben Sie Filtereinstellungen in der Spalte **Feldfilter** ein.<br /><br /> Beispielsweise können Sie ein Feld angeben, das Informationen über den Betrag überträgt. Sie können ein Datumsfeld festlegen und dafür einen Filter setzen, wenn Sie in einem Zeitraum unterschiedliche Startdaten setzen möchten. Enddatum. Sie können ein Datumsfeld nicht angeben und dafür einen Filter festlegen, wenn dasselbe Feld bereits im Feld Perioden-Gebiet " verwendet wird.|  
    |**Feldnr. Datumsfilter**|Definieren Sie ein Filterfeld, wenn die Tabelle eines hat.<br /><br /> Wenn die Tabelle mehr als einen Datumsfilter hat, definieren Sie keinen in diesem Feld.|  
    |**Behandlung von Datumsfiltern**|Geben Sie an, wie z. B.  Datumsfilter bearbeitet werden sollen:<br /><br /> * <blank>: Kein Filter festgelegt.<br /><br /> * Periode: Verwenden Sie das angegebene Startdatum und das Enddatum.<br /><br /> * Nur Enddatum: Verwenden Sie das Enddatum der Stapelverarbeitung.<br /><br /> * Nur Startdatum: Verwenden Sie das Startdatum - 1 der Stapelverarbeitung.|  
    |**Exportdateiname**|Geben Sie den Namen der Arbeitsmappe an, in die die Daten exportiert werden sollen.<br /><br /> Wenn die Tabelle beispielsweise **Sachkonto** ist, kann der Wert des **Tabellennamen exportieren** **Sachkonto** sein, und der Wert des Felds **Exportdateiname** kann **Sachkonto.txt** sein.|  
    |**Schlüsselnr.**|Optional. Definieren Sie das Schlüsselfeld.|  
  
     Weitere Informationen über Einstellungsfilter siehe. [GDPdU-Filter-Beispiele](gdpdu-filter-examples.md).  
  
     Danach müssen Sie die Felder definieren, von denen Daten exportiert werden.  
  
3.  Im Bereich **Felder** wählen Sie **Hinzufügen** aus.  
  
4.  Im Fenster **Datenexport-Felderübersicht** wählen Sie ein oder mehrere Felder aus, die Sie exportieren möchten, und wählen Sie dann die Schaltfläche **OK** aus.  
  
    1.  Wählen Sie auf der Registerkarte Aktionen **Nach oben** oder **Nach unten**, um die Reihenfolge der Felder zu ändern.  
  
    2.  Um ein Feld aus der Liste der ausgewählten Felder zu entfernen, wählen Sie **Löschen**.  
  
 Sie haben die Haupttabelle hinzugefügt, aus der Daten exportiert werden sollen. Optional können Sie mindestens eine zugehörige Tabelle hinzufügen.  
  
### <a name="to-add-related-tables-to-a-data-export-source"></a>So fügen Sie eine verwandte Tabelle einer Datenexportquelle hinzu  
  
1.  Im Fenster **Datenexport - Datensatzherkunft** in der Zeile unter der Zeile für die Haupttabelle fügen Sie die verknüpfte Tabelle hinzu.  
  
2.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Einrückung** die Option **Einrücken** aus.  
  
3.  Wählen Sie die eingerückte Tabelle und dann auf der Registerkarte **Start** in der Gruppe **Einrückung** die Option **Beziehung** aus.  
  
4.  Füllen Sie im Fenster **GDPdU Definitionsgruppen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  
  
    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Von Feldnr.**|Enthält die Nummer des Feld in der übergeordneten Tabelle. Sie können angeben, dass das Feld einen Bezug zu einem Feld in der untergeordneten Tabelle besitzt.|  
    |**Zu Feldnr.**|Enthält die Nummer des Felds in der untergeordneten Tabelle. Sie können angeben, dass ein Feld in der übergeordneten Tabelle einen Bezug zu diesem Feld besitzt.|  
  
    > [!NOTE]  
    >  Die Felder **Von Feldname** und **Zu Feldname** werden automatisch ausgefüllt.  
  
5.  Wählen Sie die Schaltfläche **OK** aus.  
  
 Nachdem Sie Tabellen und Felder hinzugefügt haben, müssen Sie überprüfen, dass die Struktur der Datenexportquelle korrekt ist.  
  
### <a name="to-validate-the-data-export-source"></a>Um die Datenexportquelle zu überprüfen  
  
-   Wählen Sie im Fenster **Datenexportquelle** auf der Registerkarte **Start** in der Gruppe **Verarbeiten** die Option **Prüfen**.  
  
     Dies überprüft die Liste der Felder anhand der Schlüssel für die Tabellen. Wenn Sie einen Primärschlüssel auswählen, nachdem Sie einen sekundären Schlüssel ausgewählt haben, wird eine Fehlermeldung angezeigt und Sie müssen die Reihenfolge der Felder im Bereich **Felder** ändern.  
  
## <a name="see-also"></a>Siehe auch  
 [Prozess für Datenzugriff und zur Prüfbarkeit digitaler Unterlagen (GDPdU)](process-for-data-access-and-testability-of-digital-documents-gdpdu-.md)   
 [Gewusst wie: Exportieren von GDPdU-Daten](how-to-export-gdpdu-data.md)   
 [GDPdU-Filterbeispiele](gdpdu-filter-examples.md)
