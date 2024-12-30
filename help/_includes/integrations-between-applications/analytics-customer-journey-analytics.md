---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# Integrieren von Adobe [!DNL Analytics] mit Kunden-Journey [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

Die Integration von Adobe [!DNL Analytics] mit Kunden-Journey [!DNL Analytics] bietet wichtige Vorteile:

+ **Umfassende Einblicke** in Kundenverhalten und -präferenzen.
+ **Nahtloses kanalübergreifendes Tracking** für eine ganzheitliche Sicht.
+ **Einheitliche Daten und Reporting** für eine präzise Analyse.
+ **Verbesserte Personalisierung** und Kundeninteraktion.
+ **Echtzeit-Dateneinblicke** für eine agile Entscheidungsfindung.

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
            <td rowspan="2">[!DNL Analytics] und Kunden-Journey [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Quell-Connector für Experience [!DNL Platform]</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Empfohlener Ansatz für Kunden, die bereits Adobe [!DNL Analytics] implementiert haben und die am schnellsten diese Daten in Experience [!DNL Platform] aufnehmen möchten, um sie in Kunden-Journey-[!DNL Analytics] zu verwenden.</li>
                    <li>Wenn die Datenverfügbarkeit für das Kundenprofil zwischen 2 und 30 Minuten ab dem Zeitpunkt der Datenerfassung betragen kann und die Verfügbarkeit für den Data Lake bis zu 90 Minuten beträgt.</li>
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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Experience [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Empfohlener Ansatz für neue [!DNL Analytics]-Implementierungen oder wenn Sie eine langfristige Strategie implementieren möchten.</li>
                    <li>Sendet Daten mithilfe der AEP Web SDK, AEP Mobile SDK oder der Edge Network Server-API direkt von einem Gerät an Experience [!DNL Platform].</li>
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
    </tbody>          
</table>
