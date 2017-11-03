---
title: Zusammenfassende Meldung in Deutschland
description: "In Deutschland wird die deutsche zusammenfassende Meldung an das „Bundeszentralamt für Steuern” (BZSt) über das BZSt-Onlineportal mithilfe der ELMA5-Schnittstelle übermittelt."
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
ms.openlocfilehash: fb18e25289f291f541672dca719c103cccbe390f
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="eu-sales-list-in-germany"></a><span data-ttu-id="78f58-103">Zusammenfassende Meldung in Deutschland</span><span class="sxs-lookup"><span data-stu-id="78f58-103">EU Sales List in Germany</span></span>
<span data-ttu-id="78f58-104">In Deutschland wird die deutsche zusammenfassende Meldung an das „Bundeszentralamt für Steuern” (BZSt) über das BZSt-Onlineportal mithilfe der ELMA5-Schnittstelle übermittelt.</span><span class="sxs-lookup"><span data-stu-id="78f58-104">In Germany, the German EU sales list is submitted to the "Bundeszentralamt für Steuern" (BZSt) through the BZSt Online Portal by using the ELMA5 interface.</span></span>  

<span data-ttu-id="78f58-105">Um die Sicherheit zu erhöhen, müssen alle Arten von Steuern und Steuererklärungen unter einer Authentifizierungsmethode übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="78f58-105">In order to increase security, all types of taxes and tax reports must be submitted under an authentication method.</span></span> <span data-ttu-id="78f58-106">Seit 1. Januar 2013 ist es obligatorisch, dass Sie Übermittlungen mit Authentifizierung vornehmen.</span><span class="sxs-lookup"><span data-stu-id="78f58-106">Beginning in January 1, 2013, it has become mandatory that you make submissions with authentication.</span></span> <span data-ttu-id="78f58-107">Dazu melden Sie sich mit Ihrer BZSt-Nummer und Ihrem privaten Schlüssel an, indem Sie Ihre Passphrase im ELMA5-Kommunikationsserver verwenden.</span><span class="sxs-lookup"><span data-stu-id="78f58-107">To do so, you sign in with your BZSt number and private key using your pass phrase on the ELMA5 communications server.</span></span> <span data-ttu-id="78f58-108">ELMA5 ist dafür ausgelegt, die Übermittlung großer Datasets von mehr als 1000 Datensätzen zu handhaben.</span><span class="sxs-lookup"><span data-stu-id="78f58-108">ELMA5 is designed to handle the transmission of large datasets of more than 1000 records.</span></span> <span data-ttu-id="78f58-109">Nach erfolgreicher Anmeldung können Sie die Datenübertragung in interaktiver Weise hochladen.</span><span class="sxs-lookup"><span data-stu-id="78f58-109">Following successful login, you can upload the data transfer in an interactive way.</span></span> <span data-ttu-id="78f58-110">Sie können die Übertragung auf automatisch einrichten.</span><span class="sxs-lookup"><span data-stu-id="78f58-110">You can also set up the transfer to be automatic.</span></span>  

## <a name="implementation-in-includenavnowincludesnavnowmdmd"></a><span data-ttu-id="78f58-111">Implementierung in [!INCLUDE[navnow](../../includes/navnow_md.md)]</span><span class="sxs-lookup"><span data-stu-id="78f58-111">Implementation in [!INCLUDE[navnow](../../includes/navnow_md.md)]</span></span>  
 [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="78f58-112"> und übermitteln Sie es dann an die Verarbeitungsbehörde (ZIVIT).</span><span class="sxs-lookup"><span data-stu-id="78f58-112"> and then submit it to the processing agency (ZIVIT).</span></span>
 
> [!IMPORTANT]  
>  <span data-ttu-id="78f58-113">Die Möglichkeit, einen MwSt.-Bericht in einem XML-Format zu übermitteln, wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78f58-113">The ability to submit a VAT report in an XML format is not supported.</span></span> <span data-ttu-id="78f58-114">Sie können jedoch eine Übermittlung von weniger als 1000 Datensätzen in einer CSV-Datei vornehmen.</span><span class="sxs-lookup"><span data-stu-id="78f58-114">However, you can make a submission of fewer than 1000 records in a .csv file.</span></span> <span data-ttu-id="78f58-115">Dazu können Sie das Elster-Onlineportal verwenden und die Stapelverarbeitung „Zusammenfassende Meldung Disk”, Bericht 88, verwenden.</span><span class="sxs-lookup"><span data-stu-id="78f58-115">For this, you can use the Elster Online portal, and use the VAT – VIES Declaration Disk batch job, report 88.</span></span>

## <a name="see-also"></a><span data-ttu-id="78f58-116">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="78f58-116">See Also</span></span>  
<span data-ttu-id="78f58-117">[BZSt-Onlineportal](http://www.bzst.de) </span><span class="sxs-lookup"><span data-stu-id="78f58-117">[BZSt Online Portal](http://www.bzst.de) </span></span>  
[<span data-ttu-id="78f58-118">Gewusst wie: MwSt.-Berichte erstellen</span><span class="sxs-lookup"><span data-stu-id="78f58-118">How to: Create VAT Reports</span></span>](how-to-create-vat-reports.md)

