---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Integration von [!DNL Analytics] und Audience Managern

{{analytics-description}}

{{audience-manager-description}}

Durch die Aktivierung dieser Integration, die serverseitige Weiterleitung von Adobe [!DNL Analytics] -Daten an Audience Manager, erhalten Audience Manager eine der wichtigsten Datenquellen, nämlich Online-Kundenverhaltensdaten. Diese Daten können dann mit anderen Daten kombiniert werden, z. B. Erstanbieter-CRM-Daten oder Partnerdaten von Drittanbietern, um umfangreiche Kundensegmente zu erstellen. Darüber hinaus werden Audience Manager-Segmente in der Antwort zur weiteren Besucheranalyse zurück an die Webseite gesendet. Beide dieser wertvollen Anwendungsfälle werden nachfolgend beschrieben.

Die wichtigsten Vorteile der Integration von Adobe [!DNL Analytics] und Audience Manager sind:

+ **Verbesserte Segmentierung**: Kombinieren Sie Adobe [!DNL Analytics]- und Audience Manager-Daten für präzise, personalisierte Zielgruppensegmente in Marketingkampagnen.
+ **Einheitliche Kundenprofile**: Integrieren Sie Datenquellen, um Interaktionen und Verhaltensweisen zu verstehen, und erstellen Sie umfassende Kundenprofile.
+ **Verbesserte Anzeigeneffizienz**: Optimieren Sie Anzeigen mit datengesteuertem Targeting aus der Adobe [!DNL Analytics]- und Audience Manager-Integration.
+ **Datenbasierte Entscheidungen**: Informieren Sie über detaillierte Einblicke, führen Sie Adobe [!DNL Analytics]- und Audience Manager-Daten zusammen.
+ **Personalisierte Erlebnisse**: Passen Sie Ihre Inhalte und Angebote an und bereichern Sie die Kundeninteraktionen über Touchpoints hinweg mithilfe beider Plattformen.

Insgesamt führt diese Integration wertvolle Daten und Zielgruppeneinblicke zusammen. Sie ermöglicht es Unternehmen, zielgerichtetere und relevantere Marketing-Kampagnen zu erstellen und gleichzeitig ein tieferes Verständnis der Präferenzen und Verhaltensweisen ihrer Kunden zu gewinnen.

## Allgemeine Integrationen

<table>
    <thead>
        <tr>
            <th>Experience Cloud-Anwendungen</th>
            <th>Integration mit</th>
            <th>Verwendungsbereiche</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] Senden von Daten an Audience Manager</a>
            </td>
            <td>Adobe [!DNL Analytics] tags-Erweiterung oder AppMeasurement.js mit aktivierter serverseitiger Weiterleitung</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Wenn Sie Adobe [!DNL Analytics] -Daten an Audience Manager senden möchten, um Segmente zu erstellen, die für andere Adobe Experience Cloud-Ziele, personenbasierte Ziele oder andere gerätebasierte und benutzerdefinierte Ziele, die von Audience Manager unterstützt werden, freigegeben werden können.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Geben Sie Segmente für Anzeigenplattformen frei, die in [!DNL Analytics] erfasste Verhaltensattribute enthalten.</li>
                    <li>Reichern Sie Segmente mit [!DNL Analytics] -Daten an, um hochwertige, kanalübergreifende Segmente zu erstellen, die für das On-site-Targeting verwendet werden.</li>
                    <li>Ebene der [!DNL Analytics] -Daten in Segmente, die von Hash-Kennungen (z. B. E-Mail) zur Verwendung in Social-Media-Plattformen abgeleitet wurden.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager, der Daten an [!DNL Analytics]</a> zurücksendet
            </td>
            <td>Adobe [!DNL Analytics] tags-Erweiterung oder AppMeasurement.js mit aktivierter serverseitiger Weiterleitung</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Wenn Sie Segmente von Audience Manager für [!DNL Analytics] freigeben möchten, um die Zielgruppenerkennung, -segmentierung und -optimierung zu unterstützen.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Verwenden Sie Audience Manager-Segmente, die demografische Daten von Drittanbietern in [!DNL Analytics] -Berichten enthalten.</li>
                    <li>Verwenden Sie Audience Manager-Segmente, die Kampagnendaten von Anzeigen-Servern in [!DNL Analytics] -Berichten enthalten.</li>
                    <li>Verwenden Sie Audience Manager-Segmente, die integrierte CRM-Daten in [!DNL Analytics] -Berichten enthalten.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
