---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Integration von [!DNL Analytics] und Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Durch die Aktivierung dieser Integration und die Server-seitige Weiterleitung von Daten [!DNL Analytics] Adobe an Audience Manager erhält Audience Manager eine seiner wichtigsten Datenquellen, nämlich Online-Kundenverhaltensdaten. Diese Daten können dann mit anderen Daten kombiniert werden, z. B. Erstanbieter-CRM-Daten oder Partnerdaten von Drittanbietern, um umfangreiche Kundensegmente zu erstellen. Darüber hinaus werden Audience Manager-Segmente dann zur weiteren Besucheranalyse in der Antwort an die Web-Seite zurückgesendet. Beide wertvollen Anwendungsfälle werden nachfolgend beschrieben.

Die Integration von Adobe [!DNL Analytics] und Audience Manager bietet folgende Hauptvorteile:

+ **Erweiterte Segmentierung**: Kombinieren Sie Daten aus Adobe [!DNL Analytics] und Audience Manager, um präzise, personalisierte Zielgruppensegmente in Marketing-Kampagnen zu erhalten.
+ **Einheitliche Kundenprofile**: Integrieren Sie Datenquellen, um Interaktionen und Verhaltensweisen zu verstehen, und erstellen Sie umfassende Kundenprofile.
+ **Verbesserte Anzeigeneffektivität**: Optimieren Sie Anzeigen mit datengesteuertem Targeting über die Integration von Adobe [!DNL Analytics] und Audience Manager.
+ **Datengesteuerte Entscheidungen**: Informieren Sie Entscheidungen durch detaillierte Einblicke und das Zusammenführen von Adobe [!DNL Analytics]- und Audience Manager-Daten.
+ **Personalisierte Erlebnisse**: Passen Sie Ihre Inhalte und Angebote an und bereichern Sie mithilfe beider Plattformen die Kundeninteraktionen über Touchpoints hinweg.

Insgesamt bringt diese Integration wertvolle Daten und Zielgruppeneinblicke zusammen. Es ermöglicht Unternehmen, zielgerichtetere und relevantere Marketing-Kampagnen zu erstellen und dabei ein tieferes Verständnis der Vorlieben und Verhaltensweisen ihrer Kunden zu gewinnen.

## Allgemeine Integrationen

<table>
    <thead>
        <tr>
            <th>Experience Cloud-Programme</th>
            <th>Integriert mit</th>
            <th>Verwendungszeitpunkt</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] Senden von Daten an Audience Manager</a>
            </td>
            <td>Tags-Erweiterung für Adobe [!DNL Analytics] oder AppMeasurement.js mit aktivierter Server-seitiger Weiterleitung</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Wenn Sie Adobe-[!DNL Analytics] an Audience Manager senden möchten, um Segmente zu erstellen, die für andere Adobe Experience Cloud-Ziele, personenbasierte Ziele oder andere gerätebasierte und benutzerdefinierte Ziele, die von Audience Manager unterstützt werden, freigegeben werden können.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Geben Sie Segmente für Anzeigenplattformen frei, die in [!DNL Analytics] erfasste Verhaltensattribute enthalten.</li>
                    <li>Reichern Sie Segmente mit [!DNL Analytics] an, um hochwertige kanalübergreifende Segmente zu erstellen, die beim Targeting auf der Site verwendet werden können.</li>
                    <li>Datenschicht [!DNL Analytics] Segmenten, die über Hash-Kennungen wie E-Mail verschlüsselt wurden, um sie auf Social-Media-Plattformen zu verwenden.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager sendet Daten zurück an [!DNL Analytics]</a>
            </td>
            <td>Tags-Erweiterung für Adobe [!DNL Analytics] oder AppMeasurement.js mit aktivierter Server-seitiger Weiterleitung</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Wenn Sie Segmente aus Audience Manager für [!DNL Analytics] freigeben möchten, um Informationen zu Zielgruppenerkennung, Segmentierung und Optimierung bereitzustellen.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Verwenden Sie Audience Manager-Segmente, die demografische Daten von Drittanbietern in [!DNL Analytics] enthalten.</li>
                    <li>Verwenden Sie Audience Manager-Segmente, die Kampagnendaten von Anzeigen-Servern in [!DNL Analytics] enthalten.</li>
                    <li>Verwenden Sie Audience Manager-Segmente, die integrierte CRM-Daten in [!DNL Analytics] enthalten.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
