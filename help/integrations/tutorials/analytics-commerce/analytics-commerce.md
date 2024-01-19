---
title: Integrieren [!DNL Analytics] mit [!DNL Commerce] Tutorial
description: Erfahren Sie mehr über die Integration von  [!DNL Analytics]  mit  [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integration" type="positive"
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 3%

---

# Integration von [!DNL Analytics] mit [!DNL Commerce]

## ErstOnboarding

Diese Anweisungen dienen zum Adobe [!DNL Commerce] Von Cloud gehostete Projekte. Das selbstständige Hosting kann in gewissem Umfang variieren, doch der Gesamtprozess sollte ähnlich sein.

1. Sehen Sie sich den Code in Ihrer lokalen Umgebung an
1. Verwenden von Composer und Installationsmodul
1. Befolgen Sie hier die einzelnen Anweisungen und geben Sie nach Abschluss zurück, um die verbleibenden Schritte abzuschließen.
   [Installieren und Konfigurieren von Experience [!DNL Platform] Connector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Composer.json erstellen und in Cloud Composer.lock-Dateien
1. Stellen Sie sicher, dass sich das Modul in den Staging- und/oder Produktionsumgebungen befindet. Melden Sie sich dazu im Admin-Bereich von Adobe an. [!DNL Commerce] und nach diesen neuen Abschnitten unter System > Dienste suchen
   ![Erlebnis [!DNL Platform] Connector-Erweiterung](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Konfigurieren Sie das Modul mit Ihren Anmeldedaten aus dem Adobe heraus. [!DNL Commerce] Backoffice.
   * Zuerst [!DNL Commerce] Konfigurationen des Services-Connectors, wie unten dargestellt.
     ![[!DNL Commerce] Einrichtung von Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Dann das Erlebnis [!DNL Platform] Connector-Einstellungen, wie unten dargestellt.
     ![Erlebnis [!DNL Platform] Connector](./assets/analytics-commerce/experience-platform-connector.png)

Weitere Informationen zu den einzelnen Phasen und Schritten des Einstiegsprozesses finden Sie in den Anweisungen unter [Erlebnis [!DNL Platform] Connector - Übersicht](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html?lang=de){target="_blank"}. Das Erlebnis [!DNL Platform] Das Connector-Tutorial behandelt jeden Abschnitt ausführlich und beantwortet alle Fragen, die Sie haben. Verwenden Sie dieses Tutorial für die restlichen Schritte zur schnellen Einrichtung.

## Konfiguration von Experience Edge und Adobe [!DNL Analytics]

1. Stellen Sie sicher, dass Ihr Unternehmen Zugriff auf Adobe hat (und haben). [!DNL Analytics]. Dies lässt sich bestätigen, indem Sie die [Adobe Experience Cloud-Homepage](https://experience.adobe.com/) und auf den Anwendungsschalter (neun Punkte) in der oberen Navigation klicken.

1. Neue Report Suite in Adobe erstellen [!DNL Analytics]oder identifizieren Sie die ID der Report Suite, die Sie per Push senden [!DNL Commerce] Daten in. Weitere Informationen finden Sie in einem Tutorial zu [Erstellen einer neuen Report Suite](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=de). Sie benötigen diese Report Suite-ID im Datastream-Schritt unten.

1. Navigieren Sie zum [Adobe-Erlebnis [!DNL Platform] Benutzeroberfläche](https://platform.adobe.com) wenn Sie Zugriff auf Erlebnis haben [!DNL Platform]. Wenn Sie keinen Zugriff auf diese Benutzeroberfläche haben, können Sie alle erforderlichen Schritte ausführen, die unten im Adobe-Erlebnis aufgeführt sind. [!DNL Platform] [Datenerfassungsoberfläche](https://experience.adobe.com/#/data-collection).

1. Erstellen oder aktualisieren Sie Ihr XDM-Schema mit [!DNL Commerce]-spezifische Feldergruppen. Weitere Informationen zum Erstellen eines Schemas finden Sie unter [&quot;Erstellen von Schemas&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=de) Tutorial.
   * Sie müssen dieses Schema aus den Optionen im unten stehenden Schritt zum Datenspeicher auswählen. Um ein Schema zu erstellen, sehen Sie in der linken Spalte unter **Data Management** und suchen **Schemas**. Klicken Sie oben rechts in der Benutzeroberfläche auf **Schema erstellen**. Wählen Sie XDM ExperienceEvent aus.
   * Nachdem Sie ein neues Schema erstellt haben, fügen Sie die [!DNL Commerce] Feldergruppen. Suchen Sie links in der Benutzeroberfläche nach Feldergruppen und klicken Sie auf **Hinzufügen**
      * Bei der Suche können Sie durch Eingabe von `ExperienceEvent Commerce`
      * Wählen Sie die **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** durch Ankreuzen des Kontrollkästchens
      * Klicken Sie anschließend auf **Feldergruppen hinzufügen** oben rechts zum Speichern und Fortsetzen

1. Optional (und nur, wenn Sie sich im Erlebnis befinden) [!DNL Platform] -Schnittstelle) - Erstellen eines neuen Datensatzes
   * Mit diesem Schritt können Sie die [!DNL Commerce] Daten in das Erlebnis [!DNL Platform] (getrennt vom Einbringen der Daten in die Adobe [!DNL Analytics]). Führen Sie diesen Schritt aus, wenn Sie Zugriff auf Erlebnis haben. [!DNL Platform]und planen die Verwendung der [!DNL Commerce] Daten im Erlebnis [!DNL Platform]-unterstützte Anwendungen, wie Echtzeit-Kundendaten [!DNL Platform], Customer Journey [!DNL Analytics]oder Journey Optimizer.
   * Sie müssen diesen Datensatz aus den Optionen im unten stehenden Schritt zum Datenspeicher auswählen.
   * Unter der linken Spalte **Data Management** in der linken Navigation, wählen Sie **Datensätze**.
   * Klicks **Datensatz erstellen** oben rechts. Wählen Sie die **Datensatz aus Schema erstellen** -Option.
   * Suchen und verwenden Sie das Schema, das Sie im letzten Schritt erstellt haben

1. Erstellen Sie den Datenspeicher, um den [!DNL Commerce] Daten an Adobe [!DNL Analytics]
   * Unter dem **Datenerfassung** in der linken Spalte, wählen Sie **Datenspeicher**.
   * Klicks **Neuer Datenspeicher** oben rechts in der Benutzeroberfläche.
   * Geben Sie einen Namen und eine optionale Beschreibung ein.
   * Suchen und wählen Sie das Schema aus, das Sie im vorherigen Schritt erstellt/identifiziert haben.
   * Fügen Sie alle gewünschten erweiterten Optionen hinzu. Weitere Informationen zu den erweiterten Optionen finden Sie im [Dokumentation](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=de).
   * Klicks **Speichern** , um fortzufahren.
   * Klicks **Dienst hinzufügen** und wählen **Adobe[!DNL Analytics]** im Dropdown-Feld.
   * Klicks **Report Suite hinzufügen** und geben Sie die Report Suite-ID ein, die Sie in einem vorherigen Schritt erstellt/identifiziert haben. Sie können mehr als eine Report Suite hinzufügen, wenn die Daten in mehrere Report Suites fließen sollen.
   * Wenn Sie einen Datensatz in einem vorherigen Schritt erstellt haben, klicken Sie optional auf **Dienst hinzufügen** Wählen Sie erneut **Adobe-Erlebnis[!DNL Platform]** aus dem Dropdown-Feld. Wählen Sie im Feld Ereignis-Datensatz den zuvor erstellten Datensatz aus.
   * Speichern Sie den Datastream.

1. Zum Schluss, um Ihre [!DNL Commerce] Daten verwenden, müssen Sie unter Adobe zu Analysis Workspace navigieren. [!DNL Analytics], erstellen Sie ein Projekt, wählen Sie Ihre Report Suite aus und fügen Sie Freiformtabellen und andere Visualisierungen hinzu, um Ihre [!DNL Commerce] Daten. Die folgende Abbildung zeigt ein Beispiel einer Tabelle, die Sie in Analysis Workspace erstellen können.

   ![[!DNL Analytics] Screenshot einiger Commerce-Daten](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Im Folgenden finden Sie einige zusätzliche Ressourcen, die Sie bei der Arbeit in Analysis Workspace unterstützen:

   * [Analysis Workspace – Übersicht](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Workspace-Projekt von Grund auf neu erstellen](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Verwenden von Tabellen, Visualisierungen und Bedienfeldern in Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Anwendungsfälle für die Visualisierung](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Darüber hinaus gibt es kostenlose Kurse auf Experience League. Siehe [!DNL Analytics] verfügbare Kurse [HIER](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses).
