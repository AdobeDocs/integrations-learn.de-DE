---
title: Anwendungsintegrationen für skalierbare Personalisierung
description: Gestalten Sie personalisierte Erlebnisse zu einem Teil jedes Augenblicks.
exl-id: 6d18813d-950c-40ae-8d5b-80bf389358fc
source-git-commit: 509b227f360718e81fb19d3a4d30aebf9de49e5a
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Personalization im großen Maßstab

In der heutigen, stark vom Wettbewerb geprägten und digital geprägten Landschaft erwarten Kunden immer mehr Erlebnisse, die auf ihre individuellen Präferenzen und Bedürfnisse zugeschnitten sind. Durch die Nutzung der Funktionen von Adobe Experience Cloud können wir umfangreiche Kundendaten erfassen und analysieren und so wertvolle Einblicke in Verhaltensweisen, Interessen und Vorlieben gewinnen. Dieses tiefe Verständnis erleichtert die Bereitstellung personalisierter Erlebnisse über verschiedene Touchpoints hinweg und stellt so aussagekräftige und ansprechende Interaktionen sicher. Durch die Nutzung der Leistungsfähigkeit von Adobe Experience Cloud wird das volle Potenzial der Personalisierung ausgeschöpft, was stärkere Kundenverbindungen fördert, die Kundentreue stärkt und das Geschäftswachstum steigert.

<table>
 <thead>
    <tr>
      <th>Anwendungsfall</th>
      <th>Beschreibung</th>
      <th>Beispiele</th>
      <th>Anwendungen</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Erstellen personalisierter PDF-Dokumente</strong></td>
      <td>
        Generieren von Kommunikationsdokumenten für das Signieren basierend auf dem Benutzer
        Auswahlen/Voreinstellungen.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Dynamisch generierte NDA basierend auf den Daten einer AEM präsentieren
            Forms-Übermittlung zum Signieren
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-acrobat-sign.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Forms und Sign</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Datenanalyse und Reporting</strong></td>
      <td>
        Analysieren von Verhaltensdaten aus digitalen Erlebnissen <br />Adobe verwenden
        [!DNL Analytics] von Verhaltensdaten in Analysis Workspace auf Kunden-Journey
        [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Konvertierungspfade oben/unten analysieren</li>
          <li>Kanalinteraktion und -konvertierung analysieren</li>
          <li>Grundlegendes zu am häufigsten angezeigten Inhalten</li>
          <li>Die wichtigsten Produktkategorien und Produkte</li>
          <li>
            Durchführen einer Tool-Nutzungsanalyse zur Optimierung von Self-Service-Erlebnissen
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] und Kunden-Journey [!DNL Analytics]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Reporting für Personalisierungsaktivitäten<br />Optimierung analysieren
        Testergebnisse, einschließlich A/B-Tests, unter Verwendung von Adobe-[!DNL Target] und
        Erstellung umfassender Berichte durch Adobe [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Anzeigen von A/B-Testergebnissen in umfangreichen Analyseberichten</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] und [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>E-Mail-Sendungen personalisieren</strong></td>
      <td>
        Personalisieren von E-Mail-Sendungen mit dynamischen Inhalten mithilfe der
        Funktionen von Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Hinzufügen personalisierter Angebote zu Kunden-E-Mails</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/campaign//campaign-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Campaign] und [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2">
        <strong>Erweiterung der Zielgruppen für Personalisierungs- und Anzeigenplattformen</strong>
      </td>
      <td>
        Verwenden von Audience Manager-Segmenten zum Erstellen von Zielgruppen in Real-Time CDP, um
        wird in Personalisierungs- und Remarketing-Taktiken verwendet.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Anonymes Targeting digitaler Zielgruppen und Personalisierung für
            Die Website, die Mobile App oder auf unterstützten Werbekanälen
          </li>
          <li>
            Optimieren Sie die Erlebnisse auf der Landingpage und vor der Authentifizierung auf der Grundlage von
            Bekannte Geräte- und Verhaltenseigenschaften
          </li>
          <li>
            Nutzen des Audience Manager-Datennetzwerks von Drittanbietern, um
            Zielgruppen für das Targeting verfeinern und erweitern
          </li>
          <li>Freigeben von Audience Manager-Segmenten für RTCDP</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/aam/aam-rtcdp.md"
          target="_blank"
          rel="noopener noreferrer"
          >Audience Manager- und Echtzeit-[!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Verwenden Sie [!DNL Analytics] Daten zum Erstellen von Zielgruppen, die in der Personalisierung oder
        Remarketing-Taktiken.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Zielgruppen-Targeting und Personalisierung für digitale Medien auf Geräten oder
            Unterstützte Werbekanäle.
          </li>
          <li>
            Bekannte Landingpages und anonyme Erlebnisse von Kunden optimieren
            basierend auf Geräte- und Verhaltensattributen.
          </li>
          <li>Zielgruppen für bekannte Kanäle wie E-Mail und SMS aktivieren.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] und Real-time Customer Data [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Web-Erlebnisse personalisieren</strong></td>
      <td>
        Anpassen von Single Page Application (SPA)-Erlebnissen durch effektive
        Verwendung von AEM Headless in Verbindung mit Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalisierung von SPA und Mobile Apps</li>
          <li>Personalisierte API-Antworten.</li>
          <li>[!DNL Target]Inhaltsbereitstellung bearbeiten.</li>
          <li>A/B-Testvarianzen.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Headless und [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Bereitstellen maßgeschneiderter Website-Erlebnisse durch effektive Nutzung von AEM Sites
        und Adobe-[!DNL Target] zur Personalisierung.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>AEM-Website-Personalisierung.</li>
          <li>Personalisieren von Website-Inhalten</li>
          <li>Optimieren Sie Benutzererlebnisse.</li>
          <li>A/B-Testvarianzen.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Sites und [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Digitale Erlebnisse personalisieren</strong></td>
      <td>
        Verwenden von Echtzeit-Kundenprofilen und zentral verwalteten [!DNL Platform]
        So personalisieren Sie Nachrichten über Web-, Mobile- und andere digitale Kanäle
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalisierung von Inhalten für bekannte Besucher</li>
          <li>Erhöhen der Treue, Anmeldung und Teilnahme</li>
          <li>Identifizieren und Interagieren von Kunden mit Abwanderungsrisiko</li>
          <li>Personalisierung von Angeboten in Echtzeit</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Real-time Customer Data [!DNL Platform] und [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Verbessern der Lead-Generierung</strong></td>
      <td>
        Verwenden von Echtzeit-Kundenprofilen und zentral verwalteten [!DNL Platform]
        So personalisieren Sie Nachrichten über Web-, Mobile- und andere digitale Kanäle
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalisierung von Inhalten für bekannte Besucher</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Real-time Customer Data [!DNL Platform] und [!DNL Target]</a
        >
      </td>
    </tr>
  </tbody>
</table>
