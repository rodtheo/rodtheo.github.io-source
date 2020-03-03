# Como publicar um jupyter notebook no Medium

1. Converter o ipynb em markdown usando o template `/Users/rodtheo/miniconda2/envs/bioPy3//lib/python3.6/site-packages/nbconvert/templates/markdown_medium.tpl`. Este template adiciona a primeira a palavra `block.py` na primeira linha de cada block de codigos. Isso eh importante para a conversao do md em post pelo site https://markdowntomedium.com/.

```
jupyter nbconvert --template=markdown_medium.tpl --to markdown FastAI_lesson_1_Pierre.ipynb
```

2. Copiar o conteudo o md e colar no site markdowntomedium.com.

3. Exportar as imagens do ipynb para um diretorio e abrir elas manualmente atraves da edicao do post no medium. Isso eh automaticamente realizado pelo nbconvert que cria um diretorio contendo as imagens do ipynb.

