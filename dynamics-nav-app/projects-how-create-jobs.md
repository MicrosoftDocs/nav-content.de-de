---
title: "Erstellen Sie eine Projektkarte für ein Projekt und geben Sie Aufgaben an"
description: "Für ein neues Projekt erstellen Sie eine Projektkarte, die Projektaufgaben und enthält Planungszeilen erstellt, um Ihnen zu helfen, Status und Budgets zu verwalten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, task
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2ba145cd15e7d7e87796b159c5d4617b39ab76c7
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-jobs"></a>So wird's gemacht: Projekt erstellen
Wenn Sie mit einem neuen Projekt beginnen, müssen Sie eine Projektkarte mit integrierten Projektaufgaben und Projektplanungszeilen erstellen, strukturiert in zwei Ebenen.  

Die erste Ebene besteht aus Projektaufgaben. Sie müssen mindestens eine Projektaufgabe pro Projekt erstellen, da sich alle Buchungen auf eine Projektaufgabe beziehen. Ist für das Projekt mindestens eine Projektaufgabe vorhanden, haben Sie die Möglichkeit zum Einrichten von Planungszeilen sowie zum Buchen des Verbrauchs für das Projekt.

Die zweite Ebene besteht aus Projektplanungszeilen, die zum Angeben des genauen Verbrauchs von Ressourcen, Artikeln sowie von verschiedenen Aufwandssachposten dienen.

Durch die Ebenenstruktur lässt sich das Projekt in kleinere Aufgaben unterteilen, was wiederum eine detaillierte Budgetierung, Angebotserstellung und Erfassung ermöglicht. Außerdem gibt sie Ihnen Einblick in den Fortschritt eines Projekt. So können Sie beispielsweise nachverfolgen, ob Sie die Meilensteine erfüllen, oder ob Sie mit den erwarteten Haushaltsmitteln zurechtkommen.

> [!NOTE]  
>   Die Aktion **Neues Projekt** im Rollencenter **Projektmanager** öffnet eine unterstütze Einrichtung, die Sie durch die Schritte zur Erstellung eines Projekts mit integrierten Aufgaben und Planungszeilen führt. Nachfolgend wird beschrieben, wie Sie die Schritte manuell ausführen.

## <a name="to-create-a-job-card"></a>So erstellen Sie eine Projektkarte
Sie erstellen eine Projektkarte und erstellen dann Projektaufgabenzeilen und Projektplanungszeilen dafür.

1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Projekt** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Wählen Sie die Aktion **Neu** aus, und füllen Sie die Felder nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Um das Projekt mit Informationen über andere Projekte anzugeben, wählen Sie die Aktion **Projekt kopieren** aus und ergänzen Sie die Felder wie nötig. Wählen Sie dann die Schaltfläche **OK** aus.

> [!NOTE]  
>   Wenn Sie Arbeitszeittabellen bei Ihrem Projekt verwenden, müssen Sie auch eine verantwortliche Person angeben. Diese Person kann Arbeitszeittabellen für die Mitarbeiteraufgaben genehmigen, die dem Projekt zugeordnet sind. Weitere Informationen finden Sie unter [Vorgehensweise: Einrichten von Arbeitszeittabellen](projects-how-setup-time-sheets.md).

## <a name="to-create-tasks-for-a-job"></a>Aufgaben für ein Projekt erstellen
Beim Einrichten eines neuen Projekts ist es wichtig, auch die verschiedenen Aufgaben für das Projekt anzugeben. Dazu fügen Sie neue Zeilen im Inforegister **Aufgaben** im Fenster **Projektkarten** hinzu, jeweils eine Aufgabe pro Zeile. Jedes Objekt muss mindestens eine Aufgabe haben.

1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Projekt** ein. Wählen Sie dann den zugehörigen Link aus.
2. Öffnen Sie die Projektkarte für ein entsprechendes Projekt.
3. Füllen Sie im Inforegister **Aufgaben** die Felder nach Bedarf auf einer neuen Zeile aus.
4. Um Aufgaben einzurücken und eine Hierarchie zu erstellen, wählen Sie die Aktion **Aufgaben** und **Projektaufgaben einrücken**.
5. Wiederholen Sie die Schritte 3 und 4 für alle Aufgaben, die Sie für das Projekt benötigen.
6. Um die Projektaufgaben mit Informationen über andere Projektaufgaben anzugeben, wählen Sie die Aktion **Projektaufgaben kopieren von** aus und ergänzen Sie die Felder wie nötig. Wählen Sie dann die Schaltfläche **OK** aus.

## <a name="to-create-planning-lines-for-a-job"></a>So erstellen Sie eine Projektplanzeile für ein Projekt
Sie können Ihre neuen Projektaufgaben für Projektplanzeilen neu definieren. Mithilfe einer Planzeile lassen sich alle Informationen erfassen, die Sie für ein Projekt nachverfolgen möchten. Planzeilen können verwendet werden, um Informationen wie erforderliche Ressourcen hinzuzufügen oder um Elemente zu erfassen, die zum Ausführen des Projekts erforderlich sind. So können Sie beispielsweise eine Aufgabe zum Einholen der Zustimmung des Debitors von einem Projekt erstellen. Diese Aufgabe können Sie mit Planzeilen für Elemente verknüpfen, beispielsweise Treffen mit dem Debitor und Zuweisen von Ressourcen.  

Eine Projektplanungszeile kann von einer der folgenden Arten sein.  

| Typ | Beschreibung |
| --- | --- |
| **Budget** |Dient zum Angeben der geschätzten Verbrauchswerte und der Kosten für das Projekt, üblicherweise in einem Aufwandsvertrag. Planzeilen dieser Art können nicht fakturiert werden. |
| **Fakturierbar** |Dient zum Angeben der geschätzten Fakturierung für den Debitor, üblicherweise in einem Festpreisprojekt. |
| **Sowohl budgetiert und verrechenbar** |Dient zum Angeben des geplanten Verbrauchs, der dem zu fakturierenden Wert entspricht. |

**Hinweis**. Beim Hinzufügen von Informationen in der Projektplanungszeilen werden die Kosteninformationen automatisch ergänzt. Wenn Sie also beispielsweise eine neue Zeile eingeben, basieren Kosten, Preis und Skonto für Ressourcen und Artikel zunächst auf den Informationen, die auf den Ressourcen- und Artikelkarten angegeben sind.

1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Projekt** ein. Wählen Sie dann den zugehörigen Link aus.
2. Eine relevante Projektkarte öffnen.
3. Wählen Sie eine Projektaufgabe aus, deren Wert für das Feld **Projektaufgabenart** **Buchen** enthält und klicken Sie anschließend auf die Aktion **Projektplanzeilen**.  
4. Auf einer neuen Zeile im Fenster **Projektplanungszeilen** füllen Sie die Felder nach Bedarf aus.
5. Wiederholen Sie die Schritte 3 und 4 für alle Planungszeilen für diese Projektaufgabe.

## <a name="see-also"></a>Siehe auch
[Projektmanagement](projects-manage-projects.md)  
[Finanzen](finance.md)  
[Einkauf](purchasing-manage-purchasing.md)         
[Verkauf](sales-manage-sales.md)      
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

