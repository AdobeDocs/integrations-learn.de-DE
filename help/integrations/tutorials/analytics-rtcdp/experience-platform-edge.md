---
title: Integrieren von [!DNL Analytics] und Echtzeit-Kundendaten [!DNL Platform] in das Tutorial zu Experience [!DNL Platform] Edge
description: Erfahren Sie, wie Sie Adobe [!DNL Analytics] mit Echtzeit-Kundendaten integrieren [!DNL Platform] , indem Sie das AEP Web SDK, das AEP Mobile SDK oder die Edge Network Server API verwenden.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
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
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 3%

---

# Integrieren von Adobe [!DNL Analytics] und Echtzeit-Kundendaten [!DNL Platform] in das Edge-Tutorial zu Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Erstellen Sie Schemas</a> , damit Daten erfasst werden.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Erstellen Sie Datensätze</a> , damit Daten erfasst werden.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie die richtigen Identitäten und Identitäts-Namespaces für das Schema</a>, um sicherzustellen, dass die erfassten Daten einem einheitlichen Profil zugeordnet werden können.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren Sie die Schemas und Datensätze für profile</a>.</li>
    <li>Erfassen von Daten in Erlebnis [!DNL Platform] mit einer der folgenden Methoden:</li>
        <ul>
           <li>Erlebnis [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=de" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Checkliste</a></li>
                </ul>
            <li>Erlebnis [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Checkliste</a></li>
                </ul></li>
            <li>Edge Network Server-API:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">Erstellen Sie Segmente in Erlebnis [!DNL Platform].</a> Das System bestimmt automatisch, ob das Segment als Batch (Data Connector) oder Streaming (Edge-Netzwerk) ausgewertet wird.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie Ziele für die Freigabe von Profilattributen und Zielgruppenmitgliedschaften für die gewünschten Ziele.</a></li>
</ol>

>[!NOTE]
>
>Die standardmäßigen Workflow-Schritte für den Quell-Connector Adobe [!DNL Analytics] erstellen das Schema und den Datensatz, die zur Erfassung der Daten von [!DNL Analytics] &quot;unverändert&quot;verwendet werden. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert die Erstellung benutzerdefinierter Attribute. Befolgen Sie daher die Schritte in vollem Umfang.
