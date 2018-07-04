# Biblioteca de Componentes Reutilizaveis para Jogos

## Componentes Existentes

### Lista de Highscores
* **Categoria:** Back-End / Score / UI;
* **Descrição:** Cria uma lista de maiores pontuações realizadas nas partidas e os usuários que realizaram essas pontuações;
* **Exemplo de Uso:** 

```C#
  // Selecting a score type
  BasicScoreFactory scoreCreator = new BasicScoreFactory();

  // Setting the max score positions and the scene of the scores
  ScoreList scoreList = new ScoreList(MAX_POSITIONS, "Test Scene");

  // Getting current score
  ScoreData score = scoreCreator.createScore("Test Player", 10);

  // Saving score on object
  scoreList.AddScore(score);

  // Saving score on Json file
  scoreList.SaveScore();
```
