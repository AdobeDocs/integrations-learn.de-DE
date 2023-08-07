---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 1%

---


# Adobe integrieren [!DNL Analytics] mit Echtzeit-Kundendaten [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

Integration von Adobe [!DNL Analytics] mit Adobe-Echtzeit-Kundendaten [!DNL Platform] (Real-Time CDP) bietet Unternehmen, die ihre Kundenerfahrungen und Marketingbemühungen verbessern möchten, mehrere Vorteile. Im Folgenden finden Sie einige der wichtigsten Vorteile:

+ **Verbessertes Zielgruppen-Targeting und Personalisierung**: Präzise Marketing auf Geräten und Kanälen, maßgeschneiderte Nachrichten für eine optimierte Interaktion.
+ **Verbesserte Optimierung der Landingpage**: Maßgeschneiderte Erlebnisse auf der Grundlage von Gerät und Verhalten, die die Benutzerzufriedenheit und Konversion steigern.
+ **Nahtlose Aktivierung der Zielgruppe**: Verwenden Sie Kundenprofile für ein effektives Targeting über bevorzugte Kanäle und senden Sie relevante Nachrichten.

Durch Kombination von Adobe [!DNL Analytics] und Real-Time CDP können Unternehmen ihre Marketingbemühungen auf die nächste Stufe bringen, personalisierte Erlebnisse bereitstellen, die Kundeninteraktion steigern und Konversionen über verschiedene digitale Touchpoints hinweg optimieren.

<table>
    <thead>
        <tr>
            <th>Experience Cloud Apps</th>
            <th>Integration mit</th>
            <th>Verwendungsbereiche</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] mit Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Erlebnis [!DNL Platform] Quell-Connector</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Empfohlener Ansatz für Kunden, die die Adobe bereits implementiert haben [!DNL Analytics]und möchten die schnellste Methode zur Aufnahme dieser Daten in Experience Platform [!DNL Platform] zur Verwendung im Echtzeit-Kundenprofil.</li>
                <li>Wenn die Datenverfügbarkeit für das Echtzeit-Kundenprofil zwischen 2 und 30 Minuten ab dem Zeitpunkt der Datenerfassung beträgt und die Verfügbarkeit für den Data Lake bis zu 90 Minuten beträgt.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Einfacher, von der Benutzeroberfläche initiierter Workflow.</li>
                <li>Zuordnen der zu kopierenden Benutzeroberfläche [!DNL Analytics] Props und eVars in neue XDM-Felder ein.</li>
                <li>Schnellste Möglichkeit, Wert aus dem Echtzeit-Kundenprofil und der Journey zu erhalten [!DNL Analytics].</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Erlebnis [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Empfohlener Ansatz für neue [!DNL Analytics] Implementierungen oder wenn Sie eine langfristige Strategie implementieren möchten.</li>
                <li>Sendet Daten direkt von einem Gerät an das Erlebnis [!DNL Platform] unter Verwendung des AEP Web SDK, AEP Mobile SDK oder der Edge Network Server-API.</li>
                <li>Neue oder vorhandene Kunden, die [!DNL Analytics] Datenverfügbarkeit für das Echtzeit-Kundenprofil , um dieselben und die nächsten Anwendungsfälle für die Personalisierung der Seite zu unterstützen.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Bietet die umfassendste Kontrolle über die erfassten Daten zur Unterstützung Ihrer Anwendungsfälle.</li>
                <li>Clientseitige Daten können einfach XDM-Feldern zugeordnet werden.</li>
                <li>Schnellste Datenverfügbarkeit für das Echtzeit-Kundenprofil.</li>
            </ul>
        </td>
    </tr>            
</table>
