---
title: Einrichten von Adobe GenStudio mithilfe von AEM Assets und GenStudio for Performance Marketing
description: Erfahren Sie, wie Sie die Integration zwischen AEM Assets und GenStudio for Performance Marketing einrichten.
solution: Experience Manager, GenStudio for Performance Marketing
version: Cloud Service
feature-set: Experience Manager Assets, GenStudio for Performance Marketing
topic: Content Supply Chain
role: User
level: Intermediate
doc-type: Feature Video
duration: 416
last-substantial-update: 2024-11-19T00:00:00Z
jira: KT-16484
source-git-commit: 7d07f37f6267eda106f895cb367d42669f0d5c65
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Einrichten

[Zurück zur Integration - Übersicht](./overview.md)

Um mit dem Adobe GenStudio mit AEM Assets as a Cloud Service und GenStudio for Performance Marketing zu beginnen, müssen beide Anwendungen ordnungsgemäß konfiguriert sein. Der Einrichtungsprozess umfasst mehrere Schritte, die abgeschlossen werden müssen, bevor Sie Adobe GenStudio vollständig in AEM Assets und GenStudio for Performance Marketing integrieren können.

Diese Aufgaben erfordern die Zusammenarbeit mit Administratoren, die über die entsprechenden Berechtigungen zum Verwalten beider Systeme verfügen.

<!-- CARDS 

* https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view
   {title=Set up AEM Assets with Assets view}
* https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up
   {title=Enable AEM Assets Content Hub}
* https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started
   {title=Set up GenStudio for Performance Marketing}
   {image=https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/media_1dd8829962c9e37e1251f3d2d92f5d72c8a58cdaf.png?width=2000&format=webply&optimize=medium}

-->
<!-- START CARDS HTML - DO NOT MODIFY BY HAND -->
<div class="columns">
    <div class="column is-half-tablet is-half-desktop is-one-third-widescreen" aria-label="Set up AEM Assets with Assets view">
        <div class="card" style="height: 100%; display: flex; flex-direction: column; height: 100%;">
            <div class="card-image">
                <figure class="image x-is-16by9">
                    <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view" title="Einrichten von AEM Assets mit Assets-Ansicht" target="_blank" rel="referrer">
                        <img class="is-bordered-r-small" src="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view./media_1e4b209baa6169af9b0aefff8a2f1f39816aa6b42.png?width=400&format=png&optimize=medium" alt="Einrichten von AEM Assets mit Assets-Ansicht"
                             style="width: 100%; aspect-ratio: 16 / 9; object-fit: cover; overflow: hidden; display: block; margin: auto;">
                    </a>
                </figure>
            </div>
            <div class="card-content is-padded-small" style="display: flex; flex-direction: column; flex-grow: 1; justify-content: space-between;">
                <div class="top-card-content">
                    <p class="headline is-size-6 has-text-weight-bold">
                        <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view" target="_blank" rel="referrer" title="Einrichten von AEM Assets mit Assets-Ansicht">Einrichten von AEM Assets mit Assets-Ansicht</a>
                    </p>
                    <p class="is-size-6">Erfahren Sie, wie Sie AEM Assets as a Cloud Service in der Assets-Ansicht mit dieser Sammlung von Video-Wiedergabelisten verwenden können, um Ihr Produktwissen zu verbessern.</p>
                </div>
                <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view" target="_blank" rel="referrer" class="spectrum-Button spectrum-Button--outline spectrum-Button--primary spectrum-Button--sizeM" style="align-self: flex-start; margin-top: 1rem;">
                    <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">Mehr erfahren</span>
                </a>
            </div>
        </div>
    </div>
    <div class="column is-half-tablet is-half-desktop is-one-third-widescreen" aria-label="Enable AEM Assets Content Hub">
        <div class="card" style="height: 100%; display: flex; flex-direction: column; height: 100%;">
            <div class="card-image">
                <figure class="image x-is-16by9">
                    <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up" title="Aktivieren von AEM Assets Content Hub" target="_blank" rel="referrer">
                        <img class="is-bordered-r-small" src="https://video.tv.adobe.com/v/3433513/?format=jpeg&nocache=1732038662663" alt="Aktivieren von AEM Assets Content Hub"
                             style="width: 100%; aspect-ratio: 16 / 9; object-fit: cover; overflow: hidden; display: block; margin: auto;">
                    </a>
                </figure>
            </div>
            <div class="card-content is-padded-small" style="display: flex; flex-direction: column; flex-grow: 1; justify-content: space-between;">
                <div class="top-card-content">
                    <p class="headline is-size-6 has-text-weight-bold">
                        <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up" target="_blank" rel="referrer" title="Aktivieren von AEM Assets Content Hub">AEM Assets Content Hub aktivieren</a>
                    </p>
                    <p class="is-size-6">Erfahren Sie, wie Sie Adobe Experience Manager Assets Content Hub in AEM as a Cloud Service einrichten.</p>
                </div>
                <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up" target="_blank" rel="referrer" class="spectrum-Button spectrum-Button--outline spectrum-Button--primary spectrum-Button--sizeM" style="align-self: flex-start; margin-top: 1rem;">
                    <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">Watch</span>
                </a>
            </div>
        </div>
    </div>
    <div class="column is-half-tablet is-half-desktop is-one-third-widescreen" aria-label="Set up GenStudio for Performance Marketing">
        <div class="card" style="height: 100%; display: flex; flex-direction: column; height: 100%;">
            <div class="card-image">
                <figure class="image x-is-16by9">
                    <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started" title="Einrichten von GenStudio for Performance Marketing" target="_blank" rel="referrer">
                        <img class="is-bordered-r-small" src="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/media_1dd8829962c9e37e1251f3d2d92f5d72c8a58cdaf.png?width=400&format=webply&optimize=medium" alt="Einrichten von GenStudio for Performance Marketing"
                             style="width: 100%; aspect-ratio: 16 / 9; object-fit: cover; overflow: hidden; display: block; margin: auto;">
                    </a>
                </figure>
            </div>
            <div class="card-content is-padded-small" style="display: flex; flex-direction: column; flex-grow: 1; justify-content: space-between;">
                <div class="top-card-content">
                    <p class="headline is-size-6 has-text-weight-bold">
                        <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started" target="_blank" rel="referrer" title="Einrichten von GenStudio for Performance Marketing">Einrichten von GenStudio for Performance Marketing</a>
                    </p>
                    <p class="is-size-6">Erfahren Sie, wie Sie mit GenStudio for Performance Marketing beginnen, um neue markenorientierte Marketinginhalte zu generieren.</p>
                </div>
                <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started" target="_blank" rel="referrer" class="spectrum-Button spectrum-Button--outline spectrum-Button--primary spectrum-Button--sizeM" style="align-self: flex-start; margin-top: 1rem;">
                    <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">Mehr erfahren</span>
                </a>
            </div>
        </div>
    </div>
</div>
<!-- END CARDS HTML - DO NOT MODIFY BY HAND -->

