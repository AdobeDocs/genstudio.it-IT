---
title: Connettersi a un archivio AEM Assets Content Hub
description: Scopri come collegare GenStudio for Performance Marketers a un archivio Content Hub Adobe Experience Manager (AEM) e sfruttare i contenuti approvati esistenti.
level: Experienced
feature: Assets, Content
source-git-commit: dc438085cfe7c93b20dc7fb0d5919d2dc8b3dcde
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Connetti a un archivio [!DNL AEM Assets Content Hub]

Se disponi di risorse in Adobe Experience Manager (AEM), puoi seguire questi passaggi per renderle accessibili in GenStudio per gli addetti al marketing delle prestazioni.

>[!BEGINSHADEBOX]

**Prerequisiti**:

I passaggi seguenti richiedono l’accesso amministrativo a Admin Console e AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Passaggio 1: abilitare [!DNL AEM Assets Content Hub]

Segui il processo self-service **Distribuisci Content Hub** per abilitare [!DNL Content Hub] per il tuo AEM Assets esistente in Cloud Manager. Consulta [Distribuisci [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) nella documentazione di _AEM as a Cloud Service_.

Dopo aver abilitato [!DNL AEM Assets Content Hub], si dispone di una nuova istanza con il suffisso `contenthub` all&#39;interno di [!DNL AEM Assets as a Cloud Service] in Admin Console.

## Passaggio 2: integrare gli utenti di GenStudio

In [!DNL Admin Console], aggiungere utenti o gruppi di utenti GenStudio ai profili di prodotto [!DNL AEM Assets Content Hub]. [!DNL AEM Assets Content Hub] utenti possono visualizzare le risorse, ma non possono aggiungere o modificare le risorse esistenti.

- [Integrato [!DNL Content Hub] amministratore](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Onboarding [!DNL Content Hub] utenti](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Passaggio 3: approvare le risorse

Approva le risorse da utilizzare in [!DNL AEM Assets Content Hub], che le rende disponibili in GenStudio per gli esperti di marketing delle prestazioni. Consulta [Approvare le risorse in Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) nella _documentazione di AEM as a Cloud Service_.

## Passaggio 4: configurare la visibilità delle risorse

Nelle opzioni di configurazione _[!DNL AEM Assets Content Hub]_, controlla ogni set di opzioni di configurazione per filtri, dettagli risorsa, ricerca e branding. Consulta [Configurare l&#39;interfaccia utente di Content Hub](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) nella_ documentazione di AEM as a Cloud Service _.

## Passaggio 5: verificare la connessione

In GenStudio for Performance Marketers Content, l&#39;elenco _[!UICONTROL Posizione]_ è disponibile sopra la raccolta sul lato destro. L&#39;elenco non è disponibile se non si dispone dell&#39;accesso o se l&#39;organizzazione non ha distribuito e connesso un archivio [!DNL AEM Assets Content Hub].