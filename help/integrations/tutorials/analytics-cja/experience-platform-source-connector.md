---
title: Tutorial  [!DNL Analytics]  Integrieren von und Kunden [!DNL Analytics] Journey mit  [!DNL Platform] -Quell-Connector
description: Erfahren Sie, wie Sie Adobe [!DNL Analytics] mit Kunden-Journey  [!DNL Analytics]  Experience  [!DNL Platform] -Quell-Connector integrieren.
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

# Integrieren von Adobe-[!DNL Analytics]- und Kunden-Journey-[!DNL Analytics] mit dem Quell-Connector von Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/de?lang=de#dashboard/learning" _target="_blank" rel="noopener noreferrer">Schemata erstellen</a> für aufzunehmende Daten.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen von </a>) für aufzunehmende Daten.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=de" _target="_blank" rel="noopener noreferrer">Konfigurieren Sie die richtigen Identitäten und Identity-Namespaces im Schema</a> um sicherzustellen, dass die aufgenommenen Daten mit einem einheitlichen Profil verknüpft werden können.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=de" _target="_blank" rel="noopener noreferrer">Aktivieren der Schemata und Datensätze für das Profil</a>.</li>
    <li>Aufnehmen von Daten in Experience [!DNL Platform] mithilfe des <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=de" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics]-Quell-Connectors</a></li>
    <li><i>(optional)</i>. Wenn Sie mehrere Datensätze verwenden, fügen Sie die Personen-IDs zusammen, um <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html?lang=de" _target="_blank" rel="noopener noreferrer">einen kombinierten Datensatz zu generieren</a>. Überspringen Sie diesen Schritt, wenn Sie einen einzelnen [!DNL Analytics]-Datensatz verwenden oder wenn für alle Datensätze, die Sie in Kunden-Journey-[!DNL Analytics] verwenden möchten, eine gemeinsame Kennung vorhanden ist.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen einer Verbindung</a> in Kunden-Journey-[!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen einer Datenansicht</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html?lang=de" _target="_blank" rel="noopener noreferrer">Konfigurieren der Komponenteneinstellungen</a> und <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html?lang=de" _target="_blank" rel="noopener noreferrer">Formatmetriken</a> in Kunden-Journey [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen Sie ein Projekt in Kunden-Journey [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Die standardmäßigen Workflow-Schritte für den Quell-Connector für Adobe-[!DNL Analytics] erstellen das Schema und den Datensatz, die verwendet werden, um die Daten aus [!DNL Analytics] Istzustand aufzunehmen. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert das Erstellen benutzerdefinierter Attribute. Befolgen Sie daher die Sequenz der Schritte vollständig.
