---
title: Vorgehensweise beim Korrigieren von MwSt.-Berichten
description: "Wenn Sie einen Korrektur-MwSt-Bericht übermitteln müssen oder einen übermittelten MwSt-Bericht löschen müssen, müssen Sie einen neuen MwSt-Bericht erstellen. Entsprechend der Gesetzgebung muss ein Korrekturbericht innerhalb eines Monats nach dem ursprünglichen Bericht übermittelt werden."
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
ms.openlocfilehash: fdc3e95b8877f70d346e5e6ef87d7320ffc229ac
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-correct-vat-reports"></a>Gewusst wie: Korrigieren von MwSt-Berichten
Wenn Sie einen Korrektur-MwSt-Bericht übermitteln müssen oder einen übermittelten MwSt-Bericht löschen müssen, müssen Sie einen neuen MwSt-Bericht erstellen. Entsprechend der Gesetzgebung muss ein Korrekturbericht innerhalb eines Monats nach dem ursprünglichen Bericht übermittelt werden.  

Wenn Sie einen Korrekturbericht erstellen, enthält die Erklärung zwei Zeilenarten pro korrigierter Zeile. In einer Zeilenart, „Stornierung”, wird der Basiswert der MwSt. als Stornierung aufgezeichnet. Alle anderen Informationen bleiben dieselben und können nicht bearbeitet werden. In einer neuen Zeile, Korrekturtyp, können Sie nach Bedarf Korrekturen am MwSt.-Betrag vornehmen. Bei der Aktion **Zeilen vorschlagen** wird jedoch der richtige Betrag, basierend auf den Filtern und gebuchten Belegen, vorgeschlagen. Sie können die **USt-IdNr.** nicht korrigieren oder ändern. Jede Periode, die korrigiert wird, benötigt ihren eigenen Korrekturbericht.  

Bei der Aktion **Zeilen vorschlagen**, werden die zu meldenden Werte neu berechnet. Die Aktion **Zeilen korrigieren** wird verwendet, um manuelle Änderungen vorzunehmen. Sie können die Auswirkungen der zwei Aktionen kombinieren, um den Bericht zu korrigieren.  

**Beispielkorrekturszenarien**  

1.  Wenn Sie zusätzliche MwSt-Posten buchen, nachdem Sie den Standardbericht im Berichtszeitraum übermitteln, wählen Sie **Zeilen vorschlagen** in der Gruppe **Verarbeiten** aus, um die aktualisierten Beträge zu erhalten.  

    > [!NOTE]  
    >  Wenn Sie den Betrag für einen Debitor oder Keditor manuell geändert haben, wird dieser Betrag überschrieben, wenn zusätzliche MwSt-Posten gebucht werden. Aktualisieren Sie den Betrag entsprechend.  

2.  Wenn Sie den Betrag einer Berichtszeile ändern möchten, die bereits übermittelt wurde und keine neuen MwSt-Posten gebucht werden, wählen Sie **Zeilen korrigieren** in der Gruppe Verarbeiten aus. Wählen Sie im Fenster **MwST-Berichtszeilen** die zu korrigierenden Lieferzeilen aus, und klicken Sie auf **OK**.  

    Für jeden Posten werden zwei Zeilen angezeigt: Stornierung oder Korrektur. Sie können jetzt den Betrag der Korrekturzeile ändern.  

    > [!NOTE]  
    >  Die Aktion **Zeilen korrigieren** schlägt den Betrag nicht vor, der auf MwSt-Posten basiert. Wenn Sie neue MwSt-Posten für den Debitor oder Kreditor haben, verwenden Sie stattdessen **Zeilen vorschlagen**.  

3.  Wenn Sie die falschen Filter verwendet haben, wie beispielsweise die falsche MwSt-Produktbuchungsgruppe, wählen Sie **Zeilen vorschlagen** in der Gruppe Verarbeiten aus, und legen Sie dann die Filter nach Bedarf fest.  

    **Zeilen vorschlagen** erstellt Posten, um die Differenz zwischen den Filter zu widerzuspiegeln.  

    > [!NOTE]  
    >  Wenn die aktualisierten Filter einen Debitor oder einen Kreditor ausschließen, erstellt [!INCLUDE[navnow](../../includes/navnow_md.md)] eine Stornierungszeile für den vorherigen berichteten Betrag und einen Korrekturposten mit Betrag 0.

## <a name="to-correct-a-vat-report"></a>So wird ein MwSt-Bericht korrigiert  

1.  Erstellen Sie einen neuen MwSt-Bericht. Weitere Informationen finden Sie unter [Gewusst wie: MwSt-Berichte erstellen](how-to-create-vat-reports.md).  
2.  Füllen Sie die Felder im Inforegister **Allgemein** aus, und legen Sie das Feld **MwSt-Berichtstyp** auf „Korrigiert” fest.  
3.  In der **Originalberichtsnr.** Feld, wählen Sie den Bericht aus, die Sie korrigieren möchten. Sie können nur Berichte vom Typ „Standard” auswählen, die als „Übermittelt” markiert sind.  
4.  Erstellen Sie Ihre Korrektur-MwSt-Berichts-Zeilenposten.  

    Wählen Sie die Aktion **Mahnungszeile vorschlagen**. Legen Sie die Filter gemäß Bedarf fest.  

    In jeder Zeile können Sie einen Drilldown zu den Beträgen durchführen, um anzuzeigen, aus welchen MwSt-Posten sich der Betrag zusammensetzt. Ändern Sie den Betrag nach Bedarf. Sie können die **USt-IdNr.** jedoch nicht bearbeiten.  

5.  Wenn die **Vorschlagszeilen** Aktion keine Vorschläge bietet, die Beträge zu korrigieren, die erforderlich sind, verwenden Sie die Aktion**Zeilen korrigieren**, um Stornierungs- und Korrekturzeilen für den Debitor oder Kreditor einzufügen.  
6.  Fahren Sie mit dem MwSt-Berichterstellungsprozess fort und geben Sie den Bericht frei.  

## <a name="see-also"></a>Siehe auch  
 [Vorgehensweise: Einrichten von MwSt.-Berichten](how-to-set-up-vat-reports.md)

