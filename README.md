
<span align="center">
    <a href="https://huggingface.co/datasets/Bhawna/MultiOCR-QA/tree/main"><img alt="Huggingface" src="https://img.shields.io/static/v1?label=Dataset&message=MultiOCR-QA&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAIGNIUk0AAHomAACAhAAA+gAAAIDoAAB1MAAA6mAAADqYAAAXcJy6UTwAAAIoUExURQAAAP/////57v/67xUVFf/clv+KAP/uzf/sxv8AAP9TAP/ltP///v/ouP/////////////////////////////8+v/pvP/biP/Vbf/Vbv/cif/qv//9+//////////03v/Yev/Zfv/14//25v/Uav/Vbv/46//////dkf/gmP/////04P/25//pvP/sxf/////lr//ouP/qwP/tyf/msv/ntf/+/P/36f/LUf/36P/w0v/w0//w0//w0//78//gm//QZv/RZv/gm//78v/////14v/nt//gnP/hn//w0f/////w0f/hn//gnP/nt//14v/////////////////LLv/MGv/PGf/LL//LG//THP/THv/SHv/UHv/LGv/LH/7SHuK8JOzDIuW+I+jAI//LHv/PTP/NF/PBG3BkOpyGMvrOH4R0NoV0NvzJGv/MF//QT//MLv/LGPu/FNayJu7FIdq2Jf7DFP/JF//ML//LJurCIsCiKujCIubAI7+hK/DHIf/LJ//HK//NGf/SHeS9IlxSP25QQmtOQmVZPu3DIf/RHf/HLP++Kf/AD/++EP3EFNCfLNhpQthrQdinKv/FFP/AEP+/K/++Dv/BEv+/Ef/CE//MIf/NIP/MGf++D//KTP/FOP/DE//PG//PHP/JGP/EFP/EM//BDf/TH//GFP/CEP/DEP/EEv/BDv/MS//IJ//JHf/JHP/JP//IQf/IHP/IJv/LSf///7SHOh0AAABUdFJOUwAAAAAAAAAAAAAAAAAABiZCQykIAUGn3/Hy4q5KAwRy7vJ/Yfb7cR/X4ipkdpepAqi5mavM2z5v/pGTtZS2QtP4999bIGyry8yUR4fJzbJ2BRIRE9ZoIHEAAAABYktHRAH/Ai3eAAAAB3RJTUUH6AIGEyohVAr+rAAAARZJREFUGNNjYGBgZGTi4xcQFBJmZmRkYQDxRUTFxCUkpaRlZBkZQXw5eYWQ0LCw0HBFJWGgCCOrskpEZFR0dExkrKoaG1BAXSMuPiExOjopOSpFU4uRgV07NS09IzMqKzsnNy9fh4OBU7egsKi4JCo6ubSsvEJPlkHfoDIqqqq6prauPiqqwVCYgcuosam5pbWtvaOzq6nbWJZBy6Snt69/wsRJk6f0TZ1masZgbjF9xsxZhbPnzJ01c8a8+ZYMVgt6F5aHLly0eGHokqVTl1kz2CxYXhi1YuWq1WuiouauXWbLYGe/bv2GjZscHDdv2bh1m5MzA7eLq5u7h6eXoLePr5+/ENDpjBwBgYH6PIyMQcF8vIyMAKnZUpQQgaV4AAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDI0LTAyLTA2VDE5OjQyOjI1KzAwOjAwybP6HAAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyNC0wMi0wNlQxOTo0MjoyNSswMDowMLjuQqAAAAAodEVYdGRhdGU6dGltZXN0YW1wADIwMjQtMDItMDZUMTk6NDI6MzMrMDA6MDBAgVbbAAAAAElFTkSuQmCC&color=20BEFF"/></a>
</span>
<a href="https://arxiv.org/pdf/2502.16781v1"><img src="https://img.shields.io/static/v1?label=Paper&message=ArXiv&color=green&logo=arXiv"></a>
<a href=""><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=red"></a>

# MultiOCR-QA: Dataset for Evaluating Robustness of LLMs in Question Answering on Multilingual OCR Texts

<img src="Images/MultiOCR-QA_pipeline.png">

MultiOCR, **a multilingual QA** dataset designed to assess the impact of OCR errors on QA systems across English, French, and German. Our dataset, derived from centuries-old documents, provides a unique evaluation of OCR-induced challenges in real-world applications.


## 🗃️Dataset

### Dataset Statistics
|                                   | English | French   | German |
| --------------------------------  | --------| ---------| ------ |
|            #QA pairs              | 10,875  | 10,004   | 39,200 | 
|           #Paragraphs             | 6,525   | 1,670    | 9,075  |
| Average paragraph length (words)  | 219.09  | 297.53   | 212.86 | 
| Average question length (words)   | 10.98   | 8.73     | 8.08   |
| Average answer length (words)     | 2.05    | 3.12     | 5.63   |
| Average questions per paragraph   | 1.67    | 5.99     | 4.32   |



**Data Structure**: 
```json
{
    "document_id": "",
    "rawOCR_text": "",
    "correctedOCR_text": "",
    "QA_pairs": [
        {
            "q_id": "",
            "question": "",
            "answer": ""
        }
    ]
}
```

- **English QA**: [Download](https://huggingface.co/datasets/Bhawna/MultiOCR-QA/resolve/main/English.json?download=true)
- **French QA**: [Download](https://huggingface.co/datasets/Bhawna/MultiOCR-QA/resolve/main/French.json?download=true)
- **German QA**: [Download](https://huggingface.co/datasets/Bhawna/MultiOCR-QA/resolve/main/German.json?download=true)


## 🪪License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ✨Citation
If you find this work useful, please cite [📜our paper](https://arxiv.org/pdf/2502.16781v1):
### Plain
Piryani, B., Mozafari, J., Abdallah, A., Doucet, A., & Jatowt, A. (2025). MultiOCR-QA: Dataset for Evaluating Robustness of LLMs in Question Answering on Multilingual OCR Texts. arXiv preprint arXiv:2502.16781
### Bibtex
```bibtex
@article{piryani2025multiocr,
  title={MultiOCR-QA: Dataset for Evaluating Robustness of LLMs in Question Answering on Multilingual OCR Texts},
  author={Piryani, Bhawna and Mozafari, Jamshid and Abdallah, Abdelrahman and Doucet, Antoine and Jatowt, Adam},
  journal={arXiv preprint arXiv:2502.16781},
  year={2025}
}

```

## 🙏Acknowledgments
Thanks to our contributors and the University of Innsbruck for supporting this project.

