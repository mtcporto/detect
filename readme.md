# Detector de Objetos com Contagem Acumulativa

## Descrição
Este projeto implementa um sistema de detecção de objetos em tempo real através da webcam, com contagem acumulativa dos objetos identificados. Ele utiliza o modelo COCO-SSD do TensorFlow.js para detectar e classificar objetos em 80 categorias diferentes (pessoas, carros, animais, objetos do cotidiano, etc.).

O sistema não apenas detecta objetos em cada quadro do vídeo, mas também rastreia objetos entre quadros consecutivos utilizando o algoritmo de Intersection Over Union (IOU), permitindo contar de forma acumulativa os objetos únicos que aparecem na cena ao longo do tempo.

## Funcionalidades
- Detecção de objetos em tempo real via webcam
- Rastreamento de objetos entre quadros
- Contagem acumulativa de objetos únicos
- Ajuste do limiar de confiança para detecção
- Exibição de contagem atual e acumulada
- Exportação dos dados de contagem para arquivo JSON
- Interface traduzida para português brasileiro

## Tecnologias Utilizadas
- **HTML5**: Estruturação da página web
- **CSS3**: Estilização da interface (com Bootstrap 5)
- **JavaScript**: Lógica de programação e manipulação do DOM
- **Bootstrap 5**: Framework CSS para design responsivo
- **TensorFlow.js**: Framework de aprendizado de máquina para execução de modelos no navegador
- **COCO-SSD**: Modelo pré-treinado para detecção de objetos
- **Canvas API**: Renderização dos resultados e manipulação gráfica
- **MediaDevices API**: Acesso à webcam do usuário

## Como Usar
1. Abra a página em um navegador moderno com acesso à webcam
2. Permita o acesso à câmera quando solicitado
3. Ajuste o limiar de confiança conforme necessário utilizando o controle deslizante
4. Os objetos detectados serão mostrados com caixas delimitadoras coloridas
5. O painel direito mostra a contagem acumulativa de objetos únicos
6. Use o botão "Zerar Contagem" para reiniciar as contagens
7. Use o botão "Exportar Dados" para salvar os resultados em formato JSON

## Requisitos
- Navegador moderno com suporte a JavaScript ES6+
- Conexão à internet (para carregamento inicial das bibliotecas)
- Webcam ou câmera integrada
- Recomendado: Processador relativamente potente para melhor desempenho em tempo real

## Limitações
- O desempenho depende do hardware do dispositivo
- A precisão da detecção está limitada às capacidades do modelo COCO-SSD
- Funciona melhor com boa iluminação e objetos claramente visíveis