# Сегментация легких человека на основе архитектуры U-Net++

## Для данного репозитория использовался датасет [радиографических изображений легких человека covid19 от kaggle](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database/) и с помощью архитектуры U-Net++ проведена сегментация нормальных(здоровых) легких человека. Точность модели на валидационной выборке- 99%

### Стек технологий:

tensorflow, keras (layers, optimizer, model, preprocessing), numpy, pandas, matplotlib

Изображения, полученные из датасета проходят предподготовку, строится архитектура кодировщика типа U-Net++ и проходит обучение модели. Для комфортного обучения создан коллбек, который останавливает обучение, если точность не поднималась выше 2 процентов (внутри блокнота можно настроить вручную)
