---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Integrieren von Adobe [!DNL Analytics] mit Real-time Customer Data [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

Die Integration von Adobe [!DNL Analytics] mit Adobe Real-time Customer Data [!DNL Platform] (Real-Time CDP) kann Unternehmen, die ihre Kundenerlebnisse und Marketing-Maßnahmen verbessern möchten, mehrere Vorteile bieten. Im Folgenden sind einige der wichtigsten Vorteile aufgeführt:

+ **Optimiertes Zielgruppen-Targeting und Personalisierung**: Präzises Marketing auf Geräten und Kanälen, maßgeschneiderte Botschaften für optimierte Interaktion.
+ **Verbesserte Landingpage-Optimierung**: Maßgeschneiderte Erlebnisse basierend auf Gerät und Verhalten, die die Benutzerzufriedenheit und Konversion steigern.
+ **Nahtlose Zielgruppenaktivierung**: Nutzen Sie Kundenprofile für eine effektive Zielgruppenbestimmung über bevorzugte Kanäle und senden Sie relevante Nachrichten.

Durch die Kombination von Adobe [!DNL Analytics] und Real-Time CDP können Unternehmen ihre Marketing-Maßnahmen auf ein höheres Niveau heben, personalisierte Erlebnisse bereitstellen, die Kundeninteraktion steigern und Konversionen über verschiedene digitale Touchpoints hinweg optimieren.

<table>
    <thead>
        <tr>
            <th>Experience Cloud-Anwendungen</th>
            <th>Integriert mit</th>
            <th>Verwendungszeitpunkt</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] mit Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Quell-Connector für Experience [!DNL Platform]</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Empfohlener Ansatz für Kunden, die bereits Adobe [!DNL Analytics] implementiert haben und die am schnellsten diese Daten in Experience [!DNL Platform] aufnehmen möchten, um sie im Echtzeit-Kundenprofil zu verwenden.</li>
                <li>Wenn die Datenverfügbarkeit für das Echtzeit-Kundenprofil zwischen 2 und 30 Minuten ab dem Zeitpunkt der Datenerfassung betragen kann und die Verfügbarkeit für den Data Lake bis zu 90 Minuten beträgt.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Einfacher, von der Benutzeroberfläche initiierter Workflow.</li>
                <li>Zuordnen der Benutzeroberfläche zum Kopieren [!DNL Analytics] Props und eVars in neue XDM-Felder.</li>
                <li>Schnellste Möglichkeit, vom Echtzeit-Kundenprofil und der Kunden-Journey-[!DNL Analytics] zu profitieren.</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Experience [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Empfohlener Ansatz für neue [!DNL Analytics]-Implementierungen oder wenn Sie eine langfristige Strategie implementieren möchten.</li>
                <li>Sendet Daten mithilfe der AEP Web SDK, AEP Mobile SDK oder der Edge Network Server-API direkt von einem Gerät an Experience [!DNL Platform].</li>
                <li>Neue oder bestehende Kunden, die [!DNL Analytics] Datenverfügbarkeit für das Echtzeit-Kundenprofil benötigen, um Anwendungsfälle für die Personalisierung derselben und der nächsten Seite zu unterstützen.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Bietet ein Höchstmaß an Kontrolle über die erfassten Daten, die zur Unterstützung Ihrer Anwendungsfälle verwendet werden können.</li>
                <li>Client-seitige Daten können einfach XDM-Feldern zugeordnet werden.</li>
                <li>Schnellste Datenverfügbarkeit für das Echtzeit-Kundenprofil.</li>
            </ul>
        </td>
    </tr>            
</table>
