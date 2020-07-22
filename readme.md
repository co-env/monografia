# Monografia 

*monografia.tex* main file

*./chapters* um arquivo .tex para cada capitulo

*./images* todas as imagens da monografia

*reference.bib* arquivo com todas as referências da monografia

## Capítulos

### Main
Incluir no cabeçalho
  ``` latex
\usepackage{subfiles}
  ```

Dentro de document, para cada capitulo
  ``` latex
\chapter{Chapter Name}
\subfile{chapters/name}
  ```

### Capítulos
Colocar o caminho para a main em \documentclass
  ``` latex
\documentclass[monografia.tex]{subfiles}
  ```
Não precisa colocar caminho para imagens, referências, etc

## Compilar

Apenas a main precisa ser compilada