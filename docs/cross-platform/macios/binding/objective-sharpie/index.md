---
title: Objektive Sharpie
description: "Dieser Abschnitt enthält eine Einführung in die Ziel-Sharpie, Xamarin Befehlszeilentool verwendet, um das Erstellen einer Bindung an eine Bibliothek für Objective-C automatisieren"
ms.topic: article
ms.prod: xamarin
ms.assetid: 8A832A76-A770-1A7C-24BA-B3E6F57617A0
ms.technology: xamarin-cross-platform
author: asb3993
ms.author: amburns
ms.date: 10/11/2017
ms.openlocfilehash: 02eebb7d8f579a207b6777771dbea223d30211cc
ms.sourcegitcommit: 6cd40d190abe38edd50fc74331be15324a845a28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/27/2018
---
# <a name="objective-sharpie"></a>Objektive Sharpie

_Dieser Abschnitt enthält eine Einführung in die Ziel-Sharpie, Xamarin Befehlszeilentool verwendet, um das Erstellen einer Bindung an eine Bibliothek für Objective-C automatisieren_

<style type="text/css"> .Terminal Blau {Color: rgb(10,96,254);} .terminal Grün {Color: rgb(12,156,26);} .terminal Magenta {Farbe: rgb(152,12,103);} </style>

- [Übersicht über](#overview) & [Verlauf](#history)
- [Erste Schritte](get-started.md)
- [Tools und Befehle](tools.md)
- [Features](platform/index.md)
- [Beispiele](examples/index.md)
- [Vollständige Exemplarische Vorgehensweise](~/ios/platform/binding-objective-c/walkthrough.md)
- [Releaseverlauf](releases.md)

#<a name="overview"></a>Übersicht

Objektive Sharpie ist ein Befehlszeilentool helfen beim Bootstrapping für des ersten Durchlaufs einer Bindung.
Es funktioniert, indem die Analyse der Headerdateien einer systemeigenen Bibliothek zuordnen die öffentliche API in der [Bindungsdefinition](~/cross-platform/macios/binding/objective-c-libraries.md#The_API_definition_file) (dieser Prozess, die zuvor manuell erstellt wurde).

Objektive Sharpie verwendet Clang Analyse der Headerdateien, damit die Bindung als genaue und umfassend wie möglich ist. Diese kann erheblich reduzieren, Zeit und Mühe dauert um eine Bindung Qualität zu erzeugen.

> [!IMPORTANT]
> **Warnung:** objektiven Sharpie ist ein Tool für erfahrene Entwickler von Xamarin mit Kenntnissen von Objective-C (und durch Erweiterung auch C). Bevor Sie versuchen, eine Bibliothek für Objective-C-Bindung sollten Sie solide Kenntnisse im Erstellen Sie die systemeigene Bibliothek auf der Befehlszeile aus (und ein gutes Verständnis der Funktionsweise der systemeigenen Bibliothek) verfügen.



#<a name="history"></a>Versionsgeschichte

Wir haben entwickelt wurde und Verwenden der Ziel-Sharpie intern über Xamarin für den letzten drei Jahren. Als Beweis der Leistungsfähigkeit des Ziels Sharpie APIs, die in Xamarin.iOS und Xamarin.Mac nach iOS 8, Mac OS X 10.10 eingeführt und WatchOS 2.0 wurden vollständig mit Ziel Sharpie einem Bootstrapping unterzogen. Xamarin basiert stark auf Ziel Sharpie intern zum Erstellen von eigenen Produkten.

Ziel-Sharpie ist jedoch ein sehr komplexen Tool, das erfordert erweiterte Kenntnisse der Objective-C und C#, wie der Clang Compiler in der Befehlszeile verwenden und im Allgemeinen wie systemeigene Bibliotheken zusammengestellt werden. Aufgrund dieser hohe Balken wir sind, dass eine GUI-Assistent legt die falschen Erwartungen und als solche Ziel Sharpie ist derzeit nur als ein Befehlszeilentool verfügbar.



## <a name="related-links"></a>Verwandte Links

- [Objektive Sharpie download](https://dl.xamarin.com/objective-sharpie/ObjectiveSharpie.pkg)
- [Exemplarische Vorgehensweise: Binden einer Objective-C-Bibliothek](~/ios/platform/binding-objective-c/walkthrough.md)
- [Binden von Objective-C-Bibliotheken](~/cross-platform/macios/binding/objective-c-libraries.md)
- [Weitere Informationen zu](~/cross-platform/macios/binding/overview.md)
- [Bindung Typen-Referenzhandbuch](~/cross-platform/macios/binding/binding-types-reference.md)
- [Xamarin für Objective-C-Entwickler](~/ios/get-started/objective-c-developers/index.md)