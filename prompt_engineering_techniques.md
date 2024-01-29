# Prompt Engineering

Résumé et traduction des recommandations d'OpenAI par [Françoise Halper](https://www.linkedin.com/posts/fran%C3%A7oise-halper_openai-prompter-llm-activity-7149999874963361792-qSnO/?utm_source=share&utm_medium=member_android)

1️⃣ Rédiger des instructions claires « le modèle ne peut pas lire dans nos pensées »
- Inclure des détails dans votre demande pour obtenir des réponses plus pertinentes
- Demander au modèle d'adopter un personnage
- Utiliser des délimiteurs pour indiquer des parties distinctes
- Préciser les étapes nécessaires pour mener à bien une tâche
- Donner des exemples
- Préciser la longueur souhaitée

2️⃣ Fournir un texte de référence pour réduire le risque « d’#hallucinations »
- Demander de répondre en utilisant un texte de référence ou avec des citations

3️⃣ Diviser les tâches complexes en sous-tâches plus simples
- Classifier les intentions pour identifier les instructions les plus pertinentes
- Pour les demandes de dialogue nécessitant des conversations longues, résumer ou filtrer le dialogue précédent
- Structurer les documents longs par morceaux

4️⃣ Donner au modèle le temps de « réfléchir »
- Demander une « chaîne de pensée » avant une réponse peut l’aider à trouver sa façon de corriger ses réponses
- Informer le modèle de déterminer sa propre solution avant de se précipiter vers une conclusion
- Lui demander s'il a manqué quelque chose

5️⃣ Utiliser des outils externes
- Compenser les faiblesses du modèle en lui fournissant les résultats d'autres outils
- Utiliser l'exécution de code pour effectuer des calculs plus précis ou appeler des API externes

6️⃣ Tester systématiquement les résultats
- Comparer les différents résultats obtenus en fonction des prompts utilisés
- Mettre en place une suite complète de tests, aussi appelé « #eval »