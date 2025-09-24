# 🎶 Typewriter de Letras de Música (com Rich)

Este projeto em Python exibe a **letra da música *"A Última Dança"* de Link do Zap (2025)** no terminal com um efeito de **máquina de escrever**, usando a biblioteca [`rich`](https://github.com/Textualize/rich).
Cada caractere aparece gradualmente, com cores e estilos diferentes, criando uma experiência envolvente para acompanhar a canção.

## 🚀 Funcionalidades

* Mostra a **letra completa da música**.
* Efeito de **digitação caractere por caractere**.
* Estilização com `rich` (negrito, itálico, tachado, cores).
* Velocidade configurável por caractere e por linha.
* Suporte a trechos segmentados com estilos distintos na mesma frase.

## 🛠️ Tecnologias

* **Python 3.11+**
* [**Rich**](https://pypi.org/project/rich/)
* **Time** (módulo padrão do Python)

## 📂 Estrutura do código

* A função `typewriter(lines, default_char_delay, default_line_delay)` imprime a letra simulando uma máquina de escrever.
* A letra está definida na variável `linhas`, em forma de lista de tuplas ou listas de segmentos.

Exemplo de linha simples:

```python
("Foi embora sem eu ver", 0.09, 0.06, "#454545")
```

Exemplo de linha segmentada:

```python
[
    ("dançar nos braços de quem ", "#454545", 0.07),
    ("não te A M A", "bold italic red", 0.05),
]
```

## ▶️ Como executar

1. Instale a dependência:

   ```bash
   pip install rich
   ```
2. Rode o script:

   ```bash
   python main.py
   ```

## ✨ Saída esperada

Ao rodar, o terminal exibirá a letra de ***"A Última Dança"* (Link do Zap, 2025)** com efeitos de digitação e estilo, por exemplo:

```
dançar nos braços de quem  não te A M A
```

(sendo o trecho “não te A M A” exibido em **vermelho, itálico e negrito**).

## 💡 Melhorias futuras

* Suporte a múltiplas músicas carregadas de arquivos externos (`.txt` ou `.json`).
* Sincronização com áudio da música.
* Exportação da apresentação em vídeo ou GIF.
