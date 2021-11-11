---
title: Richtlijnen voor het exporteren van levenscyclusgegevens
description: Richtlijnen voor informatie over de productlevenscyclus exporteren
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546794"
---
# <a name="lifecycle-data-export-guidance"></a>Richtlijnen voor het exporteren van levenscyclusgegevens
Dit document beschrijft hoe u het exportbestand van het product gebruikt.

## <a name="query-information"></a>Informatie over query
In het Excel-document zijn er velden die helpen bij het identificeren van de gegevens die in de producttabel zijn ingevuld.

### <a name="end-of-support"></a>Einde van de ondersteuning
De waarde voor het einde van de ondersteuning filtert producten op de einddatum van de ondersteuning van het product of de einddatums van de release.

Mogelijke waarden: alle (geen filter toegepast), jaar en een bereik.

### <a name="family"></a>Familie
De familiewaarde filtert producten op het bovenliggende niveau binnen de hiërarchie die bekend staat als de familie.

Mogelijke waarden: alle (geen filter toegepast), familienaam

### <a name="group"></a>Groep
De groepswaarde filtert producten binnen het bovenliggende niveau (familie) naar een specifieke groep.

Mogelijke waarden: alle (geen filter toegepast), groepsnaam

## <a name="table-columns"></a>Tabelkolommen
De producttabel bestaat uit kolommen die het product, de edities, releases en bijbehorende ondersteuningsdatums definiëren.

> [!NOTE]
> Er wordt een rij voor elke combinatie van producten, edities en releases gemaakt.

### <a name="product"></a>Product
De productnaam.

### <a name="edition"></a>Editie
De editiekolom wordt ingevuld wanneer het product edities bevat. Als er geen producteditie is, is dit veld leeg.

### <a name="release"></a>Vrijgeven
De releasekolom wordt ingevuld wanneer het product meerdere releases bevat.
Wanneer het product slechts één release heeft, is dit veld leeg.

### <a name="support-policy"></a>Ondersteuningsbeleid
Dit veld definieert welk ondersteuningsbeleid het product volgt.

Mogelijke waarden: [vast](/lifecycle/policies/fixed), [modern](/lifecycle/policies/modern), onderdeel

### <a name="start-date"></a>Begindatum
Datum dat de ondersteuning is gestart voor het product.

### <a name="mainstream-date"></a>Datum voor basis
Als het ondersteuningsbeleid **vast** of **onderdeel** is, is dit de datum voor de basis-einddatum van het product.
  
Wanneer ondersteuningsbeleid **modern** is, is dit leeg.

### <a name="extended-end-date"></a>Verlengde einddatum
Wanneer het ondersteuningsbeleid **vast** of **onderdeel** is, is dit de datum voor de uitgebreide einddatum van het product.

Wanneer ondersteuningsbeleid **modern** is, is dit leeg.

### <a name="retirement-date"></a>Datum voor beëindiging
Als het ondersteuningsbeleid **vast** of **onderdeel** is, is dit leeg.

Als ondersteuningsbeleid **modern** is, is dit de beëindigingsdatum van het product.

### <a name="release-start-date"></a>Begindatum van de release
Datum dat de ondersteuning is gestart voor de release. Wanneer het product slechts één release heeft, is dit veld leeg.
 
### <a name="release-end-date"></a>Einddatum release
Datum waarop de ondersteuning voor de release is beëindigd.
Wanneer het product slechts één release heeft, is dit veld leeg.

### <a name="docs-url"></a>Documenten-url
Url naar uitgebreide documentatie.
