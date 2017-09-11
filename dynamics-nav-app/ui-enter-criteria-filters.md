---
title: Eingeben von Kriterien in Filtern
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df386e1195db385ee053b69fec0f5082d8df4116
ms.contentlocale: de-de
ms.lasthandoff: 07/19/2017

---

# <a name="entering-criteria-in-filters"></a><span data-ttu-id="143e4-102">Eingeben von Kriterien in Filtern</span><span class="sxs-lookup"><span data-stu-id="143e4-102">Entering Criteria in Filters</span></span>
<span data-ttu-id="143e4-103">Wenn Sie nach Daten, wie Debitorennamen, Adressen oder Produktgruppen suchen möchten, geben Sie Kriterien ein.</span><span class="sxs-lookup"><span data-stu-id="143e4-103">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="143e4-104">Beim Eingeben von Filterkriterien können alle Ziffern und Buchstaben verwendet werden, die auch normalerweise im Feld zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="143e4-104">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="143e4-105">Zudem können Sie Sonderzeichen verwenden, um eine zusätzliche Filterung der Ergebnisse zu erreichen.</span><span class="sxs-lookup"><span data-stu-id="143e4-105">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="143e4-106">Suchen mithilfe des Schnellfilters</span><span class="sxs-lookup"><span data-stu-id="143e4-106">Searching using the Quick Filter</span></span>
<span data-ttu-id="143e4-107">Sie können allen Seiten Filter hinzufügen, indem Sie Schnellfilter oder erweiterte Filter verwenden.</span><span class="sxs-lookup"><span data-stu-id="143e4-107">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="143e4-108">Der Schnellfilter wird aktiviert, indem Sie das Lupensymbol in der oberen rechten Ecke einer Seite auswählen.</span><span class="sxs-lookup"><span data-stu-id="143e4-108">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="143e4-109">Diese Filterart wird für die schnelle Eingabe von Kriterien verwendet.</span><span class="sxs-lookup"><span data-stu-id="143e4-109">This filtering type is used for a fast entry of criteria.</span></span>

<span data-ttu-id="143e4-110">**Wichtig**: Der Schnellfilter bietet einen einfachen Zugriff auf Filterdaten durch die Eingabe reinen Texts, bietet aber auch zahlreiche Optionen für Suchkriterien.</span><span class="sxs-lookup"><span data-stu-id="143e4-110">**Important**: The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="143e4-111">Abhängig davon, ob Sie Freitext oder Text mit Symbolen eingeben, verhält sich der Schnellfilter unterschiedlich.</span><span class="sxs-lookup"><span data-stu-id="143e4-111">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  
- <span data-ttu-id="143e4-112">Wenn Sie Freitextangaben in den Suchkriterien eingeben, werden die Suchkriterien als die Groß-/Kleinschreibung nicht beachtend angesehen.</span><span class="sxs-lookup"><span data-stu-id="143e4-112">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
- <span data-ttu-id="143e4-113">Wenn Sie Text mit Symbolen in den Suchkriterien eingeben, werden die Suchkriterien genau wie angegeben interpretiert, und die Groß-/Kleinschreibung wird berücksichtigt.</span><span class="sxs-lookup"><span data-stu-id="143e4-113">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="143e4-114">Schnelle Filterkriterien</span><span class="sxs-lookup"><span data-stu-id="143e4-114">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="143e4-115">Suchkriterien</span><span class="sxs-lookup"><span data-stu-id="143e4-115">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="143e4-116">Interpretiert als...</span><span class="sxs-lookup"><span data-stu-id="143e4-116">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="143e4-117">Reklamationen...</span><span class="sxs-lookup"><span data-stu-id="143e4-117">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="143e4-118">>man</span><span class="sxs-lookup"><span data-stu-id="143e4-118">>man</span></span></TD>
    <TD><span data-ttu-id="143e4-119">@*man*</span><span class="sxs-lookup"><span data-stu-id="143e4-119">@*man*</span></span></TD>
    <TD><span data-ttu-id="143e4-120">Alle Datensätze, die den Text Mann enthalten und die Groß-/Kleinschreibung nicht beachten.</span><span class="sxs-lookup"><span data-stu-id="143e4-120">All records that contain the text man and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="143e4-121">>se</span><span class="sxs-lookup"><span data-stu-id="143e4-121">>se</span></span></TD>
    <TD><span data-ttu-id="143e4-122">@*se*</span><span class="sxs-lookup"><span data-stu-id="143e4-122">@*se*</span></span></TD>
    <TD><span data-ttu-id="143e4-123">Alle Datensätze, die den Text se enthalten und die Groß-/Kleinschreibung nicht beachten.</span><span class="sxs-lookup"><span data-stu-id="143e4-123">All records that contain the text se and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="143e4-124">>Man*</span><span class="sxs-lookup"><span data-stu-id="143e4-124">>Man*</span></span></TD>
    <TD><span data-ttu-id="143e4-125">Beginnt mit „Man“, Groß-/Kleinschreibung beachtet</span><span class="sxs-lookup"><span data-stu-id="143e4-125">Starts with Man and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="143e4-126">Alle Datensätze, die mit dem Text Mann beginnen.</span><span class="sxs-lookup"><span data-stu-id="143e4-126">All records that start with the text Man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="143e4-127">'man'</span><span class="sxs-lookup"><span data-stu-id="143e4-127">'man'</span></span></TD>
    <TD><span data-ttu-id="143e4-128">Exakter Text unter Berücksichtigung der Groß-/Kleinschreibung</span><span class="sxs-lookup"><span data-stu-id="143e4-128">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="143e4-129">Alle Datensätze, die mit Mann genau übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="143e4-129">All records that match man exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="143e4-130">@*man</span><span class="sxs-lookup"><span data-stu-id="143e4-130">@*man</span></span></TD>
    <TD><span data-ttu-id="143e4-131">Endet mit, Groß-/Kleinschreibung beachtet</span><span class="sxs-lookup"><span data-stu-id="143e4-131">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="143e4-132">Alle Datensätze, die mit mann enden.</span><span class="sxs-lookup"><span data-stu-id="143e4-132">All records that end with man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="143e4-133">@man*</span><span class="sxs-lookup"><span data-stu-id="143e4-133">@man*</span></span></TD>
    <TD><span data-ttu-id="143e4-134">Beginnt mit, Groß-/Kleinschreibung beachtet</span><span class="sxs-lookup"><span data-stu-id="143e4-134">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="143e4-135">Alle Datensätze, die mit Mann beginnen.</span><span class="sxs-lookup"><span data-stu-id="143e4-135">All records that start with man.</span></span></TD>
  </TR>
</TABLE>

<span data-ttu-id="143e4-136">**Hinweis**: Sie können keinen Platzhalter beim Filtern in Aufzählungsfeldern, wie das Feld **Status** in Verkaufsaufträgen verwenden.</span><span class="sxs-lookup"><span data-stu-id="143e4-136">**Note**: You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="143e4-137">Wenn Sie einen Filter für diese Art von Feld eingeben möchten, können Sie den numerischen Wert als Filterparameter eingeben.</span><span class="sxs-lookup"><span data-stu-id="143e4-137">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="143e4-138">Beispielsweise im Feld **Status** in einem Verkaufsauftrag, der die Werte **Offen**, **Freigegeben**, **Genehmigung ausstehend** und **Vorauszahlung ausstehend** hat, verwenden Sie die Werte **0**, **1**, **2** und **3**, um für diese Optionen zu filtern.</span><span class="sxs-lookup"><span data-stu-id="143e4-138">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="143e4-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="143e4-139">See Also</span></span>
[<span data-ttu-id="143e4-140">Arbeiten mit Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="143e4-140">Work with Dynamics NAV</span></span>](ui-work-product.md)

