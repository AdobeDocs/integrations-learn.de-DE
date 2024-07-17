---
title: Integrieren von [!DNL Analytics] und Customer Journey [!DNL Analytics] in das Quell-Connector-Tutorial für Experience [!DNL Platform] 1
description: Erfahren Sie, wie Sie Adobe [!DNL Analytics] mit Customer Journey [!DNL Analytics] integrieren, indem Sie den Experience [!DNL Platform] Quell-Connector verwenden.
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
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 2%

---

# Integrieren von Adobe [!DNL Analytics] und Customer Journey [!DNL Analytics] in den Experience [!DNL Platform]-Quell-Connector

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Erstellen Sie Schemas</a> , damit Daten erfasst werden.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Erstellen Sie Datensätze</a> , damit Daten erfasst werden.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie die richtigen Identitäten und Identitäts-Namespaces für das Schema</a>, um sicherzustellen, dass die erfassten Daten einem einheitlichen Profil zugeordnet werden können.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren Sie die Schemas und Datensätze für profile</a>.</li>
    <li>Erfassen von Daten in Erlebnis [!DNL Platform] mithilfe des Quell-Connectors <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=de" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics]</a></li>
    <li><i>(Optional)</i>. Wenn Sie mehrere Datensätze verwenden, verknüpfen Sie die Personen-IDs mit <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generieren Sie einen kombinierten Datensatz</a>. Wenn Sie einen einzelnen [!DNL Analytics] -Datensatz verwenden oder wenn eine gemeinsame Kennung für alle Datensätze vorhanden ist, die Sie in Customer Journey [!DNL Analytics] verwenden möchten, überspringen Sie diesen Schritt.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen Sie eine Verbindung </a> in Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Erstellen Sie eine Datenansicht</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">konfigurieren Sie die Komponenteneinstellungen</a> und <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">Formatmetriken</a> in Customer Journey [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen Sie ein Projekt unter Customer Journey [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Die standardmäßigen Workflow-Schritte für den Quell-Connector Adobe [!DNL Analytics] erstellen das Schema und den Datensatz, die zur Erfassung der Daten von [!DNL Analytics] &quot;unverändert&quot;verwendet werden. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert die Erstellung benutzerdefinierter Attribute. Befolgen Sie daher die Schritte in vollem Umfang.
