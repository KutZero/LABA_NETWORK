#Чтобы установить все зависимости введи: pip install -r requirements.txt (установит все библиотеки из файл requirements.txt)

#Чтобы запустить train_CNN.ipynb 
##Либо запусти сначала prepare_data.ipynb (он подготовит данные и положит в папку labeled_dataset) 
##Либо как то сам создай такую папочную структуру: 
labeled_dataset/ 
train/ 
&nbsp;&nbsp;&nbsp;&nbsp;blur/ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img1.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img2.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;sharp/ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img1.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img2.jpg 
val/ 
&nbsp;&nbsp;&nbsp;&nbsp;blur/ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img1.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img2.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;sharp/ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img1.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img2.jpg 
test/ 
&nbsp;&nbsp;&nbsp;&nbsp;blur/ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img1.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img2.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;sharp/ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img1.jpg 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;img2.jpg 

В папки blur клади размытые изображения В папки sharp обычные

Изображения могут быть любой ширины и высоты, в train_CNN.ipynb они автоматом преобразуются к желаемому размеру (по умолчанию 256 на 256)
