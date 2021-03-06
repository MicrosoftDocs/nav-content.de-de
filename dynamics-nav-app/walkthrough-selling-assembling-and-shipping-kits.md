---
title: 'Exemplarische Vorgehensweise: Verkauf, Montage und Liefern von Kits'
description: "Um eine Just-In-Time-Logistik sowie die Möglichkeit, Produkte an Debitorenanfragen anzupassen, zu unterstützen, können Montageaufträge automatisch erstellt und verknüpft werden, sobald die Verkaufsauftragszeile erstellt wird. Der Verknüpfung zwischen dem Verkaufsbedarf und dem Montagezubehör ermöglicht Verkaufsauftragsverarbeitern die Anpassung des Montageartikels und die Zusage von Lieferungsdaten auf der Grundlage der Verfügbarkeit von Komponenten. Darüber hinaus werden der Montageverbrauch und die Ausgabe automatisch mit der Lieferung des verknüpften Verkaufsauftrags gebucht."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7cc4a50a981041d066e029da7e6a2666241e38eb
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-selling-assembling-and-shipping-kits"></a>Exemplarische Vorgehensweise: Verkauf, Montage und Liefern von Kits
Um eine Just-In-Time-Logistik sowie die Möglichkeit, Produkte an Debitorenanfragen anzupassen, zu unterstützen, können Montageaufträge automatisch erstellt und verknüpft werden, sobald die Verkaufsauftragszeile erstellt wird. Der Verknüpfung zwischen dem Verkaufsbedarf und dem Montagezubehör ermöglicht Verkaufsauftragsverarbeitern die Anpassung des Montageartikels und die Zusage von Lieferungsdaten auf der Grundlage der Verfügbarkeit von Komponenten. Darüber hinaus werden der Montageverbrauch und die Ausgabe automatisch mit der Lieferung des verknüpften Verkaufsauftrags gebucht.  

Es sind spezielle Funktionen vorhanden, um die Lieferung von Auftragsmontagemengen zu steuern, sowohl in einfachen als auch in erweiterten Lagerkonfigurationen. Wenn Arbeiter für montagefertige Teile oder für die gesamte Auftragsmontagemenge zuständig sind, erfassen sie diese im Feld **Vesandmenge** in der Warenausgangszeile, in erweiterten Konfigurationen, und wählen dann **Warenausgang buchen**. Das Ergebnis ist, dass der entsprechende Montageausstoß, einschließlich des zugehörigen Komponentenverbrauchs, gebucht wird und eine Verkaufslieferung für die Menge für den verknüpften Verkaufsauftrag gebucht wird. Diese Anleitung illustriert den erweiterten Lagerprozess.  

In Basis-Lagerkonfigurationen bucht der zuständige Lagermitarbeiter für die jeweiligen Verkaufsauftragszeilen eine Lagerkommissionierung, wenn eine Auftragsmontagemenge für die Lieferung bereitsteht. Dies erstellt eine Lagerbestandsumlagerung für die Komponenten und bucht den Montageausstoß und die Verkaufsauftragslieferung. Weitere Informationen finden Sie im Abschnitt "Verwenden von Auftragsmontageartikeln in Lagerkommissionierungen" in Lagerkommissionierung  

## <a name="about-this-walkthrough"></a>Informationen zu dieser exemplarischen Vorgehensweise  
In dieser exemplarischen Vorgehensweise werden folgende Aufgaben erläutert:  

### <a name="setting-up-assembly-items"></a>Montageartikel einrichten  
Montageartikel sind durch ihre Beschaffungsmethode und die Montagestückliste charakterisiert. Die Montagerichtlinie des Artikels kann entweder Auftragsmontage- (ATO) oder Lagerfertigung (ATS) sein. Dieser Abschnitt behandelt die folgenden Aufgaben:  

-   Einrichten der korrekten Beschaffungsmethode und der Montagerichtlinie auf einer neuen Montageartikelkarte.  
-   Erstellen einer Montagestückliste, die die Montagekomponenten und die Ressource auflistet, die zu dem Montageartikel gehören.  

### <a name="selling-customized-assembly-items"></a>Verkauf von benutzerdefinierten Montageartikeln  
[!INCLUDE[d365fin](includes/d365fin_md.md)] bietet die Flexibilität, eine Lagermenge und eine Programmfertigungsmenge in einer Verkaufsauftragszeile einzugeben. Dieser Abschnitt behandelt die folgenden Aufgaben:  

-   Erstellen einer reinen ATO-Verkaufsauftragszeile, in der die gesamte Menge nicht verfügbar ist und vor dem Warenausgang montiert werden muss.  
-   Anpassen von ATO-Artikeln.  
-   Neuberechnen des VK-Preises eines benutzerdefinierten Montageartikels.  
-   Erstellen einer Mischverkaufsauftragszeile, in der die Teile der Vertriebsmenge aus dem Lagerbestand bereitgestellt werden und der Rest vor dem Warenausgang montiert werden muss.  
-   Verstehen der ATO-Verfügbarkeitswarnungen.  

### <a name="planning-for-assembly-items"></a>Planung für Montageartikel  
Montagenachfrage und -angebot werden vom Planungssystem ähnlich wie für Einkauf, Umlagerung und Produktion behandelt. Dieser Abschnitt behandelt die folgenden Aufgaben:  

-   Durchführen einer Neuplanung für Artikel mit Verkaufsbedarf für assemblierte Bedarfssicherung.  
-   Generierung eines Montageauftrags zur Erfüllung einer Verkaufspositionsmenge durch das angefragte Lieferdatum.  

### <a name="assembling-items"></a>Artikelmontage  
Montageaufträge funktionieren in ähnlicher Weise wie Fertigungsaufträge; sie erwarten, dass der Verbrauch und die Ausgabe direkt aus dem Auftrag erfasst und gebucht werden. Wenn die Artikel zum Bestand montiert werden, hat der Montagearbeiter vollständigen Zugriff auf alle Kopf- und Zeilenfelder. Wenn die Artikel für einen Auftrag montiert werden, in dem dem Debitor Menge und Datum zugesagt werden, können bestimmte Felder im Montageauftrag nicht bearbeitet werden. In diesem Fall wird die Montagebuchung aus dem Warenausgang für den verknüpften Verkaufsauftrag ausgeführt. Dieser Abschnitt behandelt die folgenden Aufgaben.  

-   Erfassung und Buchung von Montageverbrauch und -ausgabe für den Bestand.  
-   Aufrufen einer Warenausgangszeile aus einem ATO-Montageauftrag zur Erfassung von Montagearbeit.  
-   Aufrufen eines ATO-Montageauftrags aus einer Warenausgangszeile zur Prüfung der automatisch eingegebenen Daten.  

### <a name="shipping-assembly-items-from-stock-and-assembled-to-order"></a>Versand von Montageartikeln, aus Lagerbestand und nach Auftrag montiert  
Es sind spezielle Funktionen vorhanden, um den Versand von Auftragsmontagemengen zu steuern. Dieser Abschnitt behandelt die folgenden Aufgaben:  

-   Erstellen einer Lagerkommissionierung für Montageartikel und Montagekomponenten zur Montage vor der Lieferung.  
-   Erfassen von Lagerkommissionierungen für Montagekomponenten und dann für Montageartikel.  
-   Aufrufen eines Montageauftrags aus einem Warenausgang zur Prüfung der kommissionierten oder verbrauchten Komponenten.  
-   Versenden von Auftragsmontagemengen.  
-   Versenden von Bestandsmontageartikeln.  

## <a name="roles"></a>Rollen  
Die Aufgaben in dieser Demonstration werden von den folgenden Benutzerrollen ausgeführt:  

-   Verkaufsauftragsbearbeiter  
-   Planer  
-   Montagearbeiter  
-   Kommissionierer  
-   Lieferverantwortlicher  

## <a name="prerequisites"></a>Voraussetzungen  
Für diese exemplarische Vorgehensweise gelten folgende Voraussetzungen:  

-   Installieren von [!INCLUDE[d365fin](includes/d365fin_md.md)]  
-   Machen Sie sich anhand der nachfolgenden Schritte selbst zu einem Lagermitarbeiter am Standort WHITE:  

1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Lagerhaus-Mitarbeiter** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie das Feld **Benutzer-ID** aus, und wählen Sie Ihr eigenes Benutzerkonto im Fenster **Benutzer** aus.  
3.  Geben Sie im Feld **Lagerortcode** WHITE ein.  
4.  Wählen Sie das Feld **Standard** aus.  

Bereiten Sie den Lagerort WHITE folgendermaßen für die Montageverarbeitung vor:  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Öffnen Sie die Lagerortkarte für den Lagerort WHITE.  
3.  Im Inforegister **Lagerplätze** geben Sie **W-10-0001** im Feld **Mont.-Bereitst.-Lagerplatzcode** ein.  

    Durch die Eingabe dieses Nicht-Kommissionierungslagerplatzcodes werden alle Montageauftragszeilen zur Aufnahme ihrer Komponenten an dem Lagerplatz vorbereitet.  

4.  In dem Feld **Montage-Ausgangslagerplatzcode** geben Sie **W-01-0001** ein.  

    Durch die Eingabe dieses Kommissionierungslagerplatzcodes werden fertige Montageartikel an den Lagerplatz ausgegeben.  

Entfernen Sie die Standard-Beschaffungszeit für interne Vorgänge, indem Sie die folgenden Schritte befolgen:  

1.  Um das Fenster Marketing einzurichten, wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben **Herstellung einrichten** ein und wählen den entsprechenden Link aus.  
2.  Im Fenster **Produktion Einrichtung** im Inforegister **Planung**, löschen Sie den Wert im Feld **Vorg. Sich.-Zuschl. Besch.-Zt.** Feld.  

Erstellen Sie Bestand für Montagekomponenten, indem Sie die Anweisungen im Abschnitt "Vorbereiten von Beispieldaten" in dieser Anleitung befolgen.  

## <a name="story"></a>Hintergrund  
Am 23. Januar akzeptiert Martha, die Verkaufsauftragsverarbeiterin, einen Auftrag von The Device Shop für drei Einheiten von Kit B, wobei es sich um einen ATO-Artikel handelt. Alle drei Einheiten werden individuell angepasst und müssen eine leistungsstarke Grafikkarte und einen zusätzlichen RAM-Block enthalten. Die Laufwerke werden auf DWD aktualisiert, da die CD-Laufwerke nicht verfügbar sind. Martha weiß, dass die Einheiten sofort montiert werden können, sie lässt daher das vorgeschlagene Lieferdatum vom 23. Januar unverändert.  

Gleichzeitig bestellt der Kunde fünfzehn Einheiten von Kit A mit der speziellen Anforderung, dass fünf Einheiten mit der leistungsstarken Grafikkarte ausgerüstet werden. Obwohl Kit A typischerweise ein Bestandsfertigungsartikel ist, kombiniert die Auftragsbearbeiterin die Verkaufszeilenmengen, um zehn Einheiten aus dem Lagerbestand zu verkaufen und fünf Einheiten gemäß diesem Auftrag zu montieren. Die zehn Einheiten von Kit A sind nicht verfügbar und müssen gemäß der Montagerichtlinie des Artikels zuerst durch einen Montageauftrag in den Bestand eingefügt werden. Martha erfährt aus der Montageabteilung, dass Einheiten von Kit A in der laufenden Woche nicht fertiggestellt werden können. Sie setzt das Lieferdatum der zweiten Verkaufsauftragszeile, für die gemischte ATO- und Bestandsmenge, auf den 27. Januar fest und informiert den Kunden, dass die 15 Einheiten von Kit A vier Tage später geliefert wurden, als die drei Einheiten von Kit B. Um der Versandabteilung mitzuteilen, dass dieser Verkaufsauftrag Montageverarbeitung erfordert, erstellt sie den Warenausgangsbeleg aus dem Verkaufsauftrag.  

Jürgen, der Planer, führt das Planungsarbeitsblatt und erstellt einen Montageauftrag für zehn Standardeinheiten aus Kit A mit einem internen Fälligkeitsdatum am 27. Januar.  

Sammy, der für die Lieferung verantwortlich ist, ruft drei Warenausgangszeilen für den Verkaufsauftrag ab: Eine Zeile für die drei reinen ATO-Einheiten, eine Zeile für die fünf ATO-Einheiten in der Mischverkaufsauftragszeile und eine Zeile für die zehn ATS-Einheiten in der Mischverkaufsauftragszeile. Er erstellt einen Kommissionierbeleg über alle Montagekomponenten, die benötigt werden, um die insgesamt acht ATO-Einheiten im Warenausgangsbeleg zu montieren.  

Wilfried, der Kommissionierer, ruft Komponenten für alle ATO-Mengen auf dem Warenausgangsbeleg ab und bringt diese in den Miontagebereich. Er gibt die zu verwendende Menge ein und registriert die Kommissionierung.  

Elfriede montiert die drei ATO-Einheiten aus Kit B. Die Komponenten sind bereits kommissioniert, und sie erfasst nicht die Ausgabe- und Verbrauchsmengen und bucht auch nicht den Auftrag, da beides bereits automatisch durch die entsprechenden Lagersendungszeilen durchgeführt wird.  

Sammy speichert die montierte Menge in der Warenausgangszeile und bucht die Lieferung der drei Einheiten von Kit B. Die erste Zeile des Auftrags wird als geliefert aktualisiert. Der verknüpfte Montageauftrag bleibt offen, bis der Verkaufsauftrag vollständig fakturiert ist. Die zwei Warenausgangszeilen, eine ATO- und eine ATS-Zeile, für Kit A mit Fälligkeitsdatum 27. Januar bleiben offen.  

Am 27. Januar verarbeitet Linda zwei Montageaufträge für Kit A. Die erste Bestellung ist der ATO-Auftrag für fünf Einheiten, die sie anders als die ATO-Bestellung verarbeitet für Kit B, das sie am 23. Januar verarbeitet hat. In diesem Auftrag wird sie autorisiert, um selber auf die Warenausgangszeile zuzugreifen, um die vollständige Montagearbeit zu erfassen. Die benötigten Komponenten stehen in der Montageabteilung zur Verfügung, da sie zusammen mit Komponenten für Kit B kommissioniert wurden.  

Der zweite Montageauftrag ist der ATS-Auftrag für zehn Einheiten, der vom Planungssystem erstellt wurde. Auf diesem ATS-Auftrag führt Elfriede alle betreffenden Aktionen aus dem Montageauftrag aus. Sie erstellt einen Kommissionierbeleg für die Montagekomponenten, die benötigt werden, um die zehn Einheiten zu montieren. Wenn die Geräte montiert werden, bucht Elfriede den Montageauftrag und gibt damit an, dass die Artikel im Bestand verfügbar sind und für die Lieferung kommissioniert werden können.  

Sammy erstellt einen Kommissionierbeleg für alle verbleibenden Mengen, bevor der Warenausgang gebucht werden kann. Ein Kommissionierbeleg wird für die zehn Einheiten von Kit A erstellt, die soeben fertig gestellt wurden. Die Komponenten, die benötigt werden, um die fünf Einheiten von Kit A gemäß dem Auftrag zu montieren, wurden am 23. Januar kommissioniert.  

Wilfried bringt die zehn Einheiten von Kit A aus dem Lager in den angegebenen Warenausgangsbereich, registriert die zu verwendende Menge und dann die Kommissionierung.  

Sammy verpackt die zehn ATS-Einheiten mit den fünf ATO-Einheiten, die Elfriede zuvor montiert hat. Er gibt auf beiden Zeilen die Liefermenge ein und bucht die letzte Lieferung für The Device Shop. Der zugehörige Montageauftrag für fünf Einheiten von Kit A wird automatisch gebucht. Die zweite Zeile auf dem Verkaufsauftrag wird als "geliefert" aktualisiert. Zwei verknüpfte Montageaufträge bleiben offen, bis der Verkaufsauftrag fakturiert und abgeschlossen ist.  

Wenn der Auftrag später als vollständig fakturiert gebucht wird, werden der Verkaufsauftrag und die verknüpften Montageaufträge entfernt.  

## <a name="setting-up-the-sample-data"></a>Einrichten der Beispieldaten  

1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Fibu Buchblatt** ein und wählen den zugehörenden Link aus.  
2.  Wählen Sie das Feld **Buch.-Blattname**, und wählen Sie anschließend das Standardjournal aus.  
3.  Erstellen Sie positive Lagerregulierungen am Lagerort WHITE am Arbeitsdatum 23. Januar, indem Sie die folgenden Informationen eingeben.  

    |**Artikelnr.**|**Zonencode**|**Lagerplatzcode**|**Menge**|  
    |-----------------------------------|---------------------------------------|--------------------------------------|------------------------------------|  
    |80001|KOMMISS|W-01-0001|2.0|  
    |80005|KOMMISS|W-01-0001|2.0|  
    |80011|KOMMISS|W-01-0001|20|  
    |80014|KOMMISS|W-01-0001|20|  
    |80203|KOMMISS|W-01-0001|20|  
    |80209|KOMMISS|W-01-0001|20|  

4.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Registrieren** die Option **Registrieren** aus, und klicken Sie anschließend auf die Schaltfläche **Ja**.  

    Synchronisieren Sie anschließend die neuen Lagereinträge mit dem Bestand.  

5.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Fibu Buchblatt** ein und wählen den zugehörenden Link aus. Das Fenster  **Artikel Buch.-Blatt** wird geöffnet.  
6.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Ausgleich berechnen** aus.  
7.  Um die Funktion **Ausgleich berechnen** auszuführen, wählen Sie die Schaltfläche **OK** aus.  
8.  Wählen Sie im Fenster **Artikeljournal** auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Buchen**, und klicken Sie dann auf die Schaltfläche **Ja**  

### <a name="creating-the-assembly-items"></a>Erstellen der Montageartikel  

1.  Wählen Sie ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol nach Seite oder Bericht suchen") aus und geben Sie **Artikel** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Verwalten** die Option **Neu** aus.  
3.  Erstellen Sie den ersten Montageartikel auf der Grundlage der folgenden Informationen.  

    |Feld|Wert|  
    |---------------------------------|-----------|  
    |**Beschreibung**|Kit A – Basis-PC|  
    |**Basismaßeinheit**|STÜCK|  
    |**Artikelkategoriencode**|Sonst.|  
    |**Beschaffungsmethode**|Montage|  
    |**Montagerichtlinie**|Lagermontage|  
    |**Wiederbeschaffungsverfahren**|Los-für-Los|  

    > [!NOTE]  
    >  Kit A wird in der Regel durch Bestandsmontage geliefert und verfügt daher über ein Wiederbeschaffungsverfahren, durch das es zum Teil der allgemeinen Wiederbeschaffungsplanung wird.  

4.  Wählen Sie auf der Registerkarte **Navigieren** in der Gruppe **Montage/Fertigung** **Montage** aus, und klicken Sie anschließend auf **Montagestückliste**.  
5.  Definieren Sie eine Montagestückliste für Kit A mit den folgenden Informationen.  

    |**Typ**|**Nr.**|**Komponentenmenge**|  
    |-------------------------------|------------------------------|---------------------------------------|  
    |Artikel|80001|0|  
    |Artikel|80011|0|  
    |Artikel|80209|0|  
    |Ressource|Linda|0|  

6.  Erstellen Sie den zweiten Montageartikel auf der Grundlage der folgenden Informationen.  

    |Feld|Wert|  
    |---------------------------------|-----------|  
    |**Beschreibung**|Kit B – Profi-PC|  
    |**Basismaßeinheit**|STÜCK|  
    |**Artikelkategoriencode**|Sonst.|  
    |**Beschaffungsmethode**|Montage|  
    |**Montagerichtlinie**|Programmfertigung|  

    > [!NOTE]  
    >  Kit B wird normalerweise als Montageartikel geliefert und verfügt daher über kein Wiederbeschaffungsverfahren, da es nicht zur allgemeinen Wiederbeschaffungsplanung gehören soll.  

7.  Wählen Sie auf der Registerkarte **Navigieren** in der Gruppe **Montage/Fertigung** **Montage** aus, und klicken Sie anschließend auf **Montagestückliste**.  
8.  Definieren Sie eine Montagestückliste für Kit B mit den folgenden Informationen.  

    |**Typ**|**Nr.**|**Komponentenmenge**|  
    |-------------------------------|------------------------------|---------------------------------------|  
    |Artikel|80005|0|  
    |Artikel|80014|0|  
    |Artikel|80210|0|  
    |Ressource|Linda|0|  

### <a name="selling-the-assembly-items"></a>Verlaufen der Montageartikel  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus, geben Sie **Verkaufsaufträge** ein, und wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Verwalten** die Option **Neu** aus.  
3.  Erstellen Sie zwei Verkaufsauftragszeilen für Debitor 62000, The Device Shop, am Arbeitsdatum mit den folgenden Informationen.  

    |**Typ**|**Beschreibung**|**Menge**|Menge für Auftragsmontage|Warenausg.-Datum|  
    |--------------|---------------------|------------------|-------------------------------|-------------------|  
    |Artikel|Kit B – Profi-PC|3|3|23. Januar|  
    |Artikel|Kit A – Basis-PC|15|5|27. Januar|  

    > [!NOTE]  
    >  Für die Verkaufsauftragszeile für Kit B besteht das folgende Verfügbarkeitsproblem:  
    >   
    >  -   Montagekomponente 80210 ist nicht verfügbar. Dies bedeutet, dass die drei angegebenen Einheiten von Kit B nicht montiert werden können, angezeigt durch **0** im Feld **Montage möglich** im Fenster **Montageverfügbarkeit** .  
    >   
    >  Für die Verkaufsauftragszeile für Kit A besteht das folgende Verfügbarkeitsproblem:  
    >   
    >  -   Die zehn Einheiten von Kit A sind nicht verfügbar. Dies zeigt dem Planungssystem an, dass die Menge zum Bestand montiert werden muss.  

    Passen Sie anschließend den Verkaufsauftrag an.  

4.  Wählen Sie die Verkaufsauftragszeile für drei Einheiten von Kit B.  
5.  Wählen Sie auf dem Inforegister **Zeilen** **Zeile** aus, wählen Sie **Auftragsmontage**, und klicken Sie anschließend auf **Auftragsmontagezeilen**.  
6.  Im Fenster **Programmfertigungszeilen** der Montageauftragszeile für Artikel 80014, geben Sie **2** im Feld **Komponentenmenge** ein.  
7.  Auf der Montageauftragszeile für Artikel 80210, wählen Sie **Nr.** aus und klicken Sie anschließend auf Artikel 80209.  
8.  Erstellen Sie eine neue Montageauftragszeile mit den folgenden Informationen.  

    |Typ|Nr.|Komponentenmenge|  
    |----------|---------|------------------|  
    |Artikel|80203|0|  

9. Schließen Sie das Fenster **Auftragsmontagezeilen**.  

    Aktualisieren Sie dann den VK-Preis von Kit B entsprechend der Anpassung, die Sie gerade durchgeführt haben. Beachten Sie den aktuellen Wert im Feld **VK-Preis ohne MwSt.**.  

10. Wählen Sie auf dem Inforegister **Zeilen** **Zeile** aus, wählen Sie **Auftragsmontage**, und klicken Sie anschließend auf **Mehrstufigen Preis berechnen**.  
11. Wählen Sie die Schaltfläche **Ja** aus. Beachten Sie den höheren Wert im Feld **VK-Preis ohne MwSt.**.  
12. Wählen Sie die Verkaufsauftragszeile für 15 Einheiten von Kit A.  
13. Wählen Sie auf dem Inforegister **Zeilen** **Zeile** aus, wählen Sie **Auftragsmontage**, und klicken Sie anschließend auf **Auftragsmontagezeilen**.  
14. Erstellen Sie im Fenster **Auftragsmontagezeile** eine neue Montageauftragszeile mit den folgenden Informationen.  

    |Typ|Nr.|Komponentenmenge|  
    |----------|---------|------------------|  
    |Artikel|80203|1|  

     Ändern Sie dann das Lieferdatum gemäß dem Montagezeitplan.  

15. Geben Sie auf der Verkaufsauftragszeile für 15 Einheiten von Kit A **01-27-2014**im Feld **Versanddatum** ein.  
16. Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Freigeben** die Option **Freigeben** aus.  
17. Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Lager** die Option **Warenausgang erstellen** aus.  
18. Schließen Sie den Verkaufsauftrag.  

### <a name="planning-for-the-unavailable-ats-items"></a>Planen für die nicht verfügbaren ATS-Artikel  

1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen] Symbol (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Arbeitszeitplanung** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie auf der Registerkarte **Aktion** in der Gruppe **Funktionen** die Option **Neuplanung berechnen** aus.  
3.  Stellen Sie im Fenster **Planung berechnen** die folgenden Filter ein.  

    |Startdatum|Enddatum|Nr.|  
    |-------------------|-----------------|---------|  
    |01-23-2014|01-27-2014|Kit A – Basis-PC|  

4.  Wählen Sie die Schaltfläche **OK** aus.  

    Eine neue Planungszeile wird für den erforderlichen Montageauftrag über zehn Stück fällig am 27. Januar erstellt. Es muss keine Änderung vorgenommen werden, sodass Sie nun einen Auftrag anlegen können.  

5.  Wählen Sie auf der Registerkarte **Funktionen** in der Gruppe **Vorgang** die Option **Ereignismeldung durchführen** aus.  
6.  Wählen Sie im Fenster **Ereignismeld. durchf.** das Feld **Montageauftrag** und dann **Montageaufträge erstellen**.  
7.  Wählen Sie die Schaltfläche **OK** aus.  

### <a name="assembling-and-shipping-the-first-ato-quantity"></a>Montieren und Versenden der ersten ATO-Menge  

1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Fibu Buchblatt** ein und wählen den zugehörenden Link aus.  

    > [!NOTE]  
    >  In diesem Abschnitt ist die Person, die für die Lieferung verantwortlich ist, für die Registrierung der abgeschlossenen ATO-Montagearbeit auf der Warenausgangszeile zuständig. Dieser Workflow kann in Umgebungen vorkommen, in denen die Montagearbeit von der Person, die für die Lieferung verantwortlich ist, bzw. von Montagearbeitern im Auslieferungsbereich durchgeführt wird.  
    >   
    >  In diesem Abschnitt werden die Aktionen auf dem Montageauftrag indirekt von der Warenausgangszeile aus ausgeführt. Weitere Informationen darüber, wie ein Montageauftrag direkt verarbeitet wird, finden Sie unter "Artikel für Bestand montieren" in dieser Anleitung".  

2.  Öffnen Sie den neuesten Warenausgang, der am Lagerort WHITE erstellt wurde.  

    Beachten Sie die drei Warenausgangszeilen: Eine Zeile für die ATO-Menge des Kits B, fällig am 23. Januar. Eine Zeile für die ATO-Menge von A Kit, fällig am 27. Januar. Eine Zeile für die Bestand-Menge von Kit A, fällig am 27. Januar.  

    Das Feld **Auftragsmontage** gibt die Fertigungsmethode an.

    Erstellen Sie dann einen Kommissionierbeleg für alle ATO-Montagekomponenten, die für den Warenausgang benötigt werden.  

3.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Kommissionierung erstellen** aus, und wählen Sie anschließend **OK** aus.  

    Führen Sie dann die Aufgaben des Komissionierers aus.  

4.  Wählen Sie ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben Sie **Auswahl** ein und wählen dann den zugehörigen Link aus.  
5.  Öffnen Sie den Kommissionierbeleg, den Sie in Schritt 3 in diesem Abschnitt erstellt haben.  

    Beachten Sie den Wert im Feld **Quelldokument** und dass alle Kommissionierzeilen für Montagekomponenten gelten.  

    Registrieren Sie dann die Kommissionierung, ohne die Standardinformationen zu ändern.  

6.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Bewegungsmenge autom. ausfüllen** aus.  
7.  Wählen Sie auf der Registerkarte **Start**, in der Gruppe **Registrierung**, die Option **Kommissionierung registrieren**.  

    Kehren Sie zum Ausführen der Versandaufgaben zurück.  

8.  Öffnen Sie wieder das Fenster **Warenausgangsübersicht**.  

    Beachten Sie, dass das Feld **Ausgewählte Menge** auf allen Zeilen noch leer ist. Dies liegt daran, dass Sie die zu liefernden Artikel noch nicht kommissioniert haben, sondern nur die Komponenten, die benötigt werden, um die ATO-Mengen zu montieren.  

    Fahren Sie fort, um den verknüpften Montageauftrag zu prüfen.  

9. Wählen Sie die Warenausgangszeile für drei Einheiten von Kit B.  
10. Wählen Sie auf dem Inforegister **Zeilen** **Zeile** aus, und wählen Sie dann **Auftragsmontage**. Das Fenster **Montageauftrag** wird geöffnet.  

    Beachten Sie, dass einige Felder auf dem Montageauftrag nicht verfügbar sind, da der Auftrag mit einem Verkaufsauftrag verbunden ist.  

    Beachten Sie auf den Montageauftragszeilen, dass das Feld **Ausgewählte** ausgefüllt ist. Der Grund dafür ist die Kommissionierung, die Sie in Schritt 7 registriert haben.  

11. Versuchen Sie, in Feld **Montagemenge** einen Wert unter **3** einzugeben.  

    Lesen Sie die Fehlermeldung, die erläutert, warum dieses Feld nur durch das Feld **Versandmenge** auf der entsprechenden Lieferung ausgefüllt werden kann.  

    Das Feld **Montagemenge** ist editierbar, um Situationen zu unterstützen, in denen Sie eine Lagermenge teilweise ausliefern möchten, anstatt mehr Einheiten für den Auftrag zu montieren. Weitere Informationen finden Sie im Abschnitt "Kombinationsszenarien" in [Auftragsmontage und Lagermontage verstehen](assembly-assemble-to-order-or-assemble-to-stock.md).  

12. Schließen Sie das Fenster **Montageauftrag**, um zum Fenster **Warenausgang** zurückzukehren.  
13. Geben Sie auf der Ausgangszeile für drei Einheiten von Kit B im Feld **Versandmenge**  **3** ein.  
14. Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Buchen** die Option **Warenausgang buchen**, und wählen Sie dann die Schaltfläche **Liefern**.  

    Zusammen mit dieser Warenausgangbuchung werden die vollständige Verbrauchs- und Ausgabemenge des zugehörigen Montageauftrags gebucht, und das Feld **Verbleibende Menge** ist leer. Die Verkaufsauftragszeile für Kit B wird aktualisiert, um zu zeigen, dass die drei Einheiten geliefert werden.  

    Die Lageraktivitäten zum Erfüllen der ersten Verkaufsauftragszeile bis 23. Januar sind abgeschlossen. Als Nächstes erfüllen Sie die Verkaufsauftragszeilen, die am 27. Januar geliefert werden.  

### <a name="assembling-and-recording-the-second-ato-quantity"></a>Montieren und erfassen der zweiten ATO-Menge  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Montageaufträge** ein und wählen dann den zugehörigen Link aus.  

    Beachten Sie, dass das der ATO-Auftrag für gelieferte Einheiten von Kit B noch in der Liste ist, obwohl **Verbleibende Menge** leer ist. Dies liegt daran, dass der verknüpfte Verkaufsauftrag noch nicht vollständig fakturiert ist.  

    > [!NOTE]  
    >  In diesem Abschnitt ist der Montagearbeiter für die Erfassung der abgeschlossenen ATO-Montagearbeit auf der Warenausgangszeile zuständig. Dieser Workflow kann vorkommen in Umgebungen auftreten, in der die Montagearbeit in einer separaten Montageabteilung ausgeführt wird und Montagearbeiter autorisiert sind, um die Warenausgangszeile zu ändern.  

2.  Öffnen Sie den ATO-Montageauftrag für fünf Einheiten des Kit A.  

    Beachten Sie, dass die Felder **Menge für Montage** und **Verbrauchsmenge** leer sind, da keine Arbeit erfasst wird.  

    Beachten Sie auf den Montageauftragszeilen, dass das Feld **Ausgewählte** ausgefüllt ist. Dies liegt an der Kommissionierung, die am 23. Januar erfasst wurde.  

    Buchen Sie dann, dass der Montageauftrag abgeschlossen ist.  

3.  Klicken Sie auf der Registerkarte **Navigate** in der Gruppe **Lager**, wählen Sie **Warenausgangszeile für Programmfertigung** aus.  
4.  Geben Sie im Fenster **Warenausgangszeile für Programmfertigung**im Feld **Versandmenge** **5** ein und schließen Sie dann das Fenster.  

    Beachten Sie im Fenster , dass die Felder **Montageauftrag** und **Montagemenge** jetzt mit den **Verbrauchsmengen** ausgefüllt sind, die mit der Lieferung gebucht werden.  

5.  Schließen Sie das Fenster **Montageauftrag**.  

### <a name="assembling-the-ats-quantity"></a>Montieren der ATS-Menge  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Montageaufträge** ein und wählen dann den zugehörigen Link aus.  
2.  Öffnen Sie den Montageauftrag für zehn Einheiten des Kit A.  

    Beachten Sie, dass das Feld **Montagemenge** mit der erwarteten Menge ausgefüllt wird.  

    Als Nächstes erstellen Sie ein Kommissionierungsdokument, um die benötigten Komponenten abzurufen.  

3.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Freigeben** die Option **Freigeben** aus.  
4.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Logistik** die Option **Kommissionierung erstellen** aus, und wählen Sie anschließend **OK** aus.  

    Führen Sie dann die Aufgaben des Komissionierers aus.  

5.  Wählen Sie ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben Sie **Auswahl** ein und wählen dann den zugehörigen Link aus.  
6.  Öffnen Sie den Kommissionierbeleg, den Sie in Schritt 4 in diesem Abschnitt erstellt haben.  

     Registrieren Sie dann die Kommissionierung, ohne die Standardinformationen zu ändern.  

7.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Bewegungsmenge autom. ausfüllen** aus.  
8.  Wählen Sie auf der Registerkarte **Start**, in der Gruppe **Registrierung**, die Option **Kommissionierung registrieren**.  

    Kehren Sie zum Montageauftrag zurück, um die letzte Montageaufgabe auszuführen.  

9. Wählen Sie im Fenster **Montageauftrag** auf der Registerkarte **Aktionen** in der Gruppe **Buchen** die Option **Buchen**, und klicken Sie dann auf die Schaltfläche **Ja**.  

    Beachten Sie, dass der Montageauftrag aus der Liste der offenen Aufträge entfernt wurde.  

### <a name="shipping-the-remaining-items-partly-from-stock-and-partly-assembled-to-the-order"></a>Lieferung der übrigen Artikel, teilweise aus dem Lagerbestand und teilweise nach Auftrag montiert  

1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Fibu Buchblatt** ein und wählen den zugehörenden Link aus.  
2.  Öffnen Sie den neuesten Warenausgang, der am Lagerort WHITE erstellt wurde.  

    Beachten Sie, dass in der Zeile für zehn Einheiten von Kit A das Feld **Versandmenge** und **Ausgewählte Menge** leer ist.  

    Kommissionieren Sie dann alle übrigen Artikel.  

3.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Kommissionierung erstellen** aus, und wählen Sie anschließend **OK** aus.  

    Führen Sie dann die letzte Aufgabe der Auswahl für diesen Warenausgang aus.  

4.  Wählen Sie ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben Sie **Auswahl** ein und wählen dann den zugehörigen Link aus.  
5.  Öffnen Sie den Kommissionierbeleg, den Sie in Schritt 3 in diesem Abschnitt erstellt haben.  

    Beachten Sie, dass dieser Kommissionierbeleg für Montageartikel gilt, nicht für Montagekomponenten.  

    Registrieren Sie dann die Kommissionierung, ohne die Standardinformationen zu ändern.  

6.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Bewegungsmenge autom. ausfüllen** aus.  
7.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Registrieren** die Option **Kommissionierung registrieren** aus, und klicken Sie anschließend auf die Schaltfläche **Ja**.  

    Kehren Sie zum Warenausgang zurück, um die letzte Aufgabe auszuführen.  

8.  Öffnen Sie wieder das Fenster **Warenausgangsübersicht**.  

    Beachten Sie, dass im Fenster **Lagerahausversand** in der Zeile für zehn Einheiten von Kit A die Felder **Versandmenge**und **Ausgewählte Menge** jetzt **10** enthalten.  

9. Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Buchen** die Option **Warenausgang buchen**, und wählen Sie dann die Schaltfläche **Liefern**.  

    Das Warenausgangdokument wird entfernt, was angibt, dass die entsprechenden Lageraktivitäten ausgeführt wurden. Als Nächstes überprüfen Sie, dass der Verkaufsauftrag verarbeitet wurde.  

10. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus, geben Sie **Verkaufsaufträge** ein, und wählen Sie dann den zugehörigen Link aus.  
11. Öffnen Sie den Verkaufsauftrag für The Device Shop.  

    Beachten Sie, dass das Feld **Versandte Menge** die gesamte Menge in beiden Zeilen enthält.  

    Wenn The Device Shop für den Erhalt der 18 PCs von CRONUS zahlt, werden der Verkaufsauftrag und dessen verknüpfte Montageaufträge entfernt.  

## <a name="see-also"></a>Siehe auch  
 [Auftragsmontage und Lagermontage verstehen](assembly-assemble-to-order-or-assemble-to-stock.md)   
 [Vorgehensweise: Artikel montieren](assembly-how-to-assemble-items.md)   
 [Vorgehensweise: Kommissionieren von Artikeln für den Warenausgang](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
 [Vorgehensweise: Verkaufen von Auftragsmontageartikeln](assembly-how-to-sell-items-assembled-to-order.md)   
 [Vorgehensweise: Artikel montieren](assembly-how-to-assemble-items.md)   
 [Designdetails: Montageauftragsbuchung](design-details-assembly-order-posting.md)   
 [Designdetails: Interner Lagerfluss](design-details-internal-warehouse-flows.md)   
 [Designdetails: Ausgehender Lagerfluss](design-details-outbound-warehouse-flow.md)   
 [Exemplarische Vorgehensweise: Automatische Beschaffungsplanung](walkthrough-planning-supplies-automatically.md)

