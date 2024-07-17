---
title: Tutorial zur Integration von [!DNL Analytics] mit [!DNL Commerce] Tutorial
description: Erfahren Sie, wie Sie [!DNL Analytics] mit [!DNL Commerce] integrieren.
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
ht-degree: 0%

---

# Integrieren von [!DNL Analytics] mit [!DNL Commerce]

## ErstOnboarding

Diese Anweisungen gelten für Adobe [!DNL Commerce] gehostete Cloud-Projekte. Das selbstständige Hosting kann in gewissem Umfang variieren, doch der Gesamtprozess sollte ähnlich sein.

1. Sehen Sie sich den Code in Ihrer lokalen Umgebung an
1. Verwenden von Composer und Installationsmodul
1. Befolgen Sie hier die einzelnen Anweisungen und geben Sie nach Abschluss zurück, um die verbleibenden Schritte abzuschließen.
   [Installieren und Konfigurieren des Experience [!DNL Platform] Connectors](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Composer.json erstellen und in Cloud Composer.lock-Dateien
1. Stellen Sie sicher, dass sich das Modul in der Staging- und/oder Produktionsumgebung befindet.
Sie können dies tun, indem Sie sich beim Admin-Abschnitt von Adobe [!DNL Commerce] anmelden und nach diesen neuen Abschnitten unter System > Dienste suchen.
   ![Erlebnis [!DNL Platform] Connector-Erweiterung](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Konfigurieren Sie das Modul mit Ihren Anmeldedaten aus dem Adobe [!DNL Commerce]-Backoffice heraus.
   * Zuerst die Konfigurationen des Connectors &quot;[!DNL Commerce] Dienste&quot;, wie unten dargestellt.
     ![[!DNL Commerce] Einrichtung des Connectors für Dienste](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Anschließend die Erlebnis [!DNL Platform] -Connector-Einstellungen, wie unten dargestellt.
     ![Erlebnis [!DNL Platform]-Connector](./assets/analytics-commerce/experience-platform-connector.png)

Weitere Informationen zu den einzelnen Phasen und Schritten des Integrationsprozesses finden Sie in den Anweisungen unter [Übersicht über den Erlebnis [!DNL Platform] Connector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"} . Das Erlebnis [!DNL Platform]-Connector-Tutorial behandelt jeden Abschnitt ausführlich und beantwortet alle Fragen, die Sie möglicherweise haben. Verwenden Sie dieses Tutorial für die restlichen Schritte zur schnellen Einrichtung.

## Konfiguration von Experience Edge und Adobe [!DNL Analytics]

1. Stellen Sie sicher, dass Ihr Unternehmen Zugriff auf Adobe [!DNL Analytics] hat (und Sie darüber verfügen). Dies kann bestätigt werden, indem Sie auf der [Adobe Experience Cloud-Homepage](https://experience.adobe.com/) auf den App-Umschalter (neun Punkte) in der oberen Navigation klicken.

1. Erstellen Sie eine neue Report Suite in Adobe [!DNL Analytics] oder identifizieren Sie die ID der Report Suite, an die Sie [!DNL Commerce] -Daten senden werden. Weitere Informationen finden Sie in einem Tutorial zum Erstellen einer neuen Report Suite ](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html). [ Sie benötigen diese Report Suite-ID im Datastream-Schritt unten.

1. Navigieren Sie zur Benutzeroberfläche [Adobe-Erlebnis [!DNL Platform] 2} , wenn Sie Zugriff auf Erlebnis [!DNL Platform] haben. ](https://platform.adobe.com) Wenn Sie keinen Zugriff auf diese Benutzeroberfläche haben, können Sie alle erforderlichen Schritte ausführen, die unten in der Adobe-Erlebnis [!DNL Platform] [Datenerfassungsschnittstelle](https://experience.adobe.com/#/data-collection) aufgeführt sind.

1. Erstellen oder aktualisieren Sie Ihr XDM-Schema mit [!DNL Commerce] spezifischen Feldergruppen. Weitere Informationen zum Erstellen eines Schemas finden Sie im Tutorial [&quot;Schemas erstellen&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=de) .
   * Sie müssen dieses Schema aus den Optionen im unten stehenden Schritt zum Datenspeicher auswählen. Um ein Schema zu erstellen, suchen Sie in der linken Spalte unter **Datenverwaltung** nach **Schemas**. Klicken Sie nun oben rechts in der Benutzeroberfläche auf **Schema erstellen**. Wählen Sie XDM ExperienceEvent aus.
   * Nachdem Sie ein neues Schema erstellt haben, fügen Sie die [!DNL Commerce]-Feldergruppen hinzu. Suchen Sie links in der Benutzeroberfläche nach Feldergruppen und klicken Sie auf **Hinzufügen**
      * Bei der Suche können Sie filtern, indem Sie `ExperienceEvent Commerce` eingeben
      * Wählen Sie die **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** aus, indem Sie das Kontrollkästchen aktivieren.
      * Klicken Sie dann oben rechts auf **Feldergruppen hinzufügen** , um zu speichern und fortzufahren.

1. Optional (und nur, wenn Sie sich in der Erlebnis [!DNL Platform] -Oberfläche befinden) - Erstellen Sie einen neuen Datensatz
   * Mit diesem Schritt können Sie die [!DNL Commerce] -Daten in das Erlebnis [!DNL Platform] übertragen (getrennt vom Einbringen der Daten in Adobe [!DNL Analytics]). Führen Sie diesen Schritt aus, wenn Sie Zugriff auf Erlebnis [!DNL Platform] haben und planen, die [!DNL Commerce] -Daten in den von Erlebnis [!DNL Platform] unterstützten Anwendungen wie Echtzeit-Kundendaten [!DNL Platform], Customer Journey [!DNL Analytics] oder Journey Optimizer zu verwenden.
   * Sie müssen diesen Datensatz aus den Optionen im unten stehenden Schritt zum Datenspeicher auswählen.
   * Wählen Sie unter der linken Spalte **Datenverwaltung** im linken Navigationsbereich die Option **Datensätze**.
   * Klicken Sie oben rechts auf **Datensatz erstellen** . Wählen Sie die Option **Datensatz aus Schema erstellen** aus.
   * Suchen und verwenden Sie das Schema, das Sie im letzten Schritt erstellt haben

1. Erstellen Sie den Datenspeicher, um die [!DNL Commerce] -Daten an Adobe [!DNL Analytics] zu senden.
   * Wählen Sie unter der Überschrift **Datenerfassung** in der linken Spalte **Datastreams** aus.
   * Klicken Sie oben rechts in der Benutzeroberfläche auf **Neuer Datastream** .
   * Geben Sie einen Namen und eine optionale Beschreibung ein.
   * Suchen und wählen Sie das Schema aus, das Sie im vorherigen Schritt erstellt/identifiziert haben.
   * Fügen Sie alle gewünschten erweiterten Optionen hinzu. Weitere Informationen zu den erweiterten Optionen finden Sie in der [Dokumentation](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=de).
   * Klicken Sie auf **Speichern** , um fortzufahren.
   * Klicken Sie auf **Dienst hinzufügen** und wählen Sie **Adobe[!DNL Analytics]** im Dropdown-Feld aus.
   * Klicken Sie auf **Report Suite hinzufügen** und geben Sie die Report Suite-ID ein, die Sie in einem vorherigen Schritt erstellt/identifiziert haben. Sie können mehr als eine Report Suite hinzufügen, wenn die Daten in mehrere Report Suites fließen sollen.
   * Wenn Sie einen Datensatz in einem vorherigen Schritt erstellt haben, klicken Sie optional erneut auf **Dienst hinzufügen** und wählen Sie im Dropdown-Feld **Adobe-Erlebnis[!DNL Platform]** aus. Wählen Sie im Feld Ereignis-Datensatz den zuvor erstellten Datensatz aus.
   * Speichern Sie den Datastream.

1. Um Ihre [!DNL Commerce] -Daten anzuzeigen, müssen Sie schließlich unter Adobe [!DNL Analytics] zu Analysis Workspace navigieren, ein Projekt erstellen, Ihre Report Suite auswählen und Freiformtabellen und andere Visualisierungen hinzufügen, um Ihre [!DNL Commerce] -Daten zu melden und zu analysieren. Die folgende Abbildung zeigt ein Beispiel einer Tabelle, die Sie in Analysis Workspace erstellen können.

   ![[!DNL Analytics] Screenshot einiger Commerce-Daten](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Im Folgenden finden Sie einige zusätzliche Ressourcen, die Sie bei der Arbeit in Analysis Workspace unterstützen:

   * [Analysis Workspace – Übersicht](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Erstellen eines neuen Workspace-Projekts](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [ Tabellen, Visualisierungen und Bedienfelder in Analysis Workspace verwenden](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Anwendungsfälle für die Visualisierung](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Darüber hinaus gibt es kostenlose Kurse auf Experience League. Siehe [!DNL Analytics] verfügbare Kurse [HIER](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses).
