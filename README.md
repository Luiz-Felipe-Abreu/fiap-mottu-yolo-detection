## 📌 Descrição do Projeto

Este projeto aplica técnicas de **Visão Computacional com Inteligência Artificial** para detectar, rastrear e mapear a localização de motos em pátios de filiais da empresa **Mottu**. Utilizando o modelo **YOLOv8**, o sistema é capaz de identificar motos automaticamente em imagens e exibir suas posições em um **mapa 2D** interativo, facilitando o monitoramento da frota.

Link da demonstração do sistema: https://www.youtube.com/watch?v=M1wSZYwTVlc&ab_channel=LuizFelipe
---

## 🧪 Tecnologias Utilizadas

- **Python** – linguagem base do projeto  
- **YOLOv8 (Ultralytics)** – modelo de IA para detecção de motos  
- **OpenCV** – processamento e exibição de imagens     
- **Matplotlib** – exibição visual do mapa 2D  
- **Pathlib / OS** – gerenciamento de arquivos e pastas

---

## ⚙️ Como o Sistema Funciona

1. O usuário adiciona imagens diretamente na **pasta raiz do projeto**.
2. Em seguida, executa as células do código **em ordem**, para processar cada imagem.
3. O modelo detecta automaticamente as motos (classe 3), filtra duplicações e salva as **coordenadas (bounding boxes)**.
4. As posições são exibidas no terminal e também em um **mapa 2D** visual.
5. Todos os resultados (imagens com as detecções) são salvos na pasta `resultados_imagens/detectados`.

---

## ▶️ Instruções de Uso

1. **Instale as bibliotecas necessárias:**
   ```bash
   pip install ultralytics supervision opencv-python
   ```

2. **Adicione as imagens** que deseja analisar na **pasta raiz** do projeto.

3. **Execute as células do código em ordem**. Cada célula possui uma função específica:

---

## 🧩 Resumo das Células do Código

| Nº | O que a célula faz                                                                 |
|----|------------------------------------------------------------------------------------|
| 1  | Instala as bibliotecas necessárias.                                                |
| 2  | Importa as bibliotecas usadas no projeto.                                          |
| 3  | Carrega o modelo pré-treinado YOLOv8x.                                             |
| 4  | Define uma função para **filtrar motos duplicadas** muito próximas.                |
| 5  | Executa a **detecção de motos** na imagem, salva os resultados e as coordenadas.   |
| 6  | Mostra visualmente as detecções feitas pelo YOLO e imprime os detalhes.            |
| 6* | (Extra) Explora os dados brutos retornados pelo modelo.                            |
| 7  | Detecta motos em todas as imagens da pasta, salvando coordenadas por ID.           |
| 8  | Lista e processa automaticamente todas as imagens da pasta raiz.                   |
| 9  | Permite **consultar a posição de uma moto específica** por ID.                     |
| 10 | Exibe um **mapa 2D com a localização central** de todas as motos detectadas.       |
| 11 | Lista os IDs detectados no terminal e mostra o mapa com todos eles.                |


## 👨‍💻 Desenvolvido por

- Nome: Luiz Felipe
- RM: 555197

- Nome: Pedro Gomes
- RM: 553907

- Nome: Matheus Munuera 
- RM: 557812
