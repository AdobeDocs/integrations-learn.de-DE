---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Integration von [!DNL Analytics] und Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Durch die Aktivierung dieser Integration und die Server-seitige Weiterleitung von Adobe-[!DNL Analytics] an den Audience Manager erhält Audience Manager eine seiner wichtigsten Datenquellen, nämlich Online-Kundenverhaltensdaten. Diese Daten können dann mit anderen Daten kombiniert werden, z. B. Erstanbieter-CRM-Daten oder Partnerdaten von Drittanbietern, um umfangreiche Kundensegmente zu erstellen. Audience Manager Darüber hinaus werden Besuchersegmente in der Antwort zur weiteren Besucheranalyse an die Web-Seite zurückgesendet. Beide wertvollen Anwendungsfälle werden nachfolgend beschrieben.

Die Integration von Adobe [!DNL Analytics] und Audience Manager bietet folgende Vorteile:

+ **Erweiterte Segmentierung**: Kombinieren Sie Adobe-[!DNL Analytics]- und Audience Manager-Daten, um präzise, personalisierte Zielgruppensegmente in Marketing-Kampagnen zu erhalten.
+ **Einheitliche Kundenprofile**: Integrieren Sie Datenquellen, um Interaktionen und Verhaltensweisen zu verstehen, und erstellen Sie umfassende Kundenprofile.
+ **Verbesserte Anzeigeneffektivität**: Optimieren Sie Anzeigen mit datengesteuertem Targeting durch die Integration von Adobe-[!DNL Analytics] und Audience Manager.
+ **Datengesteuerte Entscheidungen**: Informieren Sie Entscheidungen durch detaillierte Einblicke und das Zusammenführen von Adobe-[!DNL Analytics]- und Audience Manager-Daten.
+ **Personalisierte Erlebnisse**: Passen Sie Ihre Inhalte und Angebote an und bereichern Sie mithilfe beider Plattformen die Kundeninteraktionen über Touchpoints hinweg.

Insgesamt bringt diese Integration wertvolle Daten und Zielgruppeneinblicke zusammen. Es ermöglicht Unternehmen, zielgerichtetere und relevantere Marketing-Kampagnen zu erstellen und dabei ein tieferes Verständnis der Vorlieben und Verhaltensweisen ihrer Kunden zu gewinnen.

## Allgemeine Integrationen

<table>
    <thead>
        <tr>
            <th>Experience Cloud-Anwendungen</th>
            <th>Integriert mit</th>
            <th>Verwendungszeitpunkt</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] Senden von Daten an Audience Manager </a>
            </td>
            <td>Adobe [!DNL Analytics] Tags-Erweiterung oder AppMeasurement.js mit aktivierter Server-seitiger Weiterleitung</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Wenn Sie Adobe-[!DNL Analytics]-Daten an Audience Manager senden möchten, um Segmente zu erstellen, die für andere Adobe Experience Cloud-Ziele, personenbasierte Ziele oder andere gerätebasierte und benutzerdefinierte Ziele, die von Audience Manager unterstützt werden, freigegeben werden können.</li>
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
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=de" target="_blank" rel="noreferrer">Audience Manager beim Zurücksenden von Daten an [!DNL Analytics]</a>
            </td>
            <td>Adobe [!DNL Analytics] Tags-Erweiterung oder AppMeasurement.js mit aktivierter Server-seitiger Weiterleitung</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Wenn Sie Segmente von Audience Manager für [!DNL Analytics] freigeben möchten, um Informationen zu Zielgruppenerkennung, Segmentierung und Optimierung bereitzustellen.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Verwenden Sie Audience Manager-Segmente, die demografische Daten von Drittanbietern in [!DNL Analytics] enthalten.</li>
                    <li>Verwenden Sie Audience Manager-Segmente, die Kampagnendaten von Werbeservern in [!DNL Analytics] enthalten.</li>
                    <li>Verwenden Sie Audience Manager-Segmente, die integrierte CRM-Daten in [!DNL Analytics] enthalten.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
