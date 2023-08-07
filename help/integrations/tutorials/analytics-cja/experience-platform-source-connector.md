---
title: Integrieren [!DNL Analytics] und Customer Journey [!DNL Analytics] mit Erlebnis [!DNL Platform] Quell-Connector-Tutorial
description: Erfahren Sie, wie Sie Adobe integrieren. [!DNL Analytics] mit Customer Journey [!DNL Analytics] Verwenden des Erlebnisses [!DNL Platform] Quell-Connector.
solution: Customer Journey [!DNL Analytics], [!DNL Target]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integration" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 20%

---


# Adobe integrieren [!DNL Analytics] und Customer Journey [!DNL Analytics] mit Erlebnis [!DNL Platform] Quell-Connector

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Erstellen Sie Schemata</a> für aufzunehmende Daten.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen Sie Datensätze</a> für aufzunehmende Daten.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurieren der richtigen Identitäten und Identitäts-Namespaces für das Schema</a> , um sicherzustellen, dass die erfassten Daten einem einheitlichen Profil zugeordnet werden können.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren der Schemata und Datensätze für Profile</a>.</li>
    <li>Daten in Erlebnis aufnehmen [!DNL Platform] mithilfe der <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=de" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] Quell-Connector</a></li>
    <li><i>(Optional)</i>. Wenn Sie mehrere Datensätze verwenden, verknüpfen Sie die Personen-IDs zu <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">einen kombinierten Datensatz generieren</a>. Bei Verwendung einer einzelnen [!DNL Analytics] Datensatz oder wenn eine gemeinsame Kennung über alle Datensätze hinweg vorhanden ist, die Sie in Customer Journey verwenden möchten. [!DNL Analytics], überspringen Sie diesen Schritt.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=de" _target="_blank" rel="noopener noreferrer"></a>Erstellen einer Verbindung in Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Datenansicht erstellen</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">Komponenteneinstellungen konfigurieren</a>, und <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">Formatmetriken</a> in Customer Journey [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Erstellen eines Projekts auf der Journey [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Die standardmäßigen Workflow-Schritte für die Adobe [!DNL Analytics] Quell-Connector erstellt das Schema und den Datensatz, die zur Aufnahme der Daten aus [!DNL Analytics] &quot;as-is&quot;. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert die Erstellung benutzerdefinierter Attribute. Befolgen Sie daher die Schritte in vollem Umfang.
