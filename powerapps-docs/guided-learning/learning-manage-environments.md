---
title: Omgevingen | Microsoft Docs
description: Werken met containers voor apps, verbindingen en andere resources
services: 
suite: powerapps
documentationcenter: na
author: mgblythe
manager: anneta
editor: 
tags: 
featuredvideoid: 32olG9uCmBU
courseduration: 8m
ms.service: powerapps
ms.devlang: na
ms.topic: get-started-article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 12/09/2016
ms.author: mblythe
ms.openlocfilehash: 3f17dd94359f9c6d20464662a860fd9f784991c3
ms.sourcegitcommit: 43be6a4e08849d522aabb6f767a81c092419babc
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/07/2017
---
# <a name="powerapps-environments"></a>PowerApps-omgevingen
Als u de cursus tot nu toe hebt gevolgd, hebt u enige tijd besteed aan het werken in web.powerapps.com. Of u dat nu wist of niet, u hebt al die tijd in een specifieke *omgeving* gewerkt. Een omgeving is gewoon een groepering van apps en andere resources (meer hierover vindt u wat verderop). In de rechterbovenhoek van het scherm in web.powerapps.com ziet u een vervolgkeuzelijst die uw huidige omgeving weergeeft.

![Omgeving kiezen](./media/learning-manage-environments/environment-picker.png)

Als u nog niet eerder met PowerApps hebt gewerkt, ziet u momenteel wellicht alleen de standaardomgeving. Klik of tik op het menu om te zien of er andere omgevingen beschikbaar zijn.

## <a name="why-use-environments"></a>Waarom moeten omgevingen worden gebruikt?
Een omgeving is een container voor apps en andere resources, zoals gegevensverbindingen en stromen van Microsoft Flow. Het is een manier om dingen te groeperen op basis van zakelijke vereisten. Er zijn diverse redenen om extra omgevingen naast de standaardomgeving te maken:

* **Gescheiden app-ontwikkeling per afdeling**: in een grote organisatie kan elke afdeling in een andere omgeving werken.
* **Ondersteuning voor Application Lifecycle Management (ALM)**: u kunt afzonderlijke omgevingen hebben voor apps in ontwikkeling en voor apps die al klaar zijn en die u hebt gedeeld.
* **Gegevenstoegang beheren**: elke omgeving kan een eigen Common Data Service-database hebben en andere gegevensverbindingen gelden specifiek voor een bepaalde omgeving (dat wil zeggen dat ze niet worden gedeeld tussen omgevingen).

Houd er wel rekening mee dat omgevingen alleen relevant zijn voor app-ontwikkelaars en beheerders van PowerApps. Wanneer u een app aan gebruikers beschikbaar stelt, kunnen die gebruikers de app uitvoeren zolang ze de juiste machtigingen hebben. Ze hoeven zich niet druk te maken over uit welke omgeving de app afkomstig is.

## <a name="create-an-environment"></a>Een omgeving maken
We hebben ons in deze cursus tot nu toe gericht op app-ontwikkelaars, maar omgevingen worden gemaakt en onderhouden door beheerders. Ook als u geen beheerder bent, kan deze informatie nuttig zijn wanneer u het met uw beheerder hebt over het instellen van omgevingen. Klik of tik in het beheercentrum van PowerApps op **Omgevingen** en vervolgens op **Nieuwe omgeving**. Voer in het scherm **Nieuwe omgeving** een naam in voor de omgeving, selecteer een regio, geef aan of u een Common Data Services-database voor de omgeving wilt maken en klik of tik op **Create an environment**.

![Een omgeving maken](./media/learning-manage-environments/create-environment.png)

Dat is het. U hebt nu een nieuwe omgeving om in te werken. Als u teruggaat naar web.powerapps.com, wordt de omgeving weergegeven in de vervolgkeuzelijst met omgevingen.

## <a name="manage-access-to-an-environment"></a>Toegang tot een omgeving beheren
U hebt toegang tot een omgeving als u:

* een **omgevingsbeheerder** bent: u hebt volledige machtigingen in de omgeving.
* een **omgevingsmaker** bent: u kunt alle apps zien, apps maken en werken met de Common Data Service (er gelden dan andere machtigingen).

Als beheerder verleent u toegang tot een omgeving vanaf het tabblad **Omgevingen**. Klik of tik op een omgeving om te beginnen. Als u iemand wilt toevoegen (een **omgevingsmaker** in dit voorbeeld), klikt of tikt u op **Rollen van de omgeving** en vervolgens op **Omgevingsmaker**. Voeg van daaruit gebruikers of groepen toe aan de rol en klik of tik op **Opslaan**.

![Toegang tot de omgeving beheren](./media/learning-manage-environments/environment-access.png)

U kent nu de voordelen van omgevingen, hoe u omgevingen kunt maken en hoe u er toegang tot kunt verlenen. Zelfs als u niet de rol van beheerder hebt, is het handig om te weten hoe dit werkt. Daarmee zijn we aan het eind gekomen van de sectie Apps beheren en bent u goed voorbereid om te beginnen aan de volgende sectie, Gegevens beheren, die is gewijd aan de Common Data Service.
