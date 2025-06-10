# Filtro de Sobel com OpenCV no Google Colab

Este projeto demonstra como aplicar o filtro de Sobel em uma imagem utilizando a biblioteca OpenCV, com visualização dos resultados usando Matplotlib. O código é feito para ser executado diretamente no Google Colab.

## 📷 O que é o filtro de Sobel?

O filtro de Sobel é uma técnica de detecção de bordas usada no processamento de imagens. Ele calcula a derivada da intensidade da imagem em duas direções: horizontal (eixo X) e vertical (eixo Y), destacando regiões com mudanças bruscas, como contornos e bordas.

## ⚙️ Tecnologias utilizadas

- [Python 3](https://www.python.org/)
- [OpenCV](https://opencv.org/)
- [Matplotlib](https://matplotlib.org/)
- [NumPy](https://numpy.org/)
- [Google Colab](https://colab.research.google.com/)

## 🚀 Como funciona o código

1. **Importação de bibliotecas**  
   O código importa bibliotecas essenciais: `cv2` (OpenCV), `numpy`, `matplotlib.pyplot` e `urllib.request` para leitura da imagem via URL.

2. **Leitura da imagem via link**  
   A imagem é baixada da internet diretamente a partir de um link e convertida em um formato que o OpenCV pode processar.

3. **Conversão para tons de cinza**  
   A imagem colorida é convertida para escala de cinza, uma etapa comum antes da aplicação de filtros de borda.

4. **Aplicação do filtro de Sobel**  
   - O filtro de Sobel é aplicado nas direções X e Y.
   - Os gradientes dessas direções são combinados utilizando a magnitude vetorial.
   - A imagem final é convertida para um formato exibível com `convertScaleAbs`.

5. **Exibição das imagens**  
   - A imagem original e a imagem com o filtro de Sobel aplicado são exibidas lado a lado com `matplotlib`.

## 📊 Resultado Esperado

O resultado será uma visualização com duas imagens:
- A imagem original com o título **"Imagem Original"**
- A imagem com bordas detectadas pelo filtro de Sobel com o título **"Filtro de Sobel Aplicado"**

