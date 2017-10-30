---
title: "Gewusst wie: Buchen von Inventuraufträgen"
description: "Nach Fertigstellen eines Inventurauftrags und Ändern des Status in **Beendet** kann er gebucht werden."
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
ms.openlocfilehash: 70da79ae7a6731b705178905655b09b6e9a8ff30
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-physical-inventory-orders"></a>Gewusst wie: Buchen von Inventuraufträgen
Nach Fertigstellen eines Inventurauftrags und Ändern des Status in **Beendet** kann er gebucht werden.  
  
 Der Status eines Inventurauftrags kann unter folgenden Voraussetzungen auf **Beendet** festgelegt werden:  
  
-   Alle zugehörigen Inventurerfassungen weisen den Status **Beendet** auf.  
  
-   Jede Inventurauftragszeile wurde in mindestens einer Inventurerfassungszeile erfasst.  
  
-   Die Kontrollkästchen **In Erfassungszeilen enthalten** und **Berechnete erw. Menge** wurden für alle Inventurauftragszeilen aktiviert.  
  
 Nach dem Buchen des Auftrags können die gebuchten Inventuraufträge angezeigt werden. Gebuchte Lagerbelege bieten einen vollständigen Überblick über den Inventurprozess.  
  
### <a name="to-post-a-physical-inventory-order"></a>So buchen Sie einen Inventurauftrag  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”"), geben Sie **Bestandsauftrag** ein, und wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie den Inventurauftrag aus, für den Sie eine Inventurerfassung erstellen möchten, klicken Sie auf **Startseite** und anschließend auf **Bearbeiten**.  
  
     Im Fenster **Inventurauftrag** kann die Menge angezeigt werden, die nach Ausführung der Inventur im Feld **Erfasste Menge (Basis)** erfasst wurde.  
  
3.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **Beenden** aus.  
  
4.  Wählen Sie die Schaltfläche **Ja** aus. Der Wert im Feld **Status** wird in **Beendet** geändert.  
  
    > [!NOTE]  
    >  Eine Änderung des Inventurauftragskopfs oder der Inventurauftragszeilen ist nicht möglich.  
  
5.  Wählen Sie die zu buchenden Zeilen aus, und wählen Sie dann die Aktion **Buchen** und dann **ok** aus.  
  
### <a name="to-view-posted-physical-inventory-orders"></a>So zeigen Sie gebuchte Inventuraufträge an  
  
1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Physische Inventur durchführen** ein. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie im Fenster **Gebuchter Inventurauftrag** den gebuchten Inventurauftrag aus, den Sie anzeigen möchten, klicken Sie auf **Startseite** und anschließend auf **Ansicht**.  
  
3.  Um einer Liste zugehöriger Inventurerfassungen auf der Registerkarte anzuzeigen, gehen Sie auf der Registerkarte **Navigieren** in der Gruppe **Auftrag** auf **Erfassungen**.  
  
     Sie können auch einen Bericht ausführen, in dem die Differenz zwischen der erwarteten Menge und der erfassten Menge zurückgegeben wird.  
  
4.  Schließen Sie das Fenster.  
  
## <a name="see-also"></a>Siehe auch  
 [Inventurbelege](physical-inventory-documents.md)   
 [Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md)
