---
title: FunctieFunctie Vernieuwen | Microsoft Docs
description: Naslaginformatie, inclusief syntaxis en voorbeelden, voor de functie Refresh in PowerApps
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
ms.date: 10/21/2015
ms.author: gregli
ms.openlocfilehash: 631b0c8fbfc98d73cf1d944c2a0f3933f8f10c11
ms.sourcegitcommit: 59785e9e82da8f5bd459dcb5da3d5c18064b0899
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2018
---
# <a name="refresh-function-in-powerapps"></a>De functie Refresh in PowerApps
Hiermee vernieuwt u de [records](../working-with-tables.md#records) van een [gegevensbron](../working-with-data-sources.md).

## <a name="description"></a>Beschrijving
De functie **Refresh** haalt een nieuwe kopie van een gegevensbron op.  U ziet dan wijzigingen die andere gebruikers hebben aangebracht.

**Refresh** heeft geen retourwaarde en u kunt deze functie alleen gebruiken in [gedragsformules](../working-with-formulas-in-depth.md).

## <a name="syntax"></a>Syntaxis
**Refresh**( *DataSource* )

* *DataSource* - vereist. De gegevensbron die u wilt vernieuwen.

## <a name="example"></a>Voorbeeld
In dit voorbeeld vernieuwt u de gegevensbron met de naam **IJs** die begint met deze gegevens:

![](media/function-refresh/icecream.png)

Een gebruiker op een ander apparaat wijzigt **Aantal** in de record **Aardbeien** in **400**.  U ziet deze wijziging pas nadat u deze formule hebt uitgevoerd:

**Refresh( IJs )**

Nadat de formule is uitgevoerd, wordt in galerieën die zijn gebonden aan de gegevensbron **IJs** de bijgewerkte waarde voor **Aardbeien** weergegeven:

![](media/function-refresh/icecream-after.png)

