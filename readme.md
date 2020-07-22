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

Para o caminho das imagens
  ``` latex
\graphicspath{ {images/}{../images/} }
  ```
Que é o caminho pra main e o caminho para os capítulos

Dentro de document, para cada capitulo
  ``` latex
\chapter{Chapter Name}
\subfile{chapters/name}
  ```

### Capítulos
Colocar o caminho para a main em \documentclass
  ``` latex
\documentclass[../monografia.tex]{subfiles}
  ```
Não precisa colocar caminho para referências, as das imagens está na main. 

## Compilar

Apenas a main precisa ser compilada

## Referências

Usando BibTeX

Ao longo do texto
```latex
texto \cite{label}
```

reference.bib:
```latex
@type { label, 
  title = Title Name,
  author = Author Name
}
```
Colocar { } para forçar que as letras mantenham-se como maiúsculas/minúsculas. 

Supported entry types in [Bibliography - Overleaf](https://www.overleaf.com/learn/latex/Bibliography_management_in_LaTeX)

Site mega aleatório do canadá que me ajudou a saber o tipo de referência https://www150.statcan.gc.ca/n1/pub/12-591-x/2009001/01-step-etape-eng.htm