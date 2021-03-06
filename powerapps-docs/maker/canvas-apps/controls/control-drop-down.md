---
title: 'Besturingselement voor vervolgkeuzelijst: naslag | Microsoft Docs'
description: Informatie, waaronder eigenschappen en voorbeelden, over het besturingselement Vervolgkeuzelijst
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
ms.openlocfilehash: 828292cc888d26f2060260826296960f1bd4f98f
ms.sourcegitcommit: 59785e9e82da8f5bd459dcb5da3d5c18064b0899
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2018
---
# <a name="drop-down-control-in-powerapps"></a>Besturingselement voor vervolgkeuzelijst in PowerApps
Een lijst waarin alleen het eerste item wordt weergegeven, tenzij de gebruiker de lijst opent.

## <a name="description"></a>Beschrijving
Een besturingselement **Vervolgkeuzelijst** bespaart schermruimte, zeker als de lijst een groot aantal opties bevat. Het besturingselement neemt slechts één regel in beslag, tenzij de gebruiker de pijl-omlaag selecteert om andere opties weer te geven.

## <a name="key-properties"></a>Belangrijkste eigenschappen
**[Default](properties-core.md)**: de aanvankelijke waarde van een besturingselement voordat deze door de gebruiker wordt gewijzigd.

**[Items](properties-core.md)**: de gegevensbron die wordt weergegeven in een besturingselement zoals een galerie, een lijst of een grafiek.

[!INCLUDE [long-items](../../../includes/long-items.md)]

**Selected**: het geselecteerde item.

## <a name="additional-properties"></a>Aanvullende eigenschappen
**[BorderColor](properties-color-border.md)**: de kleur van de rand van een besturingselement.

**[BorderStyle](properties-color-border.md)**: hiermee wordt aangegeven of de rand van een besturingselement **effen**, **onderbroken** of **gestippeld** is, of dat er **geen** rand is.

**[BorderThickness](properties-color-border.md)**: de dikte van de rand van een besturingselement.

**[FocusedBorderThickness](properties-color-border.md)**: de dikte van de rand van een besturingselement wanneer deze de toetsenbordfocus heeft.

**ChevronBackground**: de kleur achter de pijl-omlaag in een vervolgkeuzelijst.

**ChevronFill**: de kleur van de pijl-omlaag in een vervolgkeuzelijst.

**[Color](properties-color-border.md)**: de kleur van de tekst in een besturingselement.

**[DisplayMode](properties-core.md)**: of invoer van de gebruiker is toegestaan (**Bewerken**), alleen gegevens worden weergegeven (**Weergeven**) of is uitgeschakeld (**Uitgeschakeld**).

**[DisabledBorderColor](properties-color-border.md)**: de kleur van de rand van een besturingselement als de eigenschap **[DisplayMode](properties-core.md)** is ingesteld op **Uitgeschakeld**.

**[DisabledColor](properties-color-border.md)**: de kleur van tekst in een besturingselement als de eigenschap **[DisplayMode](properties-core.md)** is ingesteld op **Uitgeschakeld**.

**[DisabledFill](properties-color-border.md)**: de achtergrondkleur van een besturingselement als de eigenschap **[DisplayMode](properties-core.md)** is ingesteld op **Uitgeschakeld**.

**[Fill](properties-color-border.md)**: de achtergrondkleur van een besturingselement.

**[Font](properties-text.md)**: de naam van de lettertypefamilie waarin de tekst wordt weergegeven.

**[FontWeight](properties-text.md)**: het gewicht van de tekst in een besturingselement: **Bold**, **Semibold**, **Normal** of **Lighter**.

**[Height](properties-size-location.md)** : de afstand tussen de boven- en onderrand van een besturingselement.

**[HoverBorderColor](properties-color-border.md)**: de kleur van de rand van een besturingselement wanneer de gebruiker de muisaanwijzer op dat besturingselement plaatst.

**[HoverColor](properties-color-border.md)**: de kleur van de tekst in een besturingselement wanneer de gebruiker de muisaanwijzer op de tekst plaatst.

**[HoverFill](properties-color-border.md)**: de achtergrondkleur van een besturingselement wanneer de gebruiker de muisaanwijzer op de achtergrond plaatst.

**[Italic](properties-text.md)**: hiermee wordt aangegeven of de tekst in een besturingselement cursief is.

**[OnChange](properties-core.md)**: de manier waarop de app reageert wanneer de gebruiker de waarde van een besturingselement wijzigt (bijvoorbeeld door een schuifregelaar aan te passen).

**[OnSelect](properties-core.md)**: de manier waarop de app reageert wanneer de gebruiker op een besturingselement tikt of klikt.

**[PaddingBottom](properties-size-location.md)**: de afstand tussen de tekst in een besturingselement en de onderrand van het besturingselement.

**[PaddingLeft](properties-size-location.md)**: de afstand tussen de tekst in een besturingselement en de linkerrand van het besturingselement.

**[PaddingRight](properties-size-location.md)**: de afstand tussen de tekst in een besturingselement en de rechterrand van het besturingselement.

**[PaddingTop](properties-size-location.md)**: de afstand tussen de tekst in een besturingselement en de bovenrand van het besturingselement.

**[PressedBorderColor](properties-color-border.md)**: de kleur van de rand van een besturingselement wanneer de gebruiker op dat besturingselement tikt of klikt.

**[PressedColor](properties-color-border.md)**: de kleur van tekst in een besturingselement wanneer de gebruiker op dat besturingselement tikt of klikt.

**[PressedFill](properties-color-border.md)**: de achtergrondkleur van een besturingselement wanneer de gebruiker op dat besturingselement tikt of klikt.

**[Reset](properties-core.md)**: of een besturingselement wordt teruggezet op de standaardwaarde.

**[SelectionColor](properties-color-border.md)**: de tekstkleur van geselecteerde items in een lijst of de kleur van het selectiehulpmiddel in een besturingselement Pen.

**[SelectionFill](properties-color-border.md)**: de achtergrondkleur van geselecteerde items in een lijst of een geselecteerd gebied van een besturingselement Pen.

**[Size](properties-text.md)**: de tekengrootte van de tekst die in een besturingselement wordt weergegeven.

**[Strikethrough](properties-text.md)**: hiermee wordt aangegeven of een streep door de tekst van een besturingselement wordt weergegeven.

**[TabIndex](properties-accessibility.md)**: past de tabvolgorde van besturingselementen tijdens runtime aan wanneer hier een andere waarde dan nul is ingesteld.

**[Tooltip](properties-core.md)**: beschrijvende tekst die wordt weergegeven wanneer de gebruiker een besturingselement aanwijst.

**[Underline](properties-text.md)**: hiermee wordt aangegeven of onder de tekst in een besturingselement een streep wordt weergegeven.

**[Visible](properties-core.md)**: hiermee wordt aangegeven of een besturingselement zichtbaar of verborgen is.

**[Width](properties-size-location.md)**: de afstand tussen de linker- en rechterrand van een besturingselement.

**[X](properties-size-location.md)**: de afstand tussen de linkerrand van een besturingselement en de linkerrand van de bovenliggende container (het scherm als er geen bovenliggende container is).

**[Y](properties-size-location.md)**: de afstand tussen de bovenrand van een besturingselement en de bovenrand van de bovenliggende container (het scherm als er geen bovenliggende container is).

## <a name="example"></a>Voorbeeld
1. Voeg een besturingselement **[Knop](control-button.md)** toe en stel de eigenschap **[Text](properties-core.md)** ervan in op **Verzamelen**.
   
    Weet u niet hoe u [een besturingselement kunt toevoegen, een naam kunt geven of kunt configureren](../add-configure-controls.md)?
2. Stel de eigenschap **[OnSelect](properties-core.md)** van het besturingselement **[Knop](control-button.md)** in op deze formule:
   <br>**ClearCollect(Inwonersaantallen, {Stad:"Londen", Land:"Engeland", Inwonersaantal:8615000}, {Stad:"Berlijn", Land:"Duitsland", Inwonersaantal:3562000}, {Stad:"Madrid", Land:"Spanje", Inwonersaantal:3165000}, {Stad:"Rome", Land:"Italië", Inwonersaantal:2874000}, {Stad:"Parijs", Land:"Frankrijk", Inwonersaantal:2273000}, {Stad:"Hamburg", Land:"Duitsland", Inwonersaantal:1760000}, {Stad:"Barcelona", Land:"Spanje", Inwonersaantal:1602000}, {Stad:"München", Land:"Duitsland", Inwonersaantal:1494000}, {Stad:"Milaan", Land:"Italië", Inwonersaantal:1344000})**
   
    Wilt u meer informatie over de functie **[ClearCollect](../functions/function-clear-collect-clearcollect.md)** of een [andere functie](../formula-reference.md)?
3. Druk op F5, klik of tik op het besturingselement **[Button](control-button.md)** en druk vervolgens op Esc.
4. Voeg een besturingselement **Vervolgkeuzelijst** toe, geef het de naam **Landen** en stel de eigenschap **[Items](properties-core.md)** van het besturingselement in op deze formule:
   <br>**Distinct(Inwonersaantallen, Land)**
5. Voeg een besturingselement **Tekstgalerie** toe in verticale/staande richting en stel de eigenschap **[Items](properties-core.md)** van de galerie in op deze formule:
   <br>**Filter(Inwonersaantallen, Landen.Selected.Value in Land)**
6. Stel in het eerste item van het besturingselement **Tekstgalerie** de eigenschap **[Text](properties-core.md)** van het bovenste besturingselement **[Label](control-text-box.md)** in op **ThisItem.Stad** en verwijder het onderste besturingselement **[Label](control-text-box.md)**.
7. Stel de eigenschap **[TemplateSize](control-gallery.md)** van het besturingselement **Tekstgalerie** tot in op **80**.
8. Druk op F5, klik of tik op de pijl-omlaag van de lijst **Landen** en kies vervolgens een optie in de lijst.
   
    Het besturingselement **Tekstgalerie** toont alleen de plaatsen in het land dat u hebt gekozen.

