---
title: Vorläufige Benachrichtigungen in Xamarin.iOS
description: Dieses Dokument beschreibt, wie Sie Xamarin.iOS zum Arbeiten mit vorläufigen Benachrichtigungen zu verwenden. Vorläufige Benachrichtigungen, eingeführt in iOS 12, können Anwendungen ohne explizite Benutzerberechtigungen quiet Benachrichtigungen.
ms.prod: xamarin
ms.assetid: 5DCB36B9-2637-48AE-8FC0-F6124F08AC48
ms.technology: xamarin-ios
author: lobrien
ms.author: laobri
ms.date: 9/4/2018
ms.openlocfilehash: 31b4c6e98945cd7b5dd4cea8be6f5e3857444f78
ms.sourcegitcommit: e268fd44422d0bbc7c944a678e2cc633a0493122
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2018
ms.locfileid: "50131679"
---
# <a name="provisional-notifications-in-xamarinios"></a>Vorläufige Benachrichtigungen in Xamarin.iOS

Vorläufige Benachrichtigungen können apps, um Benachrichtigungen ohne explizite vorab-Zustimmung des Benutzers. Diese Benachrichtigungen unauffällig eingehen, und zeigen nur in der Mitteilungszentrale zur Verfügung, die Benutzer, die sie vor der Aktivierung für oder gegen die Fortführung Vorschau anzeigen können.

In Mitteilungszentrale zur Verfügung können Benutzer angeben, dass eine app beendet werden soll Übermittlung von Benachrichtigungen der vorläufigen, weiterhin vorläufig bereitstellen oder mit der Bereitstellung werden hervorgehoben.

## <a name="sample-app-redgreennotifications"></a>Beispiel-app: RedGreenNotifications

Sehen Sie sich die [RedGreenNotifications](https://developer.xamarin.com/samples/monotouch/iOS12/RedGreenNotifications) Beispielapp, die vorläufige Benachrichtigungen sendet.

## <a name="sending-provisional-notifications"></a>Vorläufige Senden von Benachrichtigungen

Um vorläufige Benachrichtigungen senden, bieten `UNAuthorizationOptions.Provisional` als Option für die [`RequestAuthorization`](https://developer.xamarin.com/api/member/UserNotifications.UNUserNotificationCenter.RequestAuthorization/)
Methode der `UNUserNotificationCenter`:

```csharp
public override bool FinishedLaunching(UIApplication application, NSDictionary launchOptions)
{
    UNUserNotificationCenter center = UNUserNotificationCenter.Current;
    var options = UNAuthorizationOptions.Alert | UNAuthorizationOptions.Sound | UNAuthorizationOptions.Provisional;
    center.RequestAuthorization(options, (bool success, NSError error) => {
        // ...
    );
    return true;
}
```

Wenn der Benutzer vorläufige Benachrichtigungen an gut sichtbaren Übermittlung, stuft die `UNAuthorizationOptions` an übergebenen Werte `RequestAuthorization` bestimmt die neue Einstellungen für die Übermittlung von Benachrichtigungen (im obigen Code `UNAuthorizationOptions.Alert` und `UNAuthorizationOptions.Sound`).

## <a name="related-links"></a>Verwandte Links

- [Beispiel-app – RedGreenNotifications](https://developer.xamarin.com/samples/monotouch/iOS12/RedGreenNotifications)
- [Framework für Benutzerbenachrichtigungen in Xamarin.iOS](~/ios/platform/user-notifications/index.md)
- ["Usernotifications" (Apple)](https://developer.apple.com/documentation/usernotifications?language=objc)
- [Neuerungen in Benutzerbenachrichtigungen (WWDC 2018)](https://developer.apple.com/videos/play/wwdc2018/710/)
- [Bewährte Methoden und Neuigkeiten in Benutzerbenachrichtigungen (WWDC 2017)](https://developer.apple.com/videos/play/wwdc2017/708/)
- [Generieren eine Remotebenachrichtigung (Apple)](https://developer.apple.com/documentation/usernotifications/setting_up_a_remote_notification_server/generating_a_remote_notification)
