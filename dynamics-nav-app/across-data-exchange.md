---
title: Elektronische Belege in Dynamics NAV
description: "Einführung zum Senden und Empfangen von elektronischen Belegen in [!INCLUDE[d365fin](includes/d365fin_md.md)]."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/19/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5459a76797a948555a6a20009d57de96fe9eec7f
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="exchanging-data-electronically"></a><span data-ttu-id="e153b-103">Daten elektronisch austauschen</span><span class="sxs-lookup"><span data-stu-id="e153b-103">Exchanging Data Electronically</span></span>
<span data-ttu-id="e153b-104">Sie können das Datenaustauschframework verwenden, um Geschäftsbelege, Bankdateien, Währungswechselkurse und andere Datendateien mit Ihren Geschäftspartnern auszutauschen.</span><span class="sxs-lookup"><span data-stu-id="e153b-104">You can use the Data Exchange Framework to exchange business documents, bank files, currency exchange rates, and any other data files with your business partners.</span></span>

## <a name="electronic-documents"></a><span data-ttu-id="e153b-105">Elektronische Belege</span><span class="sxs-lookup"><span data-stu-id="e153b-105">Electronic Documents</span></span>
<span data-ttu-id="e153b-106">Als Alternative zu E-Mail-Dateianhängen können Sie Geschäftsbelegen elektronisch versenden und empfangen.</span><span class="sxs-lookup"><span data-stu-id="e153b-106">As an alternative to emailing as file attachments, you can send and receive business documents electronically.</span></span> <span data-ttu-id="e153b-107">Mit elektronischem Beleg ist eine normgerechte Datei gemeint, die ein Geschäftsdokument darstellt, zum Beispiel eine Rechnung von einem Kreditor, die Sie in [!INCLUDE[d365fin](includes/d365fin_md.md)] empfangen und in eine Einkaufsrechnung konvertieren können.</span><span class="sxs-lookup"><span data-stu-id="e153b-107">By electronic document is meant a standard-compliant file representing a business document, such as an invoice from a vendor that you can receive and convert to a purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)] .</span></span> <span data-ttu-id="e153b-108">Der Austausch von elektronischen Belegen zwischen zwei Handelspartnern erfolgt über einen externen Anbieter eines Belegaustauschdiensts.</span><span class="sxs-lookup"><span data-stu-id="e153b-108">The exchange of electronic documents between two trading partners is performed by an external provider of document exchange services.</span></span> <span data-ttu-id="e153b-109">Die allgemeine Version von [!INCLUDE[d365fin](includes/d365fin_md.md)]  unterstützt das Senden und Empfangen von elektronischen Rechnungen und Gutschriften im PEPPOL-Format, das von den größten Anbietern von Belegaustauschdiensten unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="e153b-109">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)]  supports sending and receiving electronic invoices and credit memos in the PEPPOL format, which is supported by the largest providers of document exchange services.</span></span> <span data-ttu-id="e153b-110">Ein wichtiger Anbieter eines Belegaustauschdienstes ist vorkonfiguriert und kann für Ihren Mandanten eingerichtet werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-110">A major provider of document exchange services is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="e153b-111">Um Unterstützung für andere elektronische Belegformate zu bieten, müssen Sie mithilfe des Datenaustauschframework neue Datenaustauschdefinitionen erstellen.</span><span class="sxs-lookup"><span data-stu-id="e153b-111">To provide support for other electronic document formats, you must create new date exchange definitions using the Data Exchange Framework.</span></span>  

<span data-ttu-id="e153b-112">Mithilfe eines externen OCR-Dienstes (optische Zeichenerkennung) können Sie aus PDF- oder Bilddateien, die die Eingangsbelege darstellen, elektronische Belege erstellen, die Sie dann in [!INCLUDE[d365fin](includes/d365fin_md.md)] in Belegdatensätze konvertieren können, wie Sie es für elektronische PEPPOL-Belege tun.</span><span class="sxs-lookup"><span data-stu-id="e153b-112">From PDF or image files representing incoming documents, you can have an external OCR service (Optical Character Recognition) create electronic documents that you can then convert to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)], like for electronic PEPPOL documents.</span></span> <span data-ttu-id="e153b-113">Wenn Sie beispielsweise eine Rechnung in PDF-Format von Ihrem Kreditor erhalten, können Sie diese über das Fenster **Eingehende Belege** zum OCR-Dienst senden.</span><span class="sxs-lookup"><span data-stu-id="e153b-113">For example, when you receive an invoice in PDF format from your vendor, you can send it to the OCR service from the **Incoming Documents** window.</span></span> <span data-ttu-id="e153b-114">Nach einigen Sekunden erhalten Sie die Datei als elektronische Rechnung zurück, die zu einer Einkaufsrechnung für den Kreditor umgewandelt werden kann.</span><span class="sxs-lookup"><span data-stu-id="e153b-114">After a few seconds, you receive the file back as an electronic invoice that can be converted to a purchase invoice for the vendor.</span></span> <span data-ttu-id="e153b-115">Wenn Sie die Datei per E-Mail an den OCR-Service senden, wird automatisch ein neuer Datensatz für einen eingehenden elektronischen Beleg erstellt, wenn Sie den elektronischen Belegs zurückerhalten.</span><span class="sxs-lookup"><span data-stu-id="e153b-115">If you send the file to the OCR service by email, then a new incoming document record is automatically created when you receive the electronic document back.</span></span>  

<span data-ttu-id="e153b-116">Um beispielsweise Verkaufsrechnungen als elektronischer PEPPOL-Beleg zu senden, wählen Sie die Option **Elektronisches Dokument** im **Buchen und senden**-Dialogfeld aus.</span><span class="sxs-lookup"><span data-stu-id="e153b-116">To send, for example, a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box.</span></span> <span data-ttu-id="e153b-117">Dort können Sie außerdem das standardmäßige Belegsendeprofil für den Debitor einrichten.</span><span class="sxs-lookup"><span data-stu-id="e153b-117">From here, you can also set up the customer’s default document sending profile.</span></span> <span data-ttu-id="e153b-118">Zuerst müssen Sie verschiedene Stammdaten einrichten, zum Beispiel Mandantendaten, Debitoren, Artikel und Maßeinheiten.</span><span class="sxs-lookup"><span data-stu-id="e153b-118">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="e153b-119">Diese werden verwendet, um Geschäftspartner und Artikel beim Konvertieren von Daten in Feldern in [!INCLUDE[d365fin](includes/d365fin_md.md)]  in Elemente der ausgehenden Dokumentdatei zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="e153b-119">These are used to identify the business partners and items when you convert data in fields in [!INCLUDE[d365fin](includes/d365fin_md.md)]  to elements in the outgoing document file.</span></span> <span data-ttu-id="e153b-120">Die Datenkonvertierung und das Senden der PEPPOL-Verkaufsrechnung werden durch dedizierte Codeunits und XMLports ausgeführt, die im elektronischen Belegformat **PEPPOL** dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-120">The data conversion and sending of the PEPPOL sales invoice are performed by dedicated codeunits and XMLports, represented by the **PEPPOL** electronic document format.</span></span>  

<span data-ttu-id="e153b-121">Um beispielsweise eine Rechnung von einem Kreditor in Form eines elektronischen PEPPOL-Belegs zu erhalten, verarbeiten Sie den Beleg im Fenster **Eingehende Dokumente**, um ihn in eine Einkaufsrechnung in [!INCLUDE[d365fin](includes/d365fin_md.md)] zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="e153b-121">To receive, for example, an invoice from a vendor as an electronic PEPPOL document, you process the document in the **Incoming Documents** window to convert it to a purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e153b-122">Sie können entweder die Auftragswarteschlange zur regelmäßigen Verarbeitung solcher Dateien einrichten, oder Sie können den Vorgang manuell starten.</span><span class="sxs-lookup"><span data-stu-id="e153b-122">You can either set up the Job Queue feature to process such files regularly or you can start the process manually.</span></span> <span data-ttu-id="e153b-123">Zuerst müssen Sie verschiedene Stammdaten einrichten, zum Beispiel Mandantendaten, Kreditoren, Artikel und Maßeinheiten.</span><span class="sxs-lookup"><span data-stu-id="e153b-123">First, you must set up various master data, such as company information, vendors, items, and units of measure.</span></span> <span data-ttu-id="e153b-124">Diese werden verwendet, um Geschäftspartner und Artikel zu identifizieren, wenn Daten in Elementen im Eingangsbeleg zu Feldern in [!INCLUDE[d365fin](includes/d365fin_md.md)] konvertiert werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-124">These are used to identify the business partners and items when you convert data in elements in the incoming document file to fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e153b-125">Der Empfang und die Datenkonvertierung von PEPPOL-Rechnungen erfolgen über das Datenaustauschframework, das durch die Datenaustauschdefinition **PEPPOL - Rechnung** dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="e153b-125">The receiving and data conversion of PEPPOL invoices are performed by the Data Exchange Framework, represented by the **PEPPOL - Invoice** data exchange definition.</span></span>  

 <span data-ttu-id="e153b-126">Um zum Beispiel eine Rechnung als elektronischer OCR-Beleg zu empfangen, verarbeiten Sie diese genauso wie beim Empfang eines elektronischen PEPPOL-Belegs.</span><span class="sxs-lookup"><span data-stu-id="e153b-126">To receive, for example, an invoice as an electronic OCR document, you process it as when you receive an electronic PEPPOL document.</span></span> <span data-ttu-id="e153b-127">Der Empfang und die Konvertierung von elektronischen Belegen von OCR wird über das Datenaustauschframework durchgeführt, das durch die Datenaustauschdefinition **OCR - Rechnung** dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="e153b-127">The receiving and conversion of electronic documents from OCR are performed by the Data Exchange Framework, represented by the **OCR – Invoice** data exchange definition.</span></span>  

## <a name="bank-files"></a><span data-ttu-id="e153b-128">Bankdateien</span><span class="sxs-lookup"><span data-stu-id="e153b-128">Bank Files</span></span>  
 <span data-ttu-id="e153b-129">Die Formate der Dateien für den Austausch von Bankdaten mit ERP-Systemen variieren abhängig vom Lieferanten der Datei und vom jeweiligen Land oder der Region.</span><span class="sxs-lookup"><span data-stu-id="e153b-129">The formats of files for exchange of bank data with ERP systems vary depending on the supplier of the file and on the country/region.</span></span> <span data-ttu-id="e153b-130">Die allgemeine Version von [!INCLUDE[d365fin](includes/d365fin_md.md)]  unterstützt den Import und Export von SEPA-Bankdateien (Single Euro Payments Area; einheitlicher Euro-Zahlungsverkehrsraum) und einen Bankdaten-Konvertierungsdienst, der vom externen Anbieter AMC Consult bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="e153b-130">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)]  supports import and export of SEPA bank files (Single Euro Payments Area) and a bank data conversion service provided by external provider, AMC Consult.</span></span> <span data-ttu-id="e153b-131">Um Unterstützung für andere elektronische Belegformate zu bieten, verwenden Sie das Datenaustauschframework.</span><span class="sxs-lookup"><span data-stu-id="e153b-131">To provide support for other electronic document formats, you use the Data Exchange Framework.</span></span>  

<span data-ttu-id="e153b-132">Um SEPA-Gutschriftübertragungen zu exportieren, wählen Sie die Schaltfläche **Zahlungen in Datei exportieren** im Fenster **Zahlungs-Buch-Blatt.** aus und laden die Datei dann hoch, um die Zahlungen bei Ihrer Bank in Auftrag zu geben.</span><span class="sxs-lookup"><span data-stu-id="e153b-132">To export SEPA credit transfers, you choose **Export Payments to File** button in the **Payment Journal** window and then upload the file to process the payments in your bank.</span></span> <span data-ttu-id="e153b-133">Zuerst müssen Sie verschiedene Stammdaten einrichten, wie Bankkonto, Kreditoren und Zahlungsformen.</span><span class="sxs-lookup"><span data-stu-id="e153b-133">First you must set up various master data, such as bank account, vendors, and payment methods.</span></span> <span data-ttu-id="e153b-134">Die Datenkonvertierung und der Export von SEPA-Bankdaten werden durch dedizierte Codeunits und XMLports ausgeführt, die durch das Bankexport-/-importsetup **SEPA Kreditübertragung** dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-134">The data conversion and export of SEPA bank data is performed by a dedicated codeunit and XMLport, represented by the **SEPA Credit Transfer** bank export/import setup.</span></span> <span data-ttu-id="e153b-135">Alternativ können Sie den Bankdaten-Konvertierungsdienst so einrichten, dass er den Export ausführt. Dies wird durch die Datenaustauschdefinition **Bankdaten-Konvertierungsdienst - Kreditübertragung** dargestellt.</span><span class="sxs-lookup"><span data-stu-id="e153b-135">Alternatively, you can set up the bank data conversion service to perform the export, represented by the **Bank Data Conversion Service - Credit Transfer** data exchange definition.</span></span>  

<span data-ttu-id="e153b-136">Um SEPA-Lastschriften zu exportieren, wählen Sie die Schaltfläche **Lastschriftdatei exportieren** im Fenster **Lastschrift** aus und senden die Datei dann zu Ihrer Bank, damit die entsprechenden Debitorenzahlungen automatisch erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-136">To export SEPA direct debit instructions, you choose the **Export Direct Debit File** button in the **Direct Debit Collections** window and then send to your bank to automatically collect the involved customer payments.</span></span> <span data-ttu-id="e153b-137">Zuerst müssen Sie Bankkonten, Debitoren, Lastschrift-Mandage und Zahlungsformen einrichten.</span><span class="sxs-lookup"><span data-stu-id="e153b-137">First you must set up bank accounts, customers, direct-debit mandates, and payment methods.</span></span> <span data-ttu-id="e153b-138">Die Datenkonvertierung und der Export von SEPA-Bankdaten werden durch dedizierte Codeunits und XMLports ausgeführt, die durch das **SEPA-Lastschrift** Bankexport-/-importsetup dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-138">The data conversion and export of SEPA bank data is performed by dedicated a codeunit and XMLport, represented by the **SEPA Direct Debit** bank export/import setup.</span></span>  

<span data-ttu-id="e153b-139">Um SEPA-Bankauszüge zu importieren, wählen Sie die Schaltfläche "Bankauszug importieren" in den Fenstern **Zahlungsabstimmungsbuch.-Blatt** und **Bankkonto-Abstimmung** aus. Gleichen Sie dann die einzelnen Bankkontoauszugsposten manuell oder automatisch mit Zahlungen der Bankposten aus.</span><span class="sxs-lookup"><span data-stu-id="e153b-139">To import SEPA bank statements, you choose the Import Bank Statement button in the **Payment Reconciliation Journal** and **Bank Acc. Reconciliation** windows and then you proceed to apply each bank statement entry to payments or bank ledger entries, manually or automatically.</span></span> <span data-ttu-id="e153b-140">Zuerst müssen Sie Bankkonten einrichten.</span><span class="sxs-lookup"><span data-stu-id="e153b-140">First you must set up bank accounts.</span></span> <span data-ttu-id="e153b-141">Der Import und die Datenkonvertierung von SEPA-Bankdaten erfolgen über das Datenaustauschframework, das durch die Datenaustauschdefinition **SEPA CAMT** dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="e153b-141">The import and data conversion of SEPA bank data is performed by the Data Exchange Framework, represented by the **SEPA CAMT** data exchange definition.</span></span> <span data-ttu-id="e153b-142">Alternativ können Sie den Bankdaten-Konvertierungsdienst so einrichten, dass er den Import ausführt. Dies wird durch die Datenaustauschdefinition **Bankdaten-Konvertierungsdienst – Bankauszug** dargestellt.</span><span class="sxs-lookup"><span data-stu-id="e153b-142">Alternatively, you can set up the bank data conversion service to perform the import, represented by the **Bank Data Conversion Service – Bank Statement** data exchange definition.</span></span>  

 <span data-ttu-id="e153b-143">Darüber hinaus unterstützen die lokalen Versionen von [!INCLUDE[d365fin](includes/d365fin_md.md)] verschiedene andere Dateiformate für den Import und Export von Bankdaten, Lohntransaktionen und anderen Daten.</span><span class="sxs-lookup"><span data-stu-id="e153b-143">In addition, the local versions of [!INCLUDE[d365fin](includes/d365fin_md.md)] support various other file formats for import/export of bank data, payroll transactions, and other data.</span></span> <span data-ttu-id="e153b-144">Weitere Informationen finden Sie im Abschnitt „Lokale Funktion“ in der Version von [!INCLUDE[d365fin](includes/d365fin_md.md)] für Ihr Land.</span><span class="sxs-lookup"><span data-stu-id="e153b-144">For more information, see the “Local Functionality” Help section in your country version of [!INCLUDE[d365fin](includes/d365fin_md.md)] .</span></span>  

## <a name="currency-exchange-rates"></a><span data-ttu-id="e153b-145">Währungswechselkurse</span><span class="sxs-lookup"><span data-stu-id="e153b-145">Currency Exchange Rates</span></span>  
<span data-ttu-id="e153b-146">Sie können einen externen Service einrichten, um Ihre Währungswechselkurses auf dem neuesten Stand zu halten.</span><span class="sxs-lookup"><span data-stu-id="e153b-146">You can set up an external service to keep your for currency exchange rates up to date.</span></span> <span data-ttu-id="e153b-147">Der Service, der aktualisierte Währungswechselkurses bereitstellt, wird durch eine Datenaustauschdefinition aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e153b-147">The service that provides updated currency exchange rates is enabled by a data exchange definition.</span></span> <span data-ttu-id="e153b-148">Entsprechend wird das **Wechselkursaktualisierungskarte einrichten** Fenster eine verkürzte Darstellungsform des Fensters **Datenaustauschdefinition** für die entsprechenden Datenaustauschdefinition.</span><span class="sxs-lookup"><span data-stu-id="e153b-148">Accordingly, the **Exch. Rate Update Setup Card** window is a condensed view of the **Data Exchange Definition** window for the data exchange definition in question.</span></span>  

<span data-ttu-id="e153b-149">Für den gesamten Austausch von Daten in XML-Dateien können Sie die Einrichtung des Datenaustausches vorbereiten, indem Sie die zugehörige **XML-Schemadatei** im Fenster laden.</span><span class="sxs-lookup"><span data-stu-id="e153b-149">For all exchanges of data in XML files, you can prepare the data exchange setup by loading the related XML schema file in the **XML Schema Viewer** window.</span></span> <span data-ttu-id="e153b-150">Hier wählen Sie die Datenelemente aus, die Sie mit [!INCLUDE[d365fin](includes/d365fin_md.md)]  austauschen möchten, und dann initialisieren Sie entweder eine Datenaustauschdefinition oder generieren einen XMLport.</span><span class="sxs-lookup"><span data-stu-id="e153b-150">Here you select the data elements that you want to exchange with [!INCLUDE[d365fin](includes/d365fin_md.md)]  and then you either initialize a data exchange definition or generate an XMLport.</span></span>  

<span data-ttu-id="e153b-151">Die folgende Tabelle enthält eine Abfolge von Aufgaben sowie Links zu den entsprechenden Themen, in denen diese Aufgaben erläutert werden.</span><span class="sxs-lookup"><span data-stu-id="e153b-151">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="e153b-152">An</span><span class="sxs-lookup"><span data-stu-id="e153b-152">To</span></span>|<span data-ttu-id="e153b-153">Siehe</span><span class="sxs-lookup"><span data-stu-id="e153b-153">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="e153b-154">Erfahren Sie, wie das Daten-Exchange-Framework arbeitet.</span><span class="sxs-lookup"><span data-stu-id="e153b-154">Learn how the Data Exchange Framework works.</span></span>|[<span data-ttu-id="e153b-155">Über das Datenaustauschframework</span><span class="sxs-lookup"><span data-stu-id="e153b-155">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)|  
|<span data-ttu-id="e153b-156">Bereiten Sie den Datenaustausch per Datei vor, indem Sie das XML-Schema der Datei verwenden.</span><span class="sxs-lookup"><span data-stu-id="e153b-156">Prepare to exchange data in a file by reusing the file’s XML schema.</span></span> <span data-ttu-id="e153b-157">Richten Sie Datenaustauschdefinitionen ein.</span><span class="sxs-lookup"><span data-stu-id="e153b-157">Set up data exchange definitions.</span></span> <span data-ttu-id="e153b-158">Richten Sie Stammdaten für das Senden von elektronischen Belegen ein.</span><span class="sxs-lookup"><span data-stu-id="e153b-158">Set up master data for electronic document sending.</span></span> <span data-ttu-id="e153b-159">Richten Sie verschiedene Felder für den Bankimport und -export ein.</span><span class="sxs-lookup"><span data-stu-id="e153b-159">Set up various bank import/export fields.</span></span>|[<span data-ttu-id="e153b-160">Einrichten eines Datenaustauschs</span><span class="sxs-lookup"><span data-stu-id="e153b-160">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)|  
|<span data-ttu-id="e153b-161">Auf der Grundlage von Datenaustauschdefinitionen senden und empfangen Sie PEPPOL-Rechnungen, importieren Bankauszüge und exportieren Bankzahlungsdateien.</span><span class="sxs-lookup"><span data-stu-id="e153b-161">Based on data exchange definitions, send PEPPOL invoices, receive PEPPOL invoices, import bank statements, and export bank payment files.</span></span>|[<span data-ttu-id="e153b-162">Austausch von Daten</span><span class="sxs-lookup"><span data-stu-id="e153b-162">Exchanging Data</span></span>](across-exchange-data.md)|  

## <a name="see-also"></a><span data-ttu-id="e153b-163">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e153b-163">See Also</span></span>  
[<span data-ttu-id="e153b-164">Über das Datenaustauschframework</span><span class="sxs-lookup"><span data-stu-id="e153b-164">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)  
[<span data-ttu-id="e153b-165">Gewusst wie: Verwenden von XML-Schemata zur Vorbereitung von Datenaustauschdefinitionen</span><span class="sxs-lookup"><span data-stu-id="e153b-165">How to: Use XML Schemas to Prepare Data Exchange Definitions</span></span>](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)  
[<span data-ttu-id="e153b-166">Einrichten eines Datenaustauschs</span><span class="sxs-lookup"><span data-stu-id="e153b-166">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="e153b-167">Austausch von Daten</span><span class="sxs-lookup"><span data-stu-id="e153b-167">Exchanging Data</span></span>](across-exchange-data.md)  
[<span data-ttu-id="e153b-168">Eingehende Belege</span><span class="sxs-lookup"><span data-stu-id="e153b-168">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="e153b-169">Allgemeine Geschäftsfunktionen</span><span class="sxs-lookup"><span data-stu-id="e153b-169">General Business Functionality</span></span>](ui-across-business-areas.md)
