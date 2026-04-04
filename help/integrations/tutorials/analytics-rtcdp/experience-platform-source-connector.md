---
title: Tutorial  [!DNL Analytics]  Integration und Echtzeit-Kundendaten  [!DNL Platform]  Experience  [!DNL Platform] -Quell-Connector
description: Erfahren Sie, wie Sie Adobe  [!DNL Analytics]  Echtzeit-Kundendaten  [!DNL Platform]  Experience  [!DNL Platform] -Quell-Connector integrieren.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integration" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
source-git-commit: ae78e4a9f706ce315a87715302f561ccedc858e9
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 13%

---

# Integrieren von Adobe [!DNL Analytics] und Real-time Customer Data [!DNL Platform] mit dem Quell-Connector von Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/de?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Schemata erstellen</a> für aufzunehmende Daten.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen von </a>) für aufzunehmende Daten.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=de" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie die richtigen Identitäten und Identity-Namespaces im Schema</a> um sicherzustellen, dass die aufgenommenen Daten mit einem einheitlichen Profil verknüpft werden können.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren der Schemata und Datensätze für das Profil</a>.</li>
    <li>Nehmen Sie [!DNL Analytics] Daten mithilfe des <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=de" _target="_blank" rel="noopener noreferrer">Quell-Connectors für Adobe [!DNL Analytics] in Experience Platform </a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen von Segmenten in Experience [!DNL Platform].</a> Das System bestimmt automatisch, ob das Segment als Batch (Daten-Connector) oder Streaming (Edge-Netzwerk) ausgewertet wird.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=de" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie Ziele für die Freigabe von Profilattributen und Zielgruppenmitgliedschaften für die gewünschten Ziele.</a></li>   
</ol>

>[!NOTE]
>
>In den standardmäßigen Workflow-Schritten für den Quell-Connector von Adobe [!DNL Analytics] wird das Schema und der Datensatz erstellt, die zum Aufnehmen der Daten aus [!DNL Analytics] Istzustand verwendet werden. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert das Erstellen benutzerdefinierter Attribute. Befolgen Sie daher die Sequenz der Schritte vollständig.
