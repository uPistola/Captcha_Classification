# 🧠 Captcha_Classification

Este projeto implementa um pipeline completo para reconhecimento de CAPTCHAs, incluindo:

1. **Geração de CAPTCHAs sintéticos**
2. **Segmentação e normalização** dos caracteres
3. **Treinamento dos modelos YOLOv11, ResNet-50 e CRNN**
4. Exemplo de **avaliação por grupos** e visualização dos resultados

---

## 📂 Estrutura do repositório

```
Captcha_Classification/
├── fonts/ # Fonts utilizadas para a criação dos Captchas Textuais
├── src/ # Scripts principais
│ ├── YoloV11.ipynb #
│ ├── CRNN.ipynb #
│ ├── ResNet50.ipynb #
│ ├── TextCaptchas.ipynb # Responsavel por todos os testes e treinos no Captchas Textuais
├── models/ # Modelos salvos (ex: melhor modelo .pth)
├── Runs
│ ├── ... Contem todas as Runs de treino do Modelo Yolo
└── README.md # Este arquiv
├── CaptchaGeneration.py
├── DatasetProcessors.py

```

## ⚙️ Principais scripts

- **`CaptchaGeneration.py`**: cria imagens demonstrativas de CAPTCHAs com texto randomizado, distorções e ruído. Cria tanto o dataset Base quando com Wave Distortion
- **`DatasetProcessors.py`**: Realiza o download do CIFAR, requer o download prévio do dataset Google Recaptcha v2, e realiza o Holdout (80% - 20%) necessário para o treinamento dos modelos.
- **`src/***`**: Pasta que contem os Notebook de cada modelo, cada arquivo é necessario para treinamento de validação dos resultados utilizados.
- **`models/***`**: Pasta Responsavel por armazenar os melhores pesos de cada modelo treinado.

## ⚙️ Dataset Utilizados (Links Externos)

- **`Google Recaptcha v2`**: https://www.kaggle.com/datasets/mikhailma/test-dataset
- **`Cifar-100`**: https://www-cs-toronto-edu.translate.goog/~kriz/cifar.html?_x_tr_sl=en&_x_tr_tl=pt&_x_tr_hl=pt&_x_tr_pto=tc

- **`Drive com datasets Textuais`**: 
