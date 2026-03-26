---
title: Integrieren  [!DNL Analytics]  Echtzeit-Kundendaten mit  [!DNL Platform]  Tutorial zu Experience [!DNL Platform] Edge
description: Erfahren Sie, wie Sie  [!DNL Analytics]  Adobe mit Echtzeit-Kundendaten  [!DNL Platform]  AEP Web SDK, AEP Mobile SDK oder der Edge Network Server-API integrieren.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integration" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
source-git-commit: 7fffc0b887164645ab16fe94d2f82a657fcc9d64
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 10%

---

# Tutorial zur Integration von Adobe [!DNL Analytics] und Real-time Customer Data [!DNL Platform] mit Experience [!DNL Platform] Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Schemata erstellen</a> für aufzunehmende Daten.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Erstellen von </a>) für aufzunehmende Daten.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie die richtigen Identitäten und Identity-Namespaces im Schema</a> um sicherzustellen, dass die aufgenommenen Daten mit einem einheitlichen Profil verknüpft werden können.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren der Schemata und Datensätze für das Profil</a>.</li>
    <li>Nehmen Sie Daten mit einer der folgenden Methoden in Experience [!DNL Platform] auf:</li>
        <ul>
           <li>Experience [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=de" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Checkliste</a></li>
                </ul>
            <li>Experience [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Checkliste</a></li>
                </ul></li>
            <li>Edge Network-Server-API:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">Erstellen von Segmenten in Experience [!DNL Platform].</a> Das System bestimmt automatisch, ob das Segment als Batch (Daten-Connector) oder Streaming (Edge-Netzwerk) ausgewertet wird.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie Ziele für die Freigabe von Profilattributen und Zielgruppenmitgliedschaften für die gewünschten Ziele.</a></li>
</ol>

>[!NOTE]
>
>In den standardmäßigen Workflow-Schritten für den Quell-Connector von Adobe [!DNL Analytics] wird das Schema und der Datensatz erstellt, die zum Aufnehmen der Daten aus [!DNL Analytics] Istzustand verwendet werden. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert das Erstellen benutzerdefinierter Attribute. Befolgen Sie daher die Sequenz der Schritte vollständig.
