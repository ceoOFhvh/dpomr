# HW08-09

Цель: Сравнение архитектур нейросетей на CIFAR-10.

Датасет: CIFAR10 (загружается в ../datasets/ через torchvision).

Разбиение: train/val = 80/20, random seed = 42.

Эксперименты:
- E1: Однослойная сеть
- E2: Многослойная с ReLU
- E3: Глубокая + Dropout
- E4: Глубокая + BatchNorm
- O1: Сравнение оптимизаторов (SGD, Adam, RMSprop)
- O2: Влияние learning rate
- O3: Влияние batch size

Результаты: сохраняются в ./artifacts/:
- таблица экспериментов (.csv)
- конфиги (.json)
- графики (.png)
- модели (.pth)

Запуск:
pip install torch torchvision numpy matplotlib
python HW08-09.py