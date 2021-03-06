---
title: 'Besturingselement voor scherm: naslag | Microsoft Docs'
description: Informatie, waaronder eigenschappen en voorbeelden, over het besturingselement Scherm
services: ''
suite: powerapps
documentationcenter: na
author: fikaradz
manager: anneta
editor: ''
tags: ''
ms.service: powerapps
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/25/2016
ms.author: fikaradz
ms.openlocfilehash: cd2e2a8c28fb894b1935b29bf80bf65eb631a266
ms.sourcegitcommit: 59785e9e82da8f5bd459dcb5da3d5c18064b0899
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2018
---
# <a name="screen-control-in-powerapps"></a>Schermbesturingselement in PowerApps
Een UI-element dat een of meer andere besturingselementen in een app bevat.

## <a name="description"></a>Beschrijving
De meeste apps hebben meerdere besturingselementen van het type **Scherm**, met daarin de besturingselementen **[Label](control-text-box.md)** en **[Knop](control-button.md)** en andere besturingselementen voor weergave van gegevens en ondersteuning van de navigatie.

## <a name="key-properties"></a>Belangrijkste eigenschappen
**[BackgroundImage](properties-visual.md)**: de naam van een afbeeldingsbestand dat op de achtergrond van een scherm wordt weergegeven.

**[Fill](properties-color-border.md)**: de achtergrondkleur van een besturingselement.

## <a name="additional-properties"></a>Aanvullende eigenschappen
**[ImagePosition](properties-visual.md)**: de positie (**Opvullen**, **Passend maken**, **Uitrekken**, **Naast elkaar** of **Centreren**) van een afbeelding in een scherm of een besturingselement als dit niet even groot is als de afbeelding.

**OnHidden**: hoe een app reageert wanneer de gebruiker van het scherm af navigeert.

**OnVisible**: hoe een app reageert wanneer de gebruiker naar het scherm navigeert.

**OnStart**: het gedrag van de app wanneer de gebruiker de app opent.

* De formule waarvoor deze eigenschap is ingesteld, wordt uitgevoerd voordat het eerste scherm van de app wordt weergegeven. Roep de functie [**Navigeren**](../functions/function-navigate.md) aan om te wijzigen welk scherm als eerste wordt weergegeven wanneer de app wordt gestart.
* U kunt geen [contextvariabelen](../working-with-variables.md) instellen met de functie [**UpdateContext**](../functions/function-updatecontext.md) omdat er nog geen scherm wordt weergegeven. U kunt echter contextvariabelen doorgeven via de functie **Navigeren** en een [verzameling](../working-with-variables.md) maken en vullen met behulp van de functie [**Verzamelen**](../functions/function-clear-collect-clearcollect.md).
* Wanneer u een app bijwerkt, wordt de formule waarvoor deze eigenschap is ingesteld uitgevoerd wanneer de app in PowerApps Studio wordt geladen. Als u wilt zien wat het effect is als u deze eigenschap wijzigt, moet u uw app opslaan, sluiten en opnieuw laden.
* De eigenschap **OnStart** is een eigenschap van de app, niet van het scherm. Voor het gemak bij het bewerken, kunt u deze weergeven en wijzigen als eigenschap op het eerste scherm van uw app. Als u het eerste scherm verwijdert of de volgorde van de schermen wijzigt, is deze eigenschap mogelijk moeilijk te vinden. Sla uw app in dit geval op, sluit hem en laad hem opnieuw. De eigenschap wordt dan weer als een eigenschap van het eerste scherm weergegeven.

## <a name="related-functions"></a>Verwante functies
[**Distinct**( *Gegevensbron*, *Kolomnaam* )](../functions/function-distinct.md)

## <a name="example"></a>Voorbeeld
1. Voeg een besturingselement **[Keuzerondje](control-radio.md)** toe, geef het de naam **Schermvullend** en stel de eigenschap **[Items](properties-core.md)** van het besturingselement in op deze waarde:<br>
   **["Rood", "Groen"]**
   
    Weet u niet hoe u [een besturingselement kunt toevoegen, een naam kunt geven of kunt configureren](../add-configure-controls.md)?
2. Geef het standaardbesturingselement **Screen** de naam **Bron**, voeg een ander besturingselement **Scherm** toe en geef dit de naam **Doel**.
3. Voeg aan **Bron** een besturingselement **[Vorm](control-shapes-icons.md)** toe (zoals een pijl) en stel de eigenschap **[OnSelect](properties-core.md)** van het besturingselement in op deze formule:<br>
   **Navigate(Doel, Schermovergang.Fade)**
   
    Wilt u meer informatie over de functie **[Navigate](../functions/function-navigate.md)** of [andere functies](../formula-reference.md)?
4. Voeg aan **Doel** een besturingselement **[Vorm](control-shapes-icons.md)** toe (zoals een pijl) en stel de eigenschap **[OnSelect](properties-core.md)** van het besturingselement in op deze formule:<br>
   **Navigate(Bron, Schermovergang.Fade)**
5. Stel de eigenschap **[Fill](properties-color-border.md)** van **Doel** in op deze formule:<br>
   **If("Red" in ScreenFills.Selected.Value, RGBA(255, 0, 0, 1), RGBA(54, 176, 75, 1))**
6. Druk in **Bron** op F5, klik of tik op een van beide opties in het besturingselement **[Keuzerondje](control-radio.md)** en klik of tik vervolgens op het besturingselement **[Vorm](control-shapes-icons.md)**.
   
    **Doel** wordt weergegeven in de kleur die u hebt gekozen.
7. Klik of tik in **Doel** op het besturingselement **[vorm](control-shapes-icons.md)** om terug te gaan naar **Bron**.
8. (Optioneel) Klik of tik op de andere optie in het besturingselement **[Keuzerondje](control-radio.md)** en klik of tik vervolgens op het besturingselement **[Vorm](control-shapes-icons.md)** om te controleren of **Doel** in de andere kleur wordt weergegeven.
9. Druk op Esc om terug te gaan naar de standaardwerkruimte.

