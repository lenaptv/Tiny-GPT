# Tiny-GPT "AI-да Пушкин!"
Tiny-GPT: трансформер своими лапками. 

Написала decoder-only и character-based трансформер с нуля на PyTorch на основе статьи "Attention is all you need", 2017
https://arxiv.org/pdf/1706.03762v5.pdf
и двух видео от Андрея Карпаты
1) https://www.youtube.com/watch?v=kCc8FmEb1nY&t=1s

2) https://www.youtube.com/watch?v=XfpMkf4rD6E&list=PLoROMvodv4rNiJRchCzutFw5ItR_Z27CM&index=11

Для ускорения процесса обучения использовала torch.compile() из PyTorch 2.0.
По своей архитектуре - это только декодер, то есть отсутсвует часть, выделенная красным на рисунке ниже, в отличие от архитектуры, описанной в оригинальной статье "Attention is all you need"
![image alt] (https://github.com/lenaptv/Tiny-GPT-/blob/main/decoder-only.png)
