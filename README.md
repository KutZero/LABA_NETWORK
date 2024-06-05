Чтобы установить все зависимости введи:
    pip install -r requirements.txt
    (установит все библиотеки из файл requirements.txt)
    
Чтобы запустить train_CNN.ipynb
    Либо запусти сначала prepare_data.ipynb (он подготовит данные и положит в папку labeled_dataset)
    Либо как то сам создай такую папочную структуру:
        labeled_dataset/
            train/
                blur/
                    img1.jpg
                    img2.jpg
                sharp/
                    img1.jpg
                    img2.jpg
            val/
                blur/
                    img1.jpg
                    img2.jpg
                sharp/
                    img1.jpg
                    img2.jpg
            test/
                blur/
                    img1.jpg
                    img2.jpg
                sharp/
                    img1.jpg
                    img2.jpg
    В папки blur клади размытые изображения
    В папки sharp обычные

Изображения могут быть любой ширины и высоты, в train_CNN.ipynb
они автоматом преобразуются к желаемому размеру (по умолчанию 256 на 256)

P.s. В целом из этой модели ультра просто сделать классификатор с более чем 2 классами (с 2 классами она сходу заработает без именений)
1. Скачать любой датасет изображений с классами
2. Поделить изобажения на train, val и test
3. В файле train_CNN.ipynb там где вызываются tf.keras.preprocessing.image_dataset_from_directory поменять параметр label_mode на categorical
4. Установить размер последнего слоя нейронки как кол-во классов
5. Установить LOSS_FUNCTION как categorical_crossentropy
6. Ну и если классов больше 2 сменить метрики в METRICS на подходящие
Пример: https://www.tensorflow.org/tutorials/images/data_augmentation
    