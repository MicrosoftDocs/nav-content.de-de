---
title: "Ausgleichen und ändern Sie Einstellungen in gespeicherten Berichten"
description: Beschreibt vordefinierte Optionen und filtert, um einen Bericht anzupassen und die richtigen Daten zu generieren.
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 09/08/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c63b5585f724a60007e836ab06333798bce65129
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="managing-saved-settings-on-reports"></a>Gespeicherte Einstellungen in Berichtenn verwalten
Abhängig vom Bericht, der bearbeitet wird, erhalten Sie möglicherweise eine Seite, für die Sie bestimmte Optionen festlegen und filtern können, um Daten zu ändern, die im erstellten Bericht enthalten sind. Diese Seite ist die Berichtanfordearungsseite. Ein Bericht kann eine oder mehrere *Gespeicherte Einstellungen* enthalten, die Sie auf den Bericht von der Anforderungsseite anwenden können. *Gespeicherte Einstellungen* sind grundsätzlich vordefinierte Optionen und Filter. Die Verwendung von gespeicherten Einstellungen ist eine schnelle und zuverlässige Art, Berichte zu erstellen, die die richtigen Daten enthalten.

Sie können die gespeicherten Einstellungen sehen, die Ihnen für einen Bericht zur Verfügung stehen im Abschnitt **Gespeicherte Einstellungen** auf der Berichtsanforderungsseite.  

## <a name="to-apply-saved-settings-to-a-report"></a>Um gespeicherte Einstellungen auf einen Bericht anzuwenden
1. Den Bericht öffnen.

   Die Berichtanforderungsseite wird angezeigt.    
2. Im Abschnitt **Gespeicherte Einstellungen** legen Sie das Feld **Name** für die gespeicherten Einstellungenfest, die Sie verwenden möchten.

   Der Abschnitt **Gespeicherte Einstellungen** wird nur angezeigt, wenn der Bericht zuvor ausgeführt wurde, oder wenn es vorhandene gespeicherte Einstellungseinträge gibt. Der gespeicherte Einstellungseintrag mit der Bezeichnung **Zuletzt verwendete Optionen und Filter** ist immer verfügbar. Diese Einstellungen sind die die Option und die Filterwerte, die bei der letzten Berichterstellung verwendet wurden.

## <a name="administer-saved-report-settings-for-users"></a>Verwalten von gespeicherten Berichtseinstellungen für Benutzer
Wenn Sie die richtigen Berechtigungen haben, können Sie die gespeicherten Einstellungen für alle Berichte für alle Benutzer im Unternehmen anzeigen, erstellen und bearbeiten. Sie können gespeicherte Einstellungen für einen Bericht den einzelnen Benutzern oder allen Benutzern im Unternehmen zuweisen.

Sie können gespeicherte Einstellungen der Seite 1506 **Berichteinstellungen** verwalten. Um diese Seite zu öffnen, wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen")und geben **Berichtseinstellungen** ein. Wählen Sie dann den zugehörigen Link aus.

Von der Seite **Berichteinstellungen** können Sie neue Einstellungen von Grund auf erstellen oder Sie können bestehende Einstellungen kopieren oder bearbeiten. Um die Optionen und Filter für Einstellungen zu ändern, wählen Sie die Aktion **Bearbeiten**.

> [!NOTE]
> Die Funktion für gespeicherte Einstellungen in Berichten ist nur relevant, wenn die SaveValues-Eigenschaft der Anforderungsseite auf "Ja" festgelegt ist. Die SaveValues-Eigenschafteneigenschaft wird in der Entwicklungsumgebung festgelegt.  

> [!Important]
> Wenn Sie einen gespeicherten Einstellungsartikel für alle Benutzer erstellen und er denselben Namen wie bestehende gespeicherte Einstellungen für einen bestimmten Benutzer hat, ist dieser Benutzer nicht dazu in der Lage sein, die gespeicherten Einstellungen zu verwenden, die jedem zugeordnet sind.  Im Feld „Gespeicherte Einstellungen” auf der Berichtsanforderungsseite werden dem Benutzer auch zwei Optionen gespeicherter Einstellungen mit demselben Namen angezeigt. Jedoch gleichgültig welche Option er wählt, werden die benutzerspezifischen gespeicherten Einstellungen verwendet.

## <a name="see-also"></a>Siehe auch
[Arbeiten mit Berichten](ui-work-report.md)  

