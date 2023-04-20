# Embeddable AI Workshop - Aan de slag met Watson NLP


Hallo en welkom bij de Praktische Hands-on Workshop voor Embeddable AI in de Nederlandse taal! In deze workshop nemen we je mee op een leerzame en interactieve ontdekkingsreis, waar je leert hoe je onze veelzijdige en krachtige Embeddable AI NLP bibliotheek kunt benutten om jouw projecten en applicaties te voorzien van IBM's krachtige taalverwerkingstechnologie en daarmee naar een hoger niveau te tillen. 

Deze **README** bevat belangrijke informatie en instructies om je te helpen het meeste uit deze workshop te halen. Lees het zorgvuldig door voordat je begint.

</br></br>

## Inhoudsopgave
1. **[Introductie](#introductie)**

2. **[Vereisten](#vereisten)** 

3. **[Benodigdheden](#Benodigdheden)**


4. **[Installatie-instructies](#installatie):**


5. **[Documentatie en bronnen](#docs):**


</br></br>

<a id='introductie'>

## 1. Introductie 

Het doel van de workshop is om IBM Business Partners kennis te laten maken met IBM's [Embeddable AI NLP library](https://www.ibm.com/products/ibm-watson-natural-language-processing). Met Watson Natural Language Processing kunt u ongestructureerde gegevens omzetten in gestructureerde gegevens, waardoor de gegevens eenvoudiger te begrijpen en overdraagbaar worden.  Dit is met name handig als u werkt met een combinatie van ongestructureerde en gestructureerde gegevens. Voorbeelden van dergelijke gegevens zijn gegevens van callcenters, klachten van klanten, berichten op sociale media of probleemrapporten. De ongestructureerde gegevens maken vaak deel uit van een groter gegevensrecord dat kolommen met gestructureerde gegevens bevat. Door betekenis en structuur te halen uit de ongestructureerde gegevens en deze informatie te combineren met de gegevens in de kolommen met gestructureerde gegevens, verkrijgt u een dieper inzicht in de ingevoerde gegevens. Hierdoor kunt u betere beslissingen nemen op basis van de beschikbare informatie. 

Ook is het mogelijk om hele doelgerichte applicaties te ontwikkelen die de mens helpen bij het uitvoeren van foutgevoelige, repetitieve taken. Eén voorbeeld hiervan is het herkennen van persoonsgevoelige informatie in (overheids)documenten. Watson NLP is in staat om met zowel voorgetrainde modellen, al dan niet aangevuld met zelfgetrainde modellen om met hoge accuraatheid persoonsgevoelige informatie te herkennen in tekstdocumenten. Met de IBM Watson Embeddable AI NLP bibliotheek ontwikkelt u snel applicaties die helpen bij Algemene Verordening Gegevensbescherming (AVG) vraagstukken. 

De Watson Natural Language Processing-bibliotheek biedt niet alleen basisfuncties voor natuurlijke taalverwerking, zoals syntaxisanalyse, maar ook een breed scala aan kant-en-klare vooraf getrainde modellen die direct gereed zijn voor gebruik! Denk hierbij aan sentimentanalyse, het extraheren van trefwoorden en vectorisatie. Werken de voorgetrainde modellen onvoldoende op jouw specifieke domein, dan is er ook de mogelijkheid om een selectie van deze modellen te fine-tunen of volledig met eigen data te trainen. De Watson Natural Language Processing-bibliotheek is beschikbaar voor Python. 

Watson Natural Language Processing biedt vooraf getrainde modellen in meer dan 20 talen. Deze modellen worden samengesteld door een toegewijd team van experts en geëvalueerd op kwaliteit voor elke specifieke taal. Deze vooraf getrainde modellen kunnen in productieomgevingen worden gebruikt zonder dat u zich zorgen hoeft te maken over schendingen van licenties of intellectueel eigendom.

Hoewel u uw eigen modellen kunt creëren, is de eenvoudigste manier om met Watson Natural Language Processing te beginnen het uitvoeren van de vooraf getrainde modellen op ongestructureerde tekst om taalverwerkingstaken uit te voeren.

</br></br>

### In deze praktische workshop werken we twee voorbeelden uit:

1. **PII extractie**: extractie van persoonsgevoelige data uit Nederlandstalige documenten gebruikmakend van **voorgetrained modellen**
2. **Fine-tuning van het voorgetrainde Sentiment Analyse model**: Het **fine-tunen** van het voorgetrainde BERT sentiment analyse model om Nederlandstalige boekenreviews van [Hebban.nl](https://www.hebban.nl) op sentiment te beoordelen

</br></br>


## 2. Vereisten

<a id='vereisten'>

Enige kennis en ervaring met Python is sterk aanbevolen. Om deel te nemen aan deze workshop, dien je te beschikken over:

1. Basisprogrammeerkennis in Python
2. Een computer met een moderne webbrowser en internettoegang
3. Een [IBM Cloud account](https://cloud.ibm.com/registration)
4. Cloud Object Storage instance (COS)
5. Watson Studio service (CPDaaS)


</br></br>

## 3. Benodigdheden

<a id='benodigdheden'>

De benodigde Jupyter Notebooks en data kun je downloaden vanuit de volgende publiek beschikbare Git repository.
[Nederlandstalige Watson Hands-On workshop](https://github.com/joost-vos/watson-nlp-handson)
De Notebooks kun je direct vanuit de IBM Cloud in je Watson Studio omgeving downloaden _zie [Installatie](#installatie)_. 

De workshop bestaat uit twee programma-onderdelen:
* Extractie van persoonsgevoelige informatie (PII) gebruikmakend van voorgetrainde modellen [PII Notebook](https://github.com/joost-vos/watson-nlp-handson/blob/main/PII%20Extraction%20-%20Pre-Trained%20Models.ipynb)
* Fine-tuning van het voorgetrainde Sentiment Analyse model [Sentiment Analyse Notebook](https://github.com/joost-vos/watson-nlp-handson/blob/main/Boekenreviews%20-%20Sentiment%20Analyse.ipynb)

</br></br>




## 4. Installatie-instructies  
<a id='installatie'>
  
### 4.1 Opzetten van je omgeving    

Om met IBM Watson NLP aan de slag te gaan dien je een Python-notebookomgeving in die Watson Studio op IBM Cloud in te stellen. Vanuit een Jupyter notebook kun je de watson_nlp-bibliotheek gaan gebruiken. Er zijn twee manieren om je omgeving in te stellen:
1. **Met TechZone** - Voor IBM Business Partners die toegang hebben tot IBM Tech Zone, is het mogelijk om daar een demo-omgeving te reserveren.
2. **Zonder IBM TechZone** - Zonder TechZone is het mogelijk om met de Lite versie van Watson Studio het notebook rechtstreeks in uw Watson Studio-project laden. Binnen de Lite-versie verkrijg je 10 CUH (Compute Unit Hours) kostenloos; wat toereikend is om de workshop af te ronden. 


<div style="border: 2px solid red; padding: 10px; background-color: #ffe6e6; border-radius: 5px; margin-bottom: 10px;">
  ⚠️ In deze workshop gebruiken we <b>optie 2</b>.
</div>

#### 4.1.1 IBM Cloud

1. Log in met je IBM Cloud ID, of creëer een IBM Cloud ID

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/001.jpg)

</br></br>


#### 4.1.2 IBM Cloud Object Storage


<div style="border: 2px solid red; padding: 10px; background-color: #ffe6e6; border-radius: 5px; margin-bottom: 10px;">
  ⚠️ <b>Sla deze stap over als je al beschikt over een Cloud Object Storage instance</b>.
</div>

1. Klik op **Catalog**

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/002.jpg) 

</br></br>


2. Klik op **Object Storage**

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/002_COS.jpg)

</br></br>


3. Klik op **Object Storage**
	* Kies **IBM Cloud** als locatie
	* Kies **Lite** als pricing plan
	* Klik **Create**

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/003_COS.jpg)

</br></br>


#### 4.1.3 IBM Watson Studio


2. Klik op **Catalog**

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/002.jpg) 

</br></br>


3. Zoek naar **Watson Studio**

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/003.jpg)

</br></br>


4. Vraag de **Watson Studio Lite** service aan
	* Kies **Frankfurt(eu-de)** als locatie
	* Kies **Lite** als pricing plan
	* Lees en accepteer **de licentieovereenkomst**
	* Klik **Create**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/004.jpg)

</br></br>


5. Start **Watson Studio Lite** in IBM CLoud Pak for Data as a Service
	* Klik op **Launch in IBM CLoud Pak for Data**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/005.jpg)

</br></br>


6. Maak een **nieuw project** aan
	* Klik op **New Project**
	* Klik op **Next**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/006.jpg)

</br></br>


7. Definieer je **New Project**
	* Geef je project een **Naam**
	* Selecteer je **Cloud Object Store Storage Service**
	* Klik op **Create**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/007.jpg)

</br></br>


8. Voeg de praktijkles **assets** toe
	* Klik op **New asset**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/008.jpg)

</br></br>

9. Zoek in de zoekbalk naar **Jupyter**
	* Klik op **Jupyter Notebook Editor**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/009.jpg)

</br></br>


10. Voeg de **Notebook assets** uit de Watson-hands-on git repository toe
	* Klik op **From URL**
	* Geef het Notebook een **Naam**
	* Selecteer de **runtime: DO + NLP Runtime22.2 on Python 3.10 XS(2vCPU 8GB RAM)**
	* Plak de link naar het Notebook in de Github repo
	* Klik op **Create**
	

![image](https://s3.eu-de.cloud-object-storage.appdomain.cloud/embeddableainl/010.jpg)

</br></br>


<div style="border: 2px solid green; padding: 10px; background-color: #73fa79; border-radius: 5px; margin-bottom: 10px;">
  👍 <b>Je omgeving is gereed om met de hands-on aan de slag te gaan!</b>.
</div>



bron: [IBM Developer - Setting up your IBM Watson Library Environment](https://developer.ibm.com/tutorials/set-up-your-ibm-watson-libraries-environment/)

</br></br>



## 5. Documentatie en bronnen

<a id='docs'>

[IBM Embeddable AI landing page](https://www.ibm.com/products/ibm-watson-natural-language-processing).  

[IBM Developer on Embeddable AI – Tutorials and TechZone links](https://github.com/ibm-build-lab/Watson-NLP). 

[Watson NLP Library documentation for Cloud Pak for Data as a service (IBM Cloud)](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/watson-nlp.html?context=cpdaas). 

[Watson NLP Build Labs – Tutorials](https://github.com/ibm-build-lab/Watson-NLP). 

[IBM Embeddable AI Community](https://community.ibm.com/community/user/communities/community-home?CommunityKey=6036cf42-199f-4f03-9d5c-ba4aa4983e49). 


[IBM's Digital Self-Serve Co-Create Experience(DCSE)](https://dsce.ibm.com/)

[IBM TechZone Embeddable AI](https://techzone.ibm.com/collection/embedded-ai)

</br></br>

### 5.1 Demo Applicaties

</br>

[SentimentandEmotionsApp](https://ibm.biz/BdPqJ2). 
 
[TopicApp](https://ibm.biz/BdPqJq). 

[EntitiesApp](https://ibm.biz/BdPqUi). 

[TextClassificationApp](https://ibm.biz/BdPq5p). 

[STTApp](https://watson-stt-demo.tsglwatson.buildlab.cloud/). 

[TTSApp](http://b54d9c39-us-south.lb.appdomain.cloud:8052/). 

</br></br>


### 5.2 Medium Blogs

</br>

[What are Watson Libraries](https://medium.com/ibm-data-ai/what-are-watson-libraries-6963330b9d4f)

[Sentiment analysis using Watson-NLP in a jiffy](https://medium.com/ibm-data-ai/sentiment-analysis-using-watson-nlp-in-a-jiffy-10601abaf814)

[Emotion Classification using Watson NLP](https://medium.com/@christopherchen_75597/an-introduction-to-watson-x-nlp-emotion-classification-4286c5049dea)

[Hierarchical Topic Modelling Using Watson NLP](https://medium.com/ibm-data-ai/hierarchical-topic-modeling-using-watson-nlp-6d08bac5762b)

[Entities, Keywords and Phrases Extracting Using Watson NLP](https://medium.com/@christopherchen_75597/entities-keywords-and-phrases-extracting-using-watson-nlp999-e982548a0b2)

[LDA vs Watson Topic Modelling](https://medium.com/ibm-data-ai/lda-vs-watson-nlp-topic-modeling-dbba45ca8cc7)

[Build a Watson Speech to Text (STT) service and consume with a simple java application](https://medium.com/ibm-data-ai/build-a-watson-speech-to-text-stt-service-and-consume-with-a-simple-java-application-3c9bd7a0ddfd)

[Serving Watson NLP Models on Amazon ECS](https://medium.com/ibm-data-ai/serving-watson-nlp-models-on-amazon-ecs-84ea02c6251d)

[Text Classification using Watson NLP](https://medium.com/ibm-data-ai/text-classification-using-watson-nlp-d8fa2d30b0fc)

[Speech To Text (STT) using the Watson Speech Library](https://medium.com/ibm-data-ai/speech-to-text-stt-using-watson-speech-library-42735a6047e8)

[Getting Started with Serving Watson NLP Models](https://medium.com/ibm-data-ai/get-started-with-serving-watson-nlp-models-d760d5af553c)
