---
title: De functie Table | Microsoft Docs
description: Naslaginformatie, inclusief syntaxis en voorbeelden, voor de functie Table in PowerApps
services: ''
suite: powerapps
documentationcenter: na
author: gregli-msft
manager: anneta
editor: ''
tags: ''
ms.service: powerapps
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 11/07/2015
ms.author: gregli
ms.openlocfilehash: 2f543a75019bfe5d665aedb2e6171200e8321690
ms.sourcegitcommit: 59785e9e82da8f5bd459dcb5da3d5c18064b0899
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2018
---
# <a name="table-function-in-powerapps"></a>De functie Table in PowerApps
Hiermee maakt u een tijdelijke [tabel](../working-with-tables.md).

## <a name="description"></a>Beschrijving
De functie **Table** maakt een tabel van een argumentlijst met [records](../working-with-tables.md#records).

De [kolommen](../working-with-tables.md#columns) van de tabel vormen de samenvoeging van de eigenschappen van alle records in het argument. Een *lege* waarde wordt toegevoegd aan elke kolom waarvoor een record geen waarde bevat.

Een tabel is een waarde in PowerApps, net zoals een tekenreeks of getal. U kunt een tabel opgeven als een argument voor een functie en functies kunnen een tabel retourneren als resultaat. **Table** maakt geen permanente tabel. In plaats daarvan wordt een tijdelijke tabel geretourneerd, bestaande uit de argumenten.  U kunt deze tijdelijke tabel opgeven als argument voor een andere functie of de tabel visualiseren in een galerie of insluiten in een andere tabel.  Zie [werken met tabellen](../working-with-tables.md) voor meer informatie.

U kunt ook een tabel met één kolom maken met de syntaxis **[ waarde1, waarde2,... ]**.

## <a name="syntax"></a>Syntaxis
**Table**( *Record1* [, *Record2*, ... ] )

* *Record(s)* - vereist. De records die aan de tabel moeten worden toegevoegd.

## <a name="examples"></a>Voorbeelden
* Stel de eigenschap **[Items](../controls/properties-core.md)** van een keuzelijst in op deze formule:
  <br>**Table({Kleur:"rood"}, {Kleur:"groen"}, {Kleur:"blauw"})**
  
    In de keuzelijst wordt elke kleur weergegeven als een optie.
* Voeg een tekstgalerie toe en stel de eigenschap **[Items](../controls/properties-core.md)** ervan in op deze functie:<br>
  **Table({Item:"Violin123", Location:"France", Owner:"Fabrikam"}, {Item:"Violin456", Location:"Chile"})**
  
    De galerie bevat twee records die beide de naam en de locatie van een item bevatten. Slechts één record bevat de naam van de eigenaar.

