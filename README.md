# 🍌 Pipeline de Detecção e Segmentação (YOLO)

pip install ultralytics

Este trecho de código automatiza o processamento de imagens utilizando modelos de visão computacional. Ele permite filtrar classes específicas, aplicar segmentação de instância e rastrear objetos.

## 🚀 Exemplo de Uso

Utilize a função `run_pipeline` para processar arquivos individuais no ambiente do Google Colab ou localmente:

```python
run_pipeline(
    input_path="/content/exemplo.jpeg",      # Caminho da imagem ou video original
    output_path="/content/exemplo.jpeg",     # Destino do resultado anotado
    classes=[0, 16, 46],                      # IDs: 0=Pessoa, 16=Cachorro, 46=Banana, para o uso das 80 classes do YOLO so deixar vazio
    use_tracking=True,                        # Habilita o rastreio de objetos
    use_segmentation=True                     # Ativa a máscara de contorno (segmentação)
)

