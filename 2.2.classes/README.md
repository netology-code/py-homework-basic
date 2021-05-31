# Домашнее задание к лекции 2.2 «Классы и их применение в Python»

### Tasks 1-2
```
class Sheep:
    sound = 'бе бе'

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight

    def say(self):
        print(self.sound)

    def feeding(self):
        print('Вы покормили', self.name)

    def shearing(self):
        print('Вы постригли', self.name)


class Goose:
    sound = 'га га'

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight

    def say(self):
        print(self.sound)

    def feeding(self):
        print('Вы покормили', self.name)

    def collect_eggs(self):
        print('Вы собрали яйца у ', self.name)


class Chicken:
    sound = 'ко ко'

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight

    def say(self):
        print(self.sound)

    def feeding(self):
        print('Вы покормили', self.name)

    def collect_eggs(self):
        print('Вы собрали яйца у ', self.name)


class Duck:
    sound = 'кря кря'

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight

    def say(self):
        print(self.sound)

    def feeding(self):
        print('Вы покормили', self.name)

    def collect_eggs(self):
        print('Вы собрали яйца у ', self.name)


class Cow:
    sound = 'му му'

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight

    def say(self):
        print(self.sound)

    def feeding(self):
        print('Вы покормили', self.name)

    def milk(self):
        print('Вы подоили', self.name)


class Goat:
    sound = 'бе бе'

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight

    def say(self):
        print(self.sound)

    def feeding(self):
        print('Вы покормили', self.name)

    def milk(self):
        print('Вы подоили', self.name)
```

### Task 2
```
grey_goose = Goose('Серый', 15)
white_goose = Goose('Белый', 12)
cow = Cow('Манька', 120)
barashek = Sheep('Барашек', 59)
kudryash = Sheep('Кудрявый', 65)
koko_hen = Chicken('Ко-Ко', 8)
kuka_hen = Chicken('Кукареку', 5)
goat_0 = Goat('Рога', 37)
goat_1 = Goat('Копыта', 38)
duck = Duck('Кряква', 19)

animals = [grey_goose, white_goose, cow, barashek, kudryash, koko_hen, kuka_hen, goat_0, goat_1, duck]
common_sum = 0
max_weight = grey_goose.weight
max_weight_name = grey_goose.name

for animal in animals:
    common_sum += animal.weight
    if animal.weight > max_weight:
        max_weight = animal.weight
        max_weight_name = animal.name

print('Общий вес животных', common_sum, 'кг')
print('Самый тяжелый', max_weight_name)
```
