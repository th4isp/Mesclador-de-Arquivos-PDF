# 🗂️ PDF Merger

📄✨ **PDF Merger** é uma ferramenta simples para combinar vários arquivos PDF em um único documento. Ideal para organizar e consolidar documentos em um só lugar!

## 🚀 Funcionalidades

- **📂 Listagem e Ordenação**: Lista todos os arquivos PDF em um diretório específico e os organiza em ordem alfabética.
- **🔄 Mesclagem**: Combina os arquivos PDF listados em um único PDF final.
- **📝 Saída Final**: Gera um novo arquivo PDF com todos os documentos combinados.

## 🛠️ Como Usar

1. **Coloque seus arquivos PDF** no diretório `arquivos`.
2. **Execute o script** para combinar todos os PDFs na pasta.
3. **Encontre o PDF final** como `PDF Final.pdf` no diretório de trabalho.

```python
import PyPDF2
import os

merger = PyPDF2.PdfMerger()

lista_arquivos = os.listdir("arquivos")
lista_arquivos.sort()
print(lista_arquivos)

for arquivo in lista_arquivos:
    if ".pdf" in arquivo:
        merger.append(f"arquivos/{arquivo}")

merger.write("PDF Final.pdf")
```

## 📦 Requisitos

- `PyPDF2`: Instale com `pip install PyPDF2`
- Python 3.x


## 🧩 Contribua

Sinta-se à vontade para contribuir com melhorias ou correções. 

---

