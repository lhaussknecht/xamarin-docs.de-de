---
title: Wo kann ich mein Android SDK-Verzeichnissen festlegen?
ms.topic: article
ms.prod: xamarin
ms.assetid: 6A9DE6E9-3E27-4DD2-87D2-34E95E5D401C
ms.technology: xamarin-android
author: mgmclemore
ms.author: mamcle
ms.date: 11/16/2017
ms.openlocfilehash: 0113cc15bf1de5e0e668b05c2b0288a6ead141b5
ms.sourcegitcommit: 30055c534d9caf5dffcfdeafd6f08e666fb870a8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2018
---
# <a name="where-can-i-set-my-android-sdk-locations"></a>Wo kann ich mein Android SDK-Verzeichnissen festlegen?

# <a name="visual-studiotabvswin"></a>[Visual Studio](#tab/vswin)

Wechseln Sie in Visual Studio zu **Extras > Optionen > Xamarin > Android-Einstellungen** anzeigen und Festlegen der Android-SDK-Verzeichnis:

[![Beispiel für Registerkarte "Empfangsspeicherorte" in den Voreinstellungen](android-sdk-location-images/win/01-locations-sml.png)](android-sdk-location-images/win/01-locations.png#lightbox)

Der Standardspeicherort für jeden Pfad lautet wie folgt:

- Java Development Kit Speicherort: 

    **C:\\Program Files\\Java\\jdk1.8.0_131**

- Android SDK-Verzeichnis: 

    **C:\\Programme (x86)\\Android\\android-sdk**

- Android-NDK Speicherort: 

    **"C:"\\"ProgramData"\\Microsoft\\AndroidNDK64\\Android-Ndk-r13b**

Beachten Sie, dass die Versionsnummer der NDK variieren kann. Beispielsweise anstelle von **Android-Ndk-r13b**, es ist möglicherweise eine frühere Version wie z. B. **Android-Ndk-r10e**.

Um den Speicherort des Android SDK festzulegen, geben Sie den vollständigen Pfad des Android SDK-Verzeichnis, in dem **Android SDK-Verzeichnis** Feld. Sie navigieren Sie im Datei-Explorer zu dem Android SDK, aus der Adressleiste den Pfad kopieren und fügen Sie diesen Pfad in der **Android SDK-Verzeichnis** Feld.
Angenommen, Ihr Android-SDK-Speicherort zur ist **"c:"\\Benutzer\\Benutzername\\AppData\\lokale\\Android\\Sdk**, deaktivieren Sie den alten Pfad in der  **Android SDK-Verzeichnis** Feld, fügen Sie in diesen Pfad, und klicken Sie auf **OK**.

# <a name="visual-studio-for-mactabvsmac"></a>[Visual Studio für Mac](#tab/vsmac)

Wechseln Sie in Visual Studio für Mac zu **Voreinstellungen > Projekte > SDK-Verzeichnissen > Android**. In der **Android** auf die **Speicherorte** Registerkarte anzeigen und Festlegen der SDK-Verzeichnis:

[![Beispiel für Registerkarte "Empfangsspeicherorte" in den Voreinstellungen](android-sdk-location-images/mac/01-locations-sml.png)](android-sdk-location-images/mac/01-locations.png#lightbox)

Der Standardspeicherort für jeden Pfad lautet wie folgt:

- Android SDK-Verzeichnis: 

    **~/Library/Developer/Xamarin/android-sdk-macosx**

- Android-NDK Speicherort: 

    **~/Library/Developer/Xamarin/android-ndk/android-ndk-r14b**

- Speicherort des Java SDK (JDK): 

    **/usr**

Beachten Sie, dass die Versionsnummer der NDK variieren kann. Beispielsweise anstelle von **Android-Ndk-r14b**, es ist möglicherweise eine frühere Version wie z. B. **Android-Ndk-r10e**.

Um den Speicherort des Android SDK festzulegen, geben Sie den vollständigen Pfad des Android SDK-Verzeichnis, in dem **Android SDK-Verzeichnis** Feld. Wählen Sie den Android SDK-Ordner, in der Suche, drücken Sie **STRG +&#8984;+ I** zum Ordner Informationen anzeigen möchten, klicken Sie auf, und ziehen Sie den Pfad auf der rechten Seite des **, in denen:**, kopieren und fügen Sie ihn auf die **Android-SDK Speicherort** Feld der **Speicherorte** Registerkarte. Wenn Ihr Android-SDK-Speicherort am ist beispielsweise **~/Library/Developer/Android/Sdk**, deaktivieren Sie den alten Pfad in der **Android SDK-Verzeichnis** Feld, fügen Sie in diesen Pfad, und klicken Sie auf **OK**.

-----