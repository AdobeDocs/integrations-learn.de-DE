---
title: Integrieren von Adobe [!DNL Analytics] und Kunden-Journey [!DNL Analytics] mit dem Tutorial zu Experience [!DNL Platform] Edge
description: Erfahren Sie, wie Sie Adobe [!DNL Analytics] mithilfe der AEP Web SDK, AEP Mobile SDK oder der Edge Network Server-API mit Kunden-Journey-[!DNL Analytics] integrieren.
solution: Customer Journey Analytics, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt:
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integration" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
TQID: 'https://experienceleague.adobe.com/ClZddWXeWp51gWTBjRDQBZ2xNiO1bTRq-AoAdmucNEg'
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
  - id: e98b7246-966c-4318-9e95-cad2f7a17dc7
    internal-label: Customer Journey Analytics
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
    internal-label: Metrics
  - id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5e
    internal-label: Integrations
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
    internal-label: Integrations
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
    internal-label: API
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
    internal-label: Experience Cloud integration
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 4c51eef6f89060dc633dede5ea23e0f3ab445d0b
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 16%
---
# Integrieren von Adobe [!DNL Analytics] und Kunden-Journey [!DNL Analytics] mit dem Tutorial zu Experience [!DNL Platform] Edge

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
    <li><i>(optional)</i>. Wenn Sie mehrere Datensätze verwenden, fügen Sie die Personen-IDs zusammen, um <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">einen kombinierten Datensatz zu generieren</a>. Überspringen Sie diesen Schritt, wenn Sie einen einzelnen [!DNL Analytics]-Datensatz verwenden oder wenn für alle Datensätze, die Sie in Kunden-Journey-[!DNL Analytics] verwenden möchten, eine gemeinsame Kennung vorhanden ist.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen einer Verbindung</a> in Kunden-Journey-[!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Erstellen einer Datenansicht</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">Konfigurieren der Komponenteneinstellungen</a> und <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">Formatmetriken</a> in Kunden-Journey [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=de" _target="_blank" rel="noopener noreferrer">Erstellen Sie ein Projekt in Kunden-Journey [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>In den standardmäßigen Workflow-Schritten für den Quell-Connector von Adobe [!DNL Analytics] wird das Schema und der Datensatz erstellt, die zum Aufnehmen der Daten aus [!DNL Analytics] Istzustand verwendet werden. Daher werden die ersten beiden Schritte vom System verarbeitet. Der Zuordnungs-Workflow erfordert das Erstellen benutzerdefinierter Attribute. Befolgen Sie daher die Sequenz der Schritte vollständig.
