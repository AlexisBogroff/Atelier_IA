## Atelier IA

### Déroulement

**Introduction** **<g>10 min</g>**
- Présentation objectifs **<b>2 min</b>**
- Votre mentor du jour **<b>2min</b>**
- Présentation du plan **<b>1 min</b>**
- Présentation de ChatGPT **<b>5min</b>**
  - **Fonctionnement**
    - Global : Entrainement modèle vs utilisation **<b>2min</b>**
    - Technique : Prompt, contexte, embeddings, calculs **<b>2min</b>**
    - A retenir : discussion courtes, contextes riches et précis **<b>30s</b>**
  - 3.5 vs 4 : limitations utilisation **<b>30s</b>**

**Demonstrations** **<g>20 min</g>**
- Cas n°1 : Génération de contenu           **<b>4min</b>**
- Cas n°2 : Vision et résumé de documents   **<b>6min</b>**
- Cas n°3 : Génération d'images             **<b>3min</b>**
- Cas n°4 : Apprentissage                   **<b>4min</b>**
- Cas n°5 : Code no-code                    **<b>3min</b>**

**Exercices** **<g>50 min</g>**
- Ex. n°1 : Traduction **<b>5</b>**
- Ex. n°2 : Génération de contenu **<b>5</b>**
- Ex. n°3 : Assistant **<b>5</b>**
- Ex. n°4 : Apprentissage **<b>5</b>**
- Exercices spécifiques **<b>30</b>**

**Conclusion** **<g>8 min</g>**
- Evolutions Journalisme x AI **<b>4min</b>**
- Evolutions techniques à venir : mémoire, compréhension, actualisation, intégration applications **<b>1min</b>**
- Au-delà du no-code: APIs, RAG et Fine-tuning **<b>3 min</b>**

**Ressources** **<g>2 min</g>**
- Apprendre **<b>30s</b>**
- Être à jour **<b>30s</b>**
- Outils **<b>1min</b>**



------------------------------------------------------------------------


### Introduction **<g>13 min</g>**


#### Objectifs **<b>1 min</b>**
- **Prise en main** de ChatGPT
- **Connaissances** possibilités, limites **<o>LLMs</o>** (**L<o>arge</o>L<o>anguage</o> M<o>odels</o>**)
- **Compréhension** globale fonctionnement LLM
- **Intuitions** impact IA sur métiers

#### Mentor du jour **<b>2min</b>**
- **Enseignant** IA et Data Science (+ 5 ans)
- Ecole ingénieur, Université, Centres de formation
- Premières certifications IA 2017 (7 ans)
- Programmation (VBA Excel, Python) il y a 7-15 ans
- Pourquoi IA me passionne ?

#### Présentation de ChatGPT **<b>10min</b>**
**Global : Entrainement modèle vs utilisation (inférence)** **<b>3min</b>**
- **Modèle** : métaphore apprentissage humain = entraînement cerveau sur données = 5 sens
- **Données** :
  - texte
  - large partie d'internet et livres
  - représentativité monde limitée (occident, faible pourcentage personnes s'expriment sur internet)
- **Entrainement** = beaucoup de données et de calculs (millions d'euros)
- **Utilisation** = peu de données et de calculs (centimes)

**Technique : Prompt, contexte, embeddings, calculs** **<b>5min</b>**
- **Prompt** : La demande
- **Contexte** : La demande **<o>+</o>** demandes précédentes **<o>+</o>** fichiers
- **Embeddings** : Texte transformé en listes de chiffres avec notion de **similarité** entre les listes
- **Calculs** : Next token prediction, Transformers (GPT), complexité quadratique

**A retenir : discussion courtes, contextes riches et précis** **<b>30s</b>**
- **Discussions taille limitée** car complexité quadratique + problèmes de mémoire
- **Contextes très détaillés** car modèles généralistes, obtenus en pratique via discussion

**ChatGPT 3.5 vs 4** **<b>1min30s</b>**
| Version | Usage | Capacités compréhension | Multimodal |
| - | - | - | - |
| **<o>3.5</o>** | sans limite | modérées | non |
| **<o>4</o>** | limité | très bonnes | oui (accès internet, lecture de document, d'images, génération d'images) |
| Mistral | variable | bonnes | non |



------------------------------------------------------------------------



### Démonstrations **<g>20 min</g>**

#### Cas 1 - Génération de contenu - [Revivre match France-Brésil 98](https://chat.openai.com/share/b36f982a-5b5a-496f-9b9a-d4c9858c736e) **<b>3min</b>**

**Pourquoi c'est impressionnant** : capacité à retranscrire ce qui semble être de l'ambiance, les personages clés et idées au-delà des faits
**En quoi est-ce limité** : très nombreux articles écrits sur le sujet, impossible d'optenir un tel résultat sur les évènements récents et moins couverts. L'IA a fait une sorte de mélange des textes sur lesquels elle s'est entraîné. Autrement dit, l'IA ne peut **reformuler** que ce que les **journalistes ont déjà écrit**.


#### Cas 2 - Vision et résumé de documents - [Application Pompiers Anki](https://chat.openai.com/c/4bc70455-19ef-4a6b-8baf-de7f931ae875) **<b>5min</b>**

**Tâche 1** : **<o>extraction texte d'une image qui représente un tableur</o>**
- **Comment** : étant une image et non un tableur Excel, nécessité extraction visuelle
- **Limites temps de calcul** : nécessite (aujourd'hui) de passer l'image en morceaux
- **Format de sortie** défini précisément
- **Capacité de compréhension** :
  - Capable de faire le lien entre les morceaux d'images
  - Capable de comprendre suffisamment pour créer des questions-réponses cohérentes, intéressantes, utiles


**Tâche 2** : **<o>extraction texte d'un document PDF</o>**
- **Type de PDF** :
  - Si **format texte** : pas de problème
  - Si **format images** : nécessite **OCR** (donc long / coûteux), ChatGPT **refusera** plusieurs pages
- **RGPD** : Attention données sensible et privées


#### Cas 3 - Génération d'images - [Dall-e-3 via ChatGPT](https://chat.openai.com/c/d276cbac-3278-49ff-9bce-a0f153885c2f) **<b>3min</b>**

**À savoir**
- **Résultats dépendent du modèle** utilisé (Dall-e, Midjourney, Stable Diffusion)
- **Précisions prompt** : Arrière-plan, Style artistique, Focale, Point de vue, Éclairage, Couleurs, Composition, Atmosphère
- **Impact** : 1 image = 1 charge d'un smartphone

**Exemple**
- **<g>Football</g>** :
  - **Plusieurs itérations** utiles
  - **Cohérence** du corps et détails


#### Cas 4 - Apprentissage - [Maths](https://chat.openai.com/c/c625296c-8b86-4aa1-b2f1-daf903eb0368) **<b>3min</b>**
- Gain de temps
- Fluidité, agréable
- Meilleure compréhension du concept et des détails
- Davantage de connaissance de concepts liés
- Voir également [GPT : enseignant SQL](https://chat.openai.com/g/g-ZwIAvMGOW-sql-enseignant-fr)

#### Cas 5 - Code no-code - [Fonctions](https://chat.openai.com/c/c625296c-8b86-4aa1-b2f1-daf903eb0368) **<b>3min</b>**
- Formater des informations [exemple simplet](https://chat.openai.com/c/7f2dfbec-adf4-40be-bb15-89744c519175)


------------------------------------------------------------------------


### Exercices **<g>50min</g>**

#### Traduction **<b>5min</b>**
**Objectif** : découvrir l'excellence du modèle en terme d'**interprétation du langage** et connaissance des **formulations dans différentes langues**. Il ne s'agit pas d'une traduction littérale.

**Mission**
- Trouver un texte en français qui est complexe et subtile
- Le traduire en anglais via ChatGPT
- Demander de reformuler les parties qui ne convienennt pas

#### Génération de contenu **<b>5min</b>**
**Ojbectif** : appréhender le niveau (mitigé) de créativité du modèle

**Mission**
- Demander à ChatGPT de générer des textes pour : un titre d'article, la description d'un sport, un poème, une blague.
- Essayez d'améliorer les résultats en conseillant ChatGPT

#### Assistant **<b>5min</b>**

**Objectif** : comprendre la structure classique d'un prompt pour des résultats efficaces

**Mission**
- Générer un plan pour un entretien avec sportif : le prompt doit utiliser la structure rôle, contexte, tâche, contraintes, format
- Demander de modifier le plan pour qu'il corresponde davantage aux besoins
- Demander de développer une section du plan


#### Apprentissage **<b>5min</b>**

**Objectif** : Découvrir comment apprendre efficacement et de manière personalisée

**Mission**
- Découvrir un nouveau sujet (sport peu connu, méthode de comptabilité, d'écriture, d'organisation, etc.)
- Demander de reformuler, d'expliquer en détail, de donner des exemples, des métaphores.
- Sois-même essayer de reformuler et demander à ChatGPT si notre compréhension est correcte


#### Exercices spécifiques **<b>30min</b>**
- Effectuez les exercices qui correspondent à votre métier
  - Basez-vous sur les méthodes de prompt engineering [recommandées par OpenAI](https://platform.openai.com/docs/guides/prompt-engineering)
  - Notamment exploitez la puissance de **chain-of-thoughts**
  - Inspirez vous éventuellemnt de ces exercices pour effectuer une tâche réelle
  - [Clicker ce lien : Enoncé exercices spécifiques](exercices.md)



------------------------------------------------------------------------


### Conclusion **<g>8 min</g>**

#### Evolutions Journalisme x AI
**De quel point de vue**
- Basé sur ma compréhension de l'IA et ses différences avec l'humain.
- Lectures impact IA sur marché de l'emploi (Gartner, Deloitte)
- Ceci n'est pas le résultat d'une thèse scientifique mais d'une réflexion à la fois subjective et anecdotique

**Hypothèses**
- Récolte information (déplacement physique)
- Interprétation évènements (émotions, atmosphère vs faits)
- Volonté et désirs (choix sujet, rendu, etc.)

**Détail réflexion**

Avantage de l'humain, et donc complémentarité :
- Intérêt à aller sur le terrain pour récupérer des informations qui ne sont pas disponibles, et prendre des notes sur l'atmosphère, le ressenti. Ensuite demander à ChatGPT d'aider à rédiger l'article.
- Empathie, compréhension des situations humaines, subtilités, couverture plus profonde des histoires
- Guider l'IA car par défaut les articles générés seront basiques, il faut le voir comme un stagiaire
- Vérification des infos et des faits sur sources fiables, d'autant plus important dans l'ère de la désinformation
- Intuitions : sur les sujets du moment, et ce qui est vraiment important, ce qui va plaire, intéresser, etc.
- Retravailler le contenu basique généré par l'IA : utilisations des techniques littéraires et journalistiques pour engager et captiver le lecteur. L'IA est aujourd'hui très limitée dans ce domaine.
- Ajouter humour, ou ton personnel humain qui accroche et rend authentique les récits.
- Expertise spécifique d'un domaine. Bien que ChatGpt soit bon dans des domaines pointus, les journalistes possèdent des connaissances qui ne sont disponibles nulle part, ChatGpt ne peut donc pas les connaître. Des techniques, des concepts ou infos sur des sujets de niche.
- Recul sur l'impact des histoires sur le public
- Meilleure compréhension nuancée du contexte actuel
- Tout ce qui est du non dit est presque innacessible aux IAs
- Adaptabilité et créativité de l'analyse
- Auto critique des propres biais et réflexions (ChatGpt peut le faire si on pense à lui demander)

**Conclusion**
- Davantage **outil** performant que **concurrent**
- Certaines tâches pourraient tendre à disparaître
- D'autres seront effectuées de manière plus **fréquente**, **large** et **en profondeur**

#### LIMITES
- **Risque de vous distraire**, peut être utile de voir ce que vous pouvez créer avant de l'utiliser, car risque d'avoir notre vision enfermée dans ses propositions.
- **Biais**: racisme, sexisme, ne connait que la culture occidentale, et tout biais qu'on peut retrouver sur internet
- **Cognition limitée** : chatgpt3.5, manque de compréhension des subtilités
- **Hallucinations** : surtout chatgpt3.5
- **Taille de contexte limitée** : pre-contexte prend de plus en plus de place, en se basant sur nos préférences, etc, donc on ne peut pas donner un ensemble de livres complets en contexte
- **Taille de discussions limitée** : devient très lent (complexité quadratique)
- **Oubli milieu de discussion** : difficile à percevoir mais démontré par études
- **Retard de mise à jour** : informations actuellement connues jusqu'en mars 2023s
- **Créativité limitée** : risque de boucler, ou dire des choses étranges (sur des requêtes de blagues par exemple)
- **Limité dans ses connaissances et sa compréhension** si sujet nécessite expertise pointue, d'autant plus sur un domaine où très peu d'informations sont disponibles sur internet 
- **Oubli** (majoritairement) entre chaque conversations, donc ne peut pas rivaliser avec un humain sur des discussions de plus de 50 messages (sur les versions actuelles)
- **Ne peut pas apprendre en temps réel**, inutile d'essayer de lui enseigner un concept pour qu'il le connaisse (surtout en espérant retrouver dans d'autres discussions)
- **Confidentialité des données** : RGPD (personnes, entreprise)
- **Capacité limitée à interpréter les émotions** : N'a pas été fine tuneé pour être psychologue ou être un ami qui remonte le moral
- **Risque de contenu offensant** : même si arrive surtout lorsque l'utilisateur souhaite volontairement jail breaker les gardes fous
- **Bridé dans ses réponses** : précisément pour éviter les problèmes (n'est pas censé donner de conseils financiers, santé, etc). Mais jail breakable facilement (méthode "imagine ...", méthode via manipulation)
- **Dépendance langage d'entrée** : comprend et parle mieux l'anglais que toute autre langue. Très limité dans les langues peu représentées sur internet
- **Limitations en pensée abstraite** : Même si deja très avancé, compliqué pour des métaphores bien adaptée (mais bon pour exemples, puisque ne nécessite pas le même degré d'abstraction)
- **Prompts évoluent** : à chaque mise à jour de modèle, et sont différents en fonction des modèles (Mistral, ChatGPT)


#### Evolutions techniques à venir **<b>1min</b>**
- mémoire, compréhension, actualisation, intégration applications 

#### Au-delà du no-code: APIs, RAG et Fine-tuning **<b>3 min</b>**
- Exemple analyse ensemble des articles écrits par L'Equipe



------------------------------------------------------------------------



### Ressources

#### Apprendre
**Code & Papiers**
- [ArxivSanity](https://arxiv-sanity-lite.com/)
- [Algorithmes Sklearn](https://scikit-learn.org/stable/)
- [Papers with Code](https://paperswithcode.com/sota)
- Prompts
  - [OpenAI prompt engineering](https://platform.openai.com/docs/guides/prompt-engineering)
  - [Prompt Engineering Roadmap](https://roadmap.sh/prompt-engineering)


**Moocs**
- [Coursera Deep Learning Spe.](https://www.coursera.org/specializations/deep-learning)
- [Coursera ChatGPT](https://www.coursera.org/courses?query=chatgpt)
- [Datacamp ChatGPT](https://www.datacamp.com/courses/introduction-to-chatgpt)
- [Datacamp LLMs](https://www.datacamp.com/blog/learn-ai-with-datacamp-new-courses-on-chatgpt-generative-ai-llms-and-more)

**Youtube**
- [LexFridman](https://www.youtube.com/@lexfridman)
- [Umar Jamil](https://www.youtube.com/@umarjamilai)
- [AI Explained](https://www.youtube.com/@aiexplained-official)
- [CodeEmporium](https://www.youtube.com/@CodeEmporium)
- [Matt Wolfe](https://www.youtube.com/@mreflow)
- [code_your_own_AI](https://www.youtube.com/@code4AI)
- [Underscore](https://www.youtube.com/@Underscore_)
- [Wes Roth](https://www.youtube.com/@WesRoth)

#### Être à jour
**Newsletters**
- [The Batch](https://www.deeplearning.ai/the-batch/)
- [Import AI](https://jack-clark.net/)

**Twitter/X**
- [Jim Fan](https://twitter.com/DrJimFan)
- [Ian Goodfellow](https://twitter.com/goodfellow_ian)
- [François Chollet](https://twitter.com/fchollet)
- [Sam Altman](https://twitter.com/sama)
- [Kyutai](https://twitter.com/kyutai_labs)
- [Sebastian Thrun](https://twitter.com/SebastianThrun)
- [Prof. Anima Anandkumar](https://twitter.com/AnimaAnandkumar)
- [Thomas G. Dietterich](https://twitter.com/tdietterich)
- [Chelsea Finn](https://twitter.com/chelseabfinn)
- [Allen Institute for AI](https://twitter.com/allen_ai)
- [Berkeley AI Research](https://twitter.com/berkeley_ai)

#### Outils

##### Chatbots
- [Poe](https://poe.com/Mistral-Medium)
- [Perplexity labs](https://labs.perplexity.ai/)
- [OpenAI Playground](https://platform.openai.com/playground)
- [LLM Finder](https://llm.extractum.io/)
- [Custom ChatGPT](https://www.chatbase.co/)
- [Purple Llama pour evaluer la sécurité des LLMs](https://about.fb.com/news/2023/12/purple-llama-safe-responsible-ai-development/)
- [Mistral AI](https://replicate.com/nateraw/mixtral-8x7b-32kseqlen)
- Leaderboards
  - [Huggin Face Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)
  - https://mistral.ai/news/la-plateforme/
  - [Julia Code Generation](https://github.com/svilupp/Julia-LLM-Leaderboard)
  - [AI vs Human](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)
  - [Matthew Berman Comparison - ChatGPT4 vs Mistral Medium](https://www.youtube.com/watch?v=S2aQpSflywA)


##### Images
- Génération d'images
  - **Midjourney**: [www.midjourney.com](https://www.midjourney.com)
  - **Leonardo AI**: [leonardo.ai](https://leonardo.ai)
  - **Pixlr**: [pixlr.com](https://pixlr.com)
  - **Yodayo**: [yodayo.com](https://yodayo.com)
  - **NightCafe**: [creator.nightcafe.studio](https://creator.nightcafe.studio)
  - **Playground AI**: [playgroundai.com](https://playgroundai.com)
  - **Visme**: [visme.co](https://visme.co)
  - **DALL-E**: [OpenAI ou ChatGPT](https://openai.com/dall-e-3)
  - **Deep AI**: [deepai.org](https://deepai.org)
  - **Runway AI**: [runwayml.com](https://runwayml.com)
  - **Bing Image Creator**: [Bing](https://www.bing.com)
- Génération d'images réalistes
  - [Midjourney V6](https://x.com/blac_ai/status/1744465413684277460?s=20) en ajoutant "posted on reddit in 2018" ou "posted on snapchat in 2018"
  - [3D Genie](https://lumalabs.ai/genie?view=one&one=1f145227-ad46-4cc4-bc2c-81a2588da23e) : génération d'objets en 3D
- Amélioration de la définition d'une image (upscale)
  - Leader mais payant : [Magnific.ai](https://magnific.ai/)
  - Gratuit : [Krea](https://www.krea.ai/apps/image/enhancer)

##### Vidéos
- **Pika labs**: [pika](https://pika.art/login)
- **Elai.io**: [elai.io](https://elai.io)
- **Runway**: [runwayml.com](https://runwayml.com)
- **Filmora**: [filmora.wondershare.com](https://filmora.wondershare.com)
- **DeepBrain AI**: [deepbrain.ai](https://deepbrain.ai)
- **Veed.io**: [veed.io](https://veed.io)
- **Synthesia**: [synthesia.io](https://synthesia.io)
- **Synthesys**: [synthesys.io](https://synthesys.io)
- **D-ID**: [d-id.com](https://d-id.com)
- **Pictory**: [pictory.ai](https://pictory.ai)

##### Audio
- [Transformer la voix en musique](https://create.musicfy.lol/)
- [Retranscription d'un fichier audio avec insanely-fast-whisper](https://github.com/Vaibhavs10/insanely-fast-whisper)
- [Modifier la voix "speech to speech" - Elevenlabs](https://elevenlabs.io/)
- **Google Speech-to-Text**: [cloud.google.com/speech-to-text](https://cloud.google.com/speech-to-text)
- **IBM Watson Speech to Text**: [www.ibm.com/cloud/watson-speech-to-text](https://www.ibm.com/cloud/watson-speech-to-text)
- **Rev.com**: [www.rev.com](https://www.rev.com)
- **Otter.ai**: [otter.ai](https://otter.ai)
- **Sonix**: [sonix.ai](https://sonix.ai)
- **Trint**: [www.trint.com](https://www.trint.com)
- **Amberscript**: [www.amberscript.com](https://www.amberscript.com)
- **Descript**: [www.descript.com](https://www.descript.com)
- **Happy Scribe**: [www.happyscribe.com](https://www.happyscribe.com)
