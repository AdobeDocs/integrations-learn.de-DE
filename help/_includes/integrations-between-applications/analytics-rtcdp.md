---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Integrieren von Adobe [!DNL Analytics] mit Echtzeit-Kundendaten [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

Die Integration von Adobe [!DNL Analytics] in Adobe Echtzeit-Kundendaten [!DNL Platform] (Real-Time CDP) bietet Unternehmen mehrere Vorteile, die ihre Kundenerfahrungen und Marketingbemühungen verbessern möchten. Im Folgenden finden Sie einige der wichtigsten Vorteile:

+ **Verbessertes Zielgruppen-Targeting und Personalisierung**: Präzise Marketing auf Geräten und Kanälen, maßgeschneiderte Nachrichten für eine optimierte Interaktion.
+ **Verbesserte Optimierung der Landingpage**: Angepasste Erlebnisse basierend auf Gerät und Verhalten, wodurch die Benutzerzufriedenheit und Konversion gesteigert werden.
+ **Nahtlose Aktivierung der Audience**: Verwenden Sie Kundenprofile, um über bevorzugte Kanäle effektives Targeting zu ermöglichen und relevante Nachrichten zu versenden.

Durch die Kombination von Adobe [!DNL Analytics] und Real-Time CDP können Unternehmen ihre Marketingbemühungen auf die nächste Stufe bringen, personalisierte Erlebnisse bereitstellen, die Kundeninteraktion steigern und Konversionen über verschiedene digitale Touchpoints hinweg optimieren.

<table>
    <thead>
        <tr>
            <th>Experience Cloud-Anwendungen</th>
            <th>Integration mit</th>
            <th>Verwendungsbereiche</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] mit Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Quell-Connector für Erlebnis [!DNL Platform]</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Empfohlener Ansatz für Kunden, die bereits Adobe [!DNL Analytics] implementiert haben und möchten, dass diese Daten am schnellsten in Erlebnis [!DNL Platform] aufgenommen werden, damit sie im Echtzeit-Kundenprofil verwendet werden.</li>
                <li>Wenn die Datenverfügbarkeit für das Echtzeit-Kundenprofil zwischen 2 und 30 Minuten ab dem Zeitpunkt der Datenerfassung beträgt und die Verfügbarkeit für den Data Lake bis zu 90 Minuten beträgt.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Einfacher, von der Benutzeroberfläche initiierter Workflow.</li>
                <li>Zuordnen der Benutzeroberfläche zum Kopieren von [!DNL Analytics] Props und eVars in neue XDM-Felder.</li>
                <li>Schnellste Möglichkeit, Wert aus dem Echtzeit-Kundenprofil und der Journey des Kunden zu erhalten [!DNL Analytics].</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Erlebnis [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Empfohlener Ansatz für neue [!DNL Analytics] -Implementierungen oder für die Implementierung einer langfristigen Strategie.</li>
                <li>Sendet Daten direkt von einem Gerät an das Erlebnis [!DNL Platform], indem das AEP Web SDK, das AEP Mobile SDK oder die Edge Network Server-API verwendet werden.</li>
                <li>Neue oder vorhandene Kunden, die für das Echtzeit-Kundenprofil eine Datenverfügbarkeit von [!DNL Analytics] benötigen, um dieselben Anwendungsfälle für die Personalisierung der nächsten und nächsten Seite zu unterstützen.</li>
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
