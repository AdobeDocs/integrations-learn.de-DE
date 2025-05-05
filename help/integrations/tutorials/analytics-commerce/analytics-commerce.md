---
title: Integration [!DNL Analytics] mit [!DNL Commerce] Tutorial
description: Erfahren Sie, wie Sie  [!DNL Analytics]  mit  [!DNL Commerce].
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

## Erstmaliges Onboarding

Diese Anweisungen gelten für Adobe [!DNL Commerce] Cloud-gehostete Projekte. Selbst gehostet kann bis zu einem gewissen Grad variieren, aber der Gesamtprozess sollte ähnlich sein.

1. Den Code in Ihrer lokalen Umgebung auschecken
1. Composer verwenden und Modul installieren
1. Befolgen Sie die einzelnen Anweisungen hier und kehren Sie nach Abschluss zurück, um die verbleibenden Schritte abzuschließen
   [Installieren und Konfigurieren des Experience  [!DNL Platform] -Connectors](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Übergeben Sie die Dateien „composer.json“ und „composer.lock“, wenn sie sich in der Cloud befinden
1. Überprüfen, ob sich das Modul in der Staging- und/oder Produktionsumgebung befindet
Sie können dies tun, indem Sie sich im Administratorbereich von Adobe [!DNL Commerce] anmelden und nach diesen neuen Bereichen unter System > Dienste suchen
   ![Experience [!DNL Platform] Connector-Erweiterung](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Konfigurieren Sie das -Modul mit Ihren -Anmeldeinformationen innerhalb des Adobe-[!DNL Commerce]-Backoffice.
   * Zuerst die [!DNL Commerce] Services-Connector-Konfigurationen, wie unten dargestellt.

     ![[!DNL Commerce] Services-Connector einrichten](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Klicken Sie dann auf die Experience [!DNL Platform]-Connector-Einstellungen, wie unten dargestellt.

     ![Experience [!DNL Platform]-Connector](./assets/analytics-commerce/experience-platform-connector.png)

Weitere Informationen zu den einzelnen Phasen und Schritten des Onboarding-Prozesses finden Sie in den Anweisungen unter [Übersicht über Experience  [!DNL Platform] Connector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. Das Tutorial zum Experience [!DNL Platform]-Connector behandelt jeden Abschnitt ausführlich und beantwortet alle Fragen, die Sie haben. Verwenden Sie dieses Tutorial für die restlichen Schritte der Schnelleinrichtung.

## Konfiguration von Experience Edge und Adobe [!DNL Analytics]

1. Stellen Sie sicher, dass Ihr Unternehmen Zugriff auf Adobe [!DNL Analytics] hat (und Sie Zugriff darauf haben). Dies können Sie bestätigen, indem Sie auf der Startseite von [Adobe Experience Cloud ](https://experience.adobe.com/) und auf den Programmumschalter (neun Punkte) in der oberen Navigationsleiste klicken.

1. Erstellen Sie eine neue Report Suite im Adobe-[!DNL Analytics] oder identifizieren Sie die ID der Report Suite, in die Sie [!DNL Commerce] Daten pushen. Weitere Informationen finden Sie in einem Tutorial [ Erstellen einer neuen Report Suite](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html). Sie benötigen diese Report Suite-ID im folgenden Schritt zum Datenstrom.

1. Navigieren Sie zur [Adobe Experience [!DNL Platform] Interface](https://platform.adobe.com), wenn Sie Zugriff auf Experience [!DNL Platform] haben. Wenn Sie keinen Zugriff auf diese Benutzeroberfläche haben, können Sie alle erforderlichen Schritte ausführen, die unten in der Benutzeroberfläche „Datenerfassung[!DNL Platform] von Adobe [ aufgeführt ](https://experience.adobe.com/#/data-collection).

1. Erstellen oder aktualisieren Sie Ihr XDM-Schema mit [!DNL Commerce] Feldergruppen. Weiterführende Informationen zum Erstellen eines Schemas finden Sie im Tutorial [Erstellen von Schemas](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=de) .
   * Sie müssen dieses Schema aus den Optionen im unten stehenden Schritt „Datenstrom“ auswählen. Um ein Schema zu erstellen, suchen Sie in der linken Spalte unter **Daten-Management** nach **Schemata**. Klicken Sie nun oben rechts in der Benutzeroberfläche auf **Schema erstellen**. XDM ExperienceEvent auswählen.
   * Nachdem Sie ein neues Schema erstellt haben, fügen Sie die [!DNL Commerce] Feldergruppen hinzu. Suchen Sie auf der linken Seite der Benutzeroberfläche nach Feldergruppen und klicken Sie auf **Hinzufügen**
      * Bei der Suche können Sie durch Eingabe von `ExperienceEvent Commerce` filtern
      * Wählen Sie die **Adobe [!DNL Analytics] ExperienceEvent-[!DNL Commerce]** aus, indem Sie das Kontrollkästchen aktivieren
      * Klicken Sie dann oben **auf &quot;** hinzufügen“, um zu speichern und fortzufahren

1. Optional (und nur, wenn Sie sich in der Experience [!DNL Platform]-Benutzeroberfläche befinden): Erstellen eines neuen Datensatzes
   * In diesem Schritt können Sie die [!DNL Commerce] Daten in Experience [!DNL Platform] importieren (getrennt von dem Einbringen der Daten in Adobe [!DNL Analytics]). Führen Sie diesen Schritt aus, wenn Sie Zugriff auf Experience [!DNL Platform] haben und die [!DNL Commerce] Daten in den von Experience [!DNL Platform] unterstützten Programmen wie Real-time Customer Data [!DNL Platform], Customer Journey [!DNL Analytics] oder Journey Optimizer verwenden möchten.
   * Sie müssen diesen Datensatz aus den Optionen im unten stehenden Schritt „Datenstrom“ auswählen.
   * Wählen Sie in der linken Spalte **Daten** Management) im linken Navigationsbereich die Option **Datensätze**.
   * Klicken **oben** auf „Datensatz erstellen“. Wählen Sie die **Datensatz aus Schema erstellen** aus.
   * Suchen und verwenden Sie das Schema, das Sie im letzten Schritt erstellt haben

1. Erstellen Sie den Datenstrom, um die [!DNL Commerce] Daten an Adobe [!DNL Analytics] zu senden
   * Wählen Sie unter **Überschrift** Datenerfassung“ in der linken Spalte **Datenströme**.
   * Klicken **oben rechts** der Benutzeroberfläche auf „Neuer Datenstrom“.
   * Geben Sie einen Namen und eine optionale Beschreibung an.
   * Suchen Sie das Schema, das Sie im vorherigen Schritt erstellt/identifiziert haben, und wählen Sie es aus.
   * Fügen Sie die gewünschten erweiterten Optionen hinzu. Weitere Informationen zu den erweiterten Optionen finden Sie in der [Dokumentation](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=de).
   * Klicken Sie auf **Speichern**, um fortzufahren.
   * Klicken Sie **Dienst hinzufügen** und wählen Sie **Adobe-[!DNL Analytics]** in der Dropdown-Liste.
   * Klicken Sie **Report Suite hinzufügen** und geben Sie die Report Suite-ID ein, die Sie in einem vorherigen Schritt erstellt/identifiziert haben. Sie können mehr als eine Report Suite hinzufügen, wenn die Daten in mehrere Report Suites fließen sollen.
   * Wenn Sie in einem vorherigen Schritt einen Datensatz erstellt haben, klicken Sie optional erneut auf **Service hinzufügen** und wählen Sie aus der Dropdown-Liste **Adobe Experience[!DNL Platform]** aus. Wählen Sie im Feld Ereignis-Datensatz den zuvor erstellten Datensatz aus.
   * Speichern Sie den Datenstrom.

1. Um Ihre [!DNL Commerce] anzuzeigen, müssen Sie in Adobe [!DNL Analytics] zu Analysis Workspace navigieren, ein Projekt erstellen, Ihre Report Suite auswählen und Freiformtabellen und andere Visualisierungen hinzufügen, um Berichte zu Ihren [!DNL Commerce]-Daten zu erstellen und zu analysieren. Die folgende Abbildung zeigt ein Beispiel für eine Tabelle, die Sie in Analysis Workspace erstellen können.

   ![[!DNL Analytics] Screenshot einiger Commerce-Daten](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Im Folgenden finden Sie einige zusätzliche Ressourcen, die Ihnen bei der Arbeit in Analysis Workspace helfen:

   * [Analysis Workspace – Übersicht](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Erstellen eines neuen Workspace-Projekts](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Verwenden von Tabellen, Visualisierungen und Bedienfeldern in Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Anwendungsfälle für Visualisierungen](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Darüber hinaus gibt es kostenlose Kurse auf Experience League. Siehe [!DNL Analytics] verfügbaren Kurse [HIER](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses).
