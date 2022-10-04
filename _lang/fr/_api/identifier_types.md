---
nav_title: "Types d’identifiant API"
article_title: Types d’identifiant API
page_order: 2.2
description: "Cet article de référence couvre les différents types d’identifiants API qui existent dans le tableau de bord de Braze, où vous pouvez les trouver et ce à qu’ils servent." 
page_type: reference

---

# Types d’identifiant API

> Ce guide de référence aborde les différents types d’identifiants API que vous trouverez dans le tableau de bord de Braze, leur but, où vous pouvez les trouver et comment ils sont généralement utilisés. Pour plus d’informations sur les clés API REST ou les clés API du groupe d’apps, reportez-vous à la [présentation de la clé API Rest]({{site.baseurl}}/api/api_key/)

Les identifiants API suivants peuvent être utilisés pour accéder à votre modèle, Canvas, campagne, segment, envoi ou carte de l’API externe de Braze. Tous les messages doivent suivre le codage [UTF-8][1].

{% tabs %}
{% tab Template Ids %}

## Identifiant API modèle

Un identifiant API [modèle]({{site.baseurl}}/api/endpoints/templates/) ou ID modèle est une clé prête à l’emploi proposée par Braze pour un modèle donné dans le tableau de bord. Les ID de modèle sont uniques pour chaque modèle et peuvent être utilisés pour référencer les modèles via l’API. 

Les modèles sont parfaits si votre entreprise établit des contrats sur vos conceptions HTML pour les campagnes. Une fois les modèles construits, vous disposez d’un modèle qui n’est pas spécifique à une campagne, mais qui peut être appliqué à une série de campagnes comme un bulletin d’information.

### Où puis-je le trouver ?
Vous pouvez trouver votre ID de modèle de deux manières :

1. Dans le tableau de bord, ouvrez **Templates & Media (Modèles et médias)** dans **Engagement** et sélectionnez un modèle préexistant. Si le modèle que vous voulez n’existe pas encore, créez-en un et enregistrez-le. Au bas de la page de modèle individuel, vous trouverez votre identifiant API modèle.<br><br>
2. Braze propose une recherche des **identifiants API supplémentaires**. Vous pouvez rapidement y rechercher des identifiants spécifiques. Elle se trouve au bas de l’onglet **API Settings (Paramètres API)** sur la page **Developer Console (Console du développeur)**.

### À quoi cela sert-il ?

- Mettre à jour les modèles sur API
- Saisir des informations sur un modèle spécifique

<br>
{% endtab %}
{% tab Canvas IDs %}

## Identifiant API Canvas

Un identifiant API [Canvas]({{site.baseurl}}/user_guide/engagement_tools/canvas/) ou ID Canvas est une clé prête à l’emploi proposée par Braze pour un Canvas donné dans le tableau de bord. Les ID Canvas sont uniques pour chaque Canvas et peuvent être utilisés pour référencer des Canvas via l’API. 

Notez que si vous disposez d’un Canvas qui comporte des variantes, il existe un ID Canvas global ainsi que des ID Canvas aux variantes individuelles imbriqués dans le Canvas principal. 

### Où puis-je le trouver ?
Vous pouvez trouver votre ID Canvas dans le tableau de bord. Ouvrez **Canvas** dans **Engagement** et sélectionnez un Canvas préexistant. Si le Canvas que vous voulez n’existe pas encore, créez-en une et enregistrez-le. Au bas d’une page Canvas distincte, cliquez sur **Analyze Variants (Analyser les variantes)**. Une fenêtre apparaît avec l’identifiant de l’API Canvas situé en bas.

### À quoi cela sert-il ?
- Suivre l’analyse d’un message spécifique
- Obtenir des statistiques globales de haut niveau sur les performances du Canvas
- Obtenir des informations sur un Canvas spécifique
- Avec Currents pour apporter des données au niveau utilisateur pour une approche « d’image plus large » des Canvas
- Avec la livraison déclenchée par API afin de collecter des statistiques pour les messages transactionnels

<br>
{% endtab %}
{% tab Campaign IDs %}

## Identifiant API de campagne

Un identifiant API de [campagne]({{site.baseurl}}/user_guide/engagement_tools/campaigns/) ou ID campagne est une clé prête à l’emploi proposée par Braze pour une campagne donnée dans le tableau de bord. Les ID de campagne sont uniques pour chaque campagne et peuvent être utilisés pour référencer des campagnes via l’API. 

Notez que si vous disposez d’une campagne qui comporte des variantes, il existe un ID de campagne global ainsi que des ID de campagne aux variantes distinctes imbriqués dans la campagne principale. 

### Où puis-je le trouver ?
Vous pouvez trouver votre ID de campagne de deux manières :

1. Dans le tableau de bord, ouvrez **Campagnes** dans **Engagement** et sélectionnez une campagne préexistante. Si la campagne que vous souhaitez n’existe pas encore, créez-en une et enregistrez-la. Au bas de la page de campagne individuelle, vous trouverez votre **identifiant API de campagne**.<br><br>
2. Braze propose une recherche des **identifiants API supplémentaires**. Vous pouvez rapidement y rechercher des identifiants spécifiques. Vous pouvez la trouver au bas de l’onglet **API Settings (Paramètres API)** dans **Developer Console (Console du développeur)**.

### À quoi cela sert-il ?
- Suivre l’analyse d’un message spécifique
- Obtenir des statistiques globales de haut niveau sur les performances de la campagne
- Obtenir des informations sur une campagne spécifique
- Avec Currents pour apporter des données au niveau utilisateur pour une approche « d’image plus large » des campagnes
- Avec la livraison déclenchée par API afin de collecter des statistiques pour les messages transactionnels

<br>
{% endtab %}
{% tab Segment IDs %}

## Identifiant API de segment

Un identifiant API de [segment]({{site.baseurl}}/user_guide/engagement_tools/segments/) ou ID de segment est une clé prête à l’emploi proposée par Braze pour un segment donné dans le tableau de bord. Les ID de segment sont uniques pour chaque segment et peuvent être utilisés pour référencer les segments via l’API. 

### Où puis-je le trouver ?
Vous pouvez trouver votre ID de segment de deux manières :

1. Dans le tableau de bord, ouvrez **Segments** dans **Engagement** et sélectionnez un segment préexistant. Si le segment que vous voulez n’existe pas encore, créez-en un et enregistrez-le. Au bas de la page du segment individuel, vous trouverez votre identifiant API de segment. <br><br>
2. Braze propose une recherche des **identifiants API supplémentaires**. Vous pouvez rapidement y rechercher des identifiants spécifiques. Elle se trouve au bas de l’onglet **API Settings (Paramètres API)** sur la page **Developer Console (Console du développeur)**.

### À quoi cela sert-il ?
- Obtenir des informations sur un segment spécifique
- Récupérer l’analyse d’un segment spécifique
- Récupérer le nombre de fois où un événement personnalisé a été enregistré pour un segment particulier
- Spécifier et envoyer une campagne à un membre d’un segment depuis l’API

{% endtab %}
{% tab Card IDs %}

## Identifiant API de carte

Un identifiant API de carte ou ID de carte est une clé prête à l’emploi proposée par Braze pour une carte de fil d’actualité donnée dans le tableau de bord. Les ID de carte sont uniques pour chaque carte de [fil d’actualité]({{site.baseurl}}/user_guide/engagement_tools/news_feed/) et peuvent être utilisés pour référencer les cartes via l’API. 

### Où puis-je le trouver ?
Vous pouvez trouver votre ID de carte de deux manières :

1. Dans le tableau de bord, ouvrez **Fil d’actualité** dans **Engagement** et sélectionnez un fil d’actualité préexistant. Si le fil d’actualité que vous voulez n’existe pas encore, créez-en un et enregistrez-le. Au bas de la page du fil d’actualité individuel, vous trouverez votre identifiant API unique de carte. <br><br>
2. Braze propose une recherche des **identifiants API supplémentaires**. Vous pouvez rapidement y rechercher des identifiants spécifiques. Elle se trouve au bas de l’onglet **API Settings (Paramètres API)** sur la page **Developer Console (Console du développeur)**.

### À quoi cela sert-il ?
- Récupérer les informations pertinentes sur une carte
- Suivre les événements liés aux cartes de contenu et à l’engagement

<br>
{% endtab %}
{% tab Send IDs %}

## Identifiant d’envoi

Un identifiant d’envoi ou un ID d’envoi est une clé générée par Braze ou créée par vous pour un message donné et envoyé dans le cadre duquel l’analyse doit être suivie. L’identifiant d’envoi vous permet de récupérer des analyses pour une instance spécifique d’une campagne envoyée via l’endpoint [`sends/data_series`]({{site.baseurl}}/api/endpoints/export/campaigns/get_send_analytics/).

### Où puis-je le trouver ?

Les API et campagnes déclenchées par API qui sont envoyées en tant que diffusion génèrent automatiquement un identifiant d’envoi si un identifiant d’envoi n’est pas fourni. Si vous souhaitez spécifier votre propre identifiant d’envoi, vous devrez d’abord en créer un via l’endpoint [`sends/id/create`]({{site.baseurl}}/api/endpoints/messaging/send_messages/post_create_send_ids/). L’identifiant doit comporter tous les caractères ASCII et au maximum 64 caractères. Vous pouvez réutiliser un identifiant d’envoi sur plusieurs envois de la même campagne si vous souhaitez regrouper les analyses de ces envois.

### À quoi cela sert-il ?
Envoyer et suivre par programme les performances des messages, sans création de campagne pour chaque envoi.

<br>
{% endtab %}
{% endtabs %}

[1]: https://en.wikipedia.org/wiki/UTF-8