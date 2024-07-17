---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# Integrieren von Adobe [!DNL Analytics] mit Customer Journey [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

Die Integration von Adobe [!DNL Analytics] mit Customer Journey [!DNL Analytics] bietet wichtige Vorteile:

+ **Umfassende Einblicke** in das Verhalten und die Präferenzen von Kunden.
+ **Nahtloses kanalübergreifendes Tracking** für eine ganzheitliche Sicht.
+ **Einheitliche Daten und Berichterstellung** für eine genaue Analyse.
+ **Verbesserte Personalisierung** und verbesserte Kundeninteraktion.
+ **Echtzeitdateneinblicke** für eine agile Entscheidungsfindung.

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
            <td rowspan="2">[!DNL Analytics] und Customer Journey [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Quell-Connector für Erlebnis [!DNL Platform]</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Empfohlener Ansatz für Kunden, die bereits Adobe [!DNL Analytics] implementiert haben und die am schnellsten diese Daten in Erlebnis [!DNL Platform] aufnehmen möchten, um sie in Customer Journey [!DNL Analytics] zu verwenden.</li>
                    <li>Wenn die Datenverfügbarkeit für das Kundenprofil zwischen 2 und 30 Minuten ab dem Zeitpunkt der Datenerfassung liegen kann und die Verfügbarkeit für den Data Lake bis zu 90 Minuten beträgt.</li>
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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Erlebnis [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Empfohlener Ansatz für neue [!DNL Analytics] -Implementierungen oder für die Implementierung einer langfristigen Strategie.</li>
                    <li>Sendet Daten direkt von einem Gerät an das Erlebnis [!DNL Platform], indem das AEP Web SDK, das AEP Mobile SDK oder die Edge Network Server-API verwendet werden.</li>
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
