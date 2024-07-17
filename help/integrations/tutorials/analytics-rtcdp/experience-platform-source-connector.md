---
title: Integrieren von [!DNL Analytics] und Echtzeit-Kundendaten [!DNL Platform] in das Quell-Connector-Tutorial für Experience [!DNL Platform] 1
description: Erfahren Sie, wie Sie Adobe [!DNL Analytics] mit Echtzeit-Kundendaten [!DNL Platform] integrieren, indem Sie den Experience [!DNL Platform] Quell-Connector verwenden.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integration" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 2%

---

# Integrieren von Adobe [!DNL Analytics] und Echtzeit-Kundendaten [!DNL Platform] in den Quell-Connector von Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Erstellen Sie Schemas</a> , damit Daten erfasst werden.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Erstellen Sie Datensätze</a> , damit Daten erfasst werden.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie die richtigen Identitäten und Identitäts-Namespaces für das Schema</a>, um sicherzustellen, dass die erfassten Daten einem einheitlichen Profil zugeordnet werden können.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren Sie die Schemas und Datensätze für profile</a>.</li>
    <li>Erfassen Sie [!DNL Analytics] Daten über den Quell-Connector <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=de" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] </a> in die Experience-Plattform.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Erstellen Sie Segmente in Erlebnis [!DNL Platform].</a> Das System bestimmt automatisch, ob das Segment als Batch (Data Connector) oder Streaming (Edge-Netzwerk) ausgewertet wird.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie Ziele für die Freigabe von Profilattributen und Zielgruppenmitgliedschaften für die gewünschten Ziele.</a></li>   
</ol>

>[!NOTE]
>
>Die standardmäßigen Workflow-Schritte für den Quell-Connector Adobe [!DNL Analytics] erstellen das Schema und den Datensatz, die zur Erfassung der Daten von [!DNL Analytics] &quot;unverändert&quot;verwendet werden. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert die Erstellung benutzerdefinierter Attribute. Befolgen Sie daher die Schritte in vollem Umfang.
