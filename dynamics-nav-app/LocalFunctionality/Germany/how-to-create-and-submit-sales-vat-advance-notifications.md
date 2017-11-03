---
title: Vorgehensweise beim Erstellen und Senden von Umsatzsteuervoranmeldungen
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln. Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben."
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
ms.openlocfilehash: e730b9e00f689cf4e42a8ff2e0a8d332ccc700d7
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-and-submit-sales-vat-advance-notifications"></a><span data-ttu-id="17818-104">Gewusst wie: Erstellen und Senden von Umsatzsteuervoranmeldungen</span><span class="sxs-lookup"><span data-stu-id="17818-104">How to: Create and Submit Sales VAT Advance Notifications</span></span>
<span data-ttu-id="17818-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln.</span><span class="sxs-lookup"><span data-stu-id="17818-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can submit the sales VAT advance notification file electronically to the ELSTER portal.</span></span> <span data-ttu-id="17818-106">Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben.</span><span class="sxs-lookup"><span data-stu-id="17818-106">You can transmit the sales VAT advance notification file to the tax authorities after you have verified the calculated tax amount and the base amount.</span></span>  

## <a name="to-create-an-xml-document-for-sales-vat-advance-notification"></a><span data-ttu-id="17818-107">So erstellen Sie ein XML-Dokument für Umsatzsteuervoranmeldung</span><span class="sxs-lookup"><span data-stu-id="17818-107">To create an XML document for sales VAT advance notification</span></span>  

1.  <span data-ttu-id="17818-108">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”") aus, und geben Sie **Umsatzsteuervoranmeldungsliste** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="17818-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Vat Advanced Notification List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="17818-109">Im Fenster **Umsatzsteuervoranmeldungsliste** auf der Registerkarte Aktionen, wählen Sie **Neu** aus.</span><span class="sxs-lookup"><span data-stu-id="17818-109">In the **Sales Vat Advanced Notification List** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="17818-110">Füllen Sie im Fenster **USt.-Voranmeldungskarte** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="17818-110">In the **Sales VAT Adv. Notif. Card** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="17818-111">Feld</span><span class="sxs-lookup"><span data-stu-id="17818-111">Field</span></span>|<span data-ttu-id="17818-112">Description</span><span class="sxs-lookup"><span data-stu-id="17818-112">Description</span></span>|  
    |------------------------------------|---------------------------------------|  
    |<span data-ttu-id="17818-113">**Ansprechpartner für Finanzamt**</span><span class="sxs-lookup"><span data-stu-id="17818-113">**Contact for Tax Office**</span></span>|<span data-ttu-id="17818-114">Die Kontaktperson für das Finanzamt in Ihrer Organisation.</span><span class="sxs-lookup"><span data-stu-id="17818-114">The contact person for the tax office in your organization.</span></span>|  
    |<span data-ttu-id="17818-115">**Telefonnummer Kontakt**</span><span class="sxs-lookup"><span data-stu-id="17818-115">**Contact Phone No.**</span></span>|<span data-ttu-id="17818-116">Telefonnummer der Kontaktperson.</span><span class="sxs-lookup"><span data-stu-id="17818-116">The contact person's telephone number.</span></span>|  
    |<span data-ttu-id="17818-117">**Kontakt-E-Mail**</span><span class="sxs-lookup"><span data-stu-id="17818-117">**Contact E-Mail**</span></span>|<span data-ttu-id="17818-118">E-Mail-Adresse der Kontaktperson.</span><span class="sxs-lookup"><span data-stu-id="17818-118">The contact person's email address.</span></span>|  

5.  <span data-ttu-id="17818-119">Wählen Sie die Aktion **XML-Datei erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="17818-119">Choose the **Create XML-File** action.</span></span>  
6.  <span data-ttu-id="17818-120">Im Batchauftrag **MwSt.-Voranmeldung erstellen** im Inforegister **Optionen**, im Feld **XML-Datei**, wählen Sie **Erstellen** oder **Erstellen und anzeigen** aus.</span><span class="sxs-lookup"><span data-stu-id="17818-120">In the **Create Sales VAT Adv. Notif.** batch job, on the **Options** FastTab, in the **XML-File** field, select the **Create** or the **Create and Show** option.</span></span>  
7.  <span data-ttu-id="17818-121">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="17818-121">Choose the **OK** button.</span></span>  

## <a name="to-submit-an-xml-document-for-sales-vat-advance-notification"></a><span data-ttu-id="17818-122">So übermitteln Sie ein XML-Dokument für Umsatzsteuervoranmeldung</span><span class="sxs-lookup"><span data-stu-id="17818-122">To submit an XML document for sales VAT advance notification</span></span>  

1.  <span data-ttu-id="17818-123">Im Fenster **Umsatzsteuervoranmeldungsliste** wählen Sie den Beleg aus, den Sie an ELSTER senden möchten.</span><span class="sxs-lookup"><span data-stu-id="17818-123">In the **Sales VAT Advance Notification List** window, select the document that you want to submit to ELSTER.</span></span>  
2.  <span data-ttu-id="17818-124">Wählen Sie die Aktion **XML-Datei übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="17818-124">Choose the **Transmit XML-File** action.</span></span>  

<span data-ttu-id="17818-125">Die XML-Datei wird an ELSTER übermittelt.</span><span class="sxs-lookup"><span data-stu-id="17818-125">The XML file is transmitted to ELSTER.</span></span>  

## <a name="see-also"></a><span data-ttu-id="17818-126">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="17818-126">See Also</span></span>  
 <span data-ttu-id="17818-127">[Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md) </span><span class="sxs-lookup"><span data-stu-id="17818-127">[Electronic Submission of Sales VAT Advance Notifications to ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md) </span></span>  
 [<span data-ttu-id="17818-128">Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER</span><span class="sxs-lookup"><span data-stu-id="17818-128">How to: Set Up Sales VAT Advance Notifications for ELSTER</span></span>](how-to-set-up-sales-vat-advance-notifications-for-elster.md)

