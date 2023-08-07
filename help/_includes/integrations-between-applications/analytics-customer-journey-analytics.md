---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 2%

---


# Adobe integrieren [!DNL Analytics] mit Customer Journey [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

Integration von Adobe [!DNL Analytics] mit Customer Journey [!DNL Analytics] bietet wichtige Vorteile:

+ **Umfassende Erkenntnisse** in Kundenverhalten und -präferenzen.
+ **Nahtloses kanalübergreifendes Tracking** für eine ganzheitliche Sicht.
+ **Einheitliche Daten und Berichterstellung** für eine genaue Analyse.
+ **Verbesserte Personalisierung** und verbesserte Kundeninteraktion.
+ **Echtzeitdateneinblicke** für eine agile Entscheidungsfindung.

## Allgemeine Integrationen

<table>
    <thead>
        <tr>
            <th>Experience Cloud Apps</th>
            <th>Integration mit</th>
            <th>Verwendungsbereiche</th>
            <th>Häufige Anwendungsfälle</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2">[!DNL Analytics] und Customer Journey [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Erlebnis [!DNL Platform] Quell-Connector</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Empfohlener Ansatz für Kunden, die die Adobe bereits implementiert haben [!DNL Analytics]und möchten die schnellste Methode zur Aufnahme dieser Daten in Experience Platform [!DNL Platform] zur Verwendung in Customer Journey [!DNL Analytics].</li>
                    <li>Wenn die Datenverfügbarkeit für das Kundenprofil zwischen 2 und 30 Minuten ab dem Zeitpunkt der Datenerfassung liegen kann und die Verfügbarkeit für den Data Lake bis zu 90 Minuten beträgt.</li>
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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Erlebnis [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Empfohlener Ansatz für neue [!DNL Analytics] Implementierungen oder wenn Sie eine langfristige Strategie implementieren möchten.</li>
                    <li>Sendet Daten direkt von einem Gerät an das Erlebnis [!DNL Platform] unter Verwendung des AEP Web SDK, AEP Mobile SDK oder der Edge Network Server-API.</li>
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
    </tbody>          
</table>
