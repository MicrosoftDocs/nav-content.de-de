---
title: "Vorgehensweise: Kommissionierung für interne Arbeitsgänge in erweiterter Lagerkonfigurationen"
description: "In der erweiterten Lagerkonfigurationen, in der der Lagerort für Kommissionierung und Lieferung eingerichtet wurde, können Sie Komponenten für Produktions- und Montageaktivitäten im Fenster **Kommissionierung** kommissionieren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 08b79f573a9fc013068f7e1f5dd593a596a579a3
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-pick-for-assembly-or-production-in-advanced-warehouse-configurations"></a>Vorgehensweise: Kommissionierung für Montage oder Produktion in erweiterter Lagerkonfiguration
In der erweiterten Lagerkonfigurationen, in der der Lagerort für Kommissionierung und Lieferung eingerichtet wurde, können Sie Komponenten für Produktions- und Montageaktivitäten im Fenster **Kommissionierung** kommissionieren.  

Alternativ können Sie das Fenster **Lagerplatzumlagerungsvorschlag** verwenden, um die Artikel ohne Bezug zu einem Herkunftsbeleg zwischen Lagerplätzen ad hoc zu verschieben. Weitere Informationen finden Sie unter [Vorgehensweise: Umlagern von Artikeln in erweiterten Lagerkonfigurationen](warehouse-how-to-move-items-in-advanced-warehousing.md).  

Allgemeine Informationen über das Kommissionieren von Artikeln für interne Arbeitsgänge an den Basislagerorten, die ausschließlich für die Kommissionierung eingerichtet sind, finden Sie unter [Vorgehensweise: Umlagern von Komponenten in einen Arbeitsgangbereich in den Basis-Lagerkonfigurationen](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  

Sie können einen Kommissionierungsbeleg nicht von Grund auf neu erstellen, da eine Kommissionierungsaktivität immer Teil eines Workflows ist, entweder in einem Abruf- oder Push-Szenario.  

Sie können den Kommissionierungsbeleg Push-artig erstellen, indem Sie im Herkunftsbeleg, wie einem freigegebenen Montageauftrag oder einem Warenausgang, **Kommissionierung erstellen** auswählen. Weitere Informationen finden Sie unter [Vorgehensweise: Entnahme von Artikeln mit Kommissionierungen](warehouse-how-to-pick-items-for-warehouse-shipment.md).  

Alternativ können Sie den Kommissionierungsbeleg abrufartig erstellen, indem Sie das Fenster **Kommissioniervorschlag** verwenden, um Kommissionieranforderungen für den Warenausgang und für interne Arbeitsgänge zu ermitteln, und dann die erforderlichen Kommissionierungsbelege zu erstellen.  

Nachfolgend wird ein Abrufszenario beschrieben, in dem Sie Komponenten für einen freigegebenen FA über das Fenster **Kommissioniervorschlag** kommissionieren. Das Verfahren gilt auch für einen Montageauftrag.  

Um Kommissionieranforderungen zu erstellen, müssen für Abruf- und Push-Szenarien die betreffenden Herkunftsbelege freigegeben werden. Die Freigabe von Herkunftsbelegen für interne Arbeitsgänge geschieht auf die folgenden Arten.  

|Herkunftsbeleg|Freigabeverfahren|  
|---------------------|--------------------|  
|Fertigungsauftrag|Änderung des Auftragstyps in einen freigegebenen Fertigungsauftrag.|  
|Montageauftrag|Änderung des Status in "Freigegeben".|  

## <a name="to-pick-components-using-the-pick-worksheet"></a>So kommissionieren Sie Komponenten vom Kommissioniervorschlag aus:  
1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen] Symbol (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Kommissioniervorschlag** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Aktion **Logistikbeleg holen** aus, und wählen Sie anschließend die Komponentenzeilen des freigegebenen Fertigungsauftrags aus.  
3.  Prüfen Sie die Zeilen, sortieren Sie sie so, dass sie eine effiziente Kommissionierrunde ergeben, und kombinieren Sie sie, falls erforderlich, mit anderen Kommissionierzeilen, um die Arbeitszeit der Mitarbeiter bestmöglich zu nutzen.  
4.  Wählen Sie die Aktion **Kommissionierung erstellen** aus.  
5.  Legen Sie fest, wie die Kommissionierungsbelege erstellt und wie Kommissionierzeilen sortiert werden, indem Sie die Felder im Fenster **Kommissionierung erstellen** ausfüllen.  
6.  Wählen Sie die Schaltfläche **OK** aus. Kommissionierungsbelege werden mit Kommissionierzeilen für jede Komponente erstellt, die im internen Arbeitsgang erforderlich ist.  

Wenn der interne Vorgangsbereich, wie ein Produktionsfertigungsbereich, mit einem Lagerplatz eingerichtet ist, der für die Lagerung von Komponenten für den Arbeitsgang verwendet wird, dann wird dieser Lagerplatzcode in die Einlagerungszeilen des Kommissionierungsbelegs eingefügt, der Lagermitarbeiter anweist, wo sie die Artikel einlagern sollen. Weitere Informationen finden Sie im Feld **Fert.-Bereitst.-Lagerplatzcode** oder **Mont.-Bereitst.-Lagerplatzcode**.

## <a name="filling-the-consumption-bin"></a>Auffüllen des Verbrauchslagerplatzes
Dieses Flussdiagramm zeigt, wie das Feld **Lagerplatzcode** in FA-Komponentenzeilen entsprechend Ihrer Einrichtung ausgefüllt wird.

![Lagerplatz-Flussdiagramm](media/binflow.png "Lagerfluss")  

## <a name="see-also"></a>Siehe auch
[Logistik](warehouse-manage-warehouse.md)  
[Lagerbest](inventory-manage-inventory.md)  
[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)     
[Montageverwaltung](assembly-assemble-items.md)    
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

