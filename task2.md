# В этом файле будет CV
## Здесь заголовок 2 уровня
### А это заголовок 3 уровня

## Список достижений:

- Смог установить IDE и подключить в неё git
- Научился пользоваться markdown
- Сделал коммит
- ~~И возможно даже с первого раза~~

**А ещё можно делать вот такие списки:**
1. one
2. two
3. three

текст

1. новый список
1. можно писать 1. каждый раз
1. и это тоже будет работать
1. круто

> А это цитата
***
> А там наверху линия
---
А вот ссылка на видео с [котиком](https://youtu.be/dQw4w9WgXcQ "Там рикролл")

### А это я разбирался в  python

```
import random

def start_game():
    r_number = random.randint(1, 100)
    try_count = 5
    while try_count > 0:
        guess = int(input('Угадайте число от 1 до 100: '))
        try_count -= 1
        check_result = check_guess(guess, r_number)
        if check_result == 'same':
            print('Это правильное число')
            break
        elif check_result == 'bellow':
            print('Введёное число меньше загаданного')
            print(f'Оставшееся число попыток: {try_count}')
            continue
        elif check_result == 'above':
            print('Введёное число больше загадонного')
            print(f'Оставшееся число попыток: {try_count}')
            continue
    if try_count == 0:
        print('Попытки закончились')
        print(f'Загаданное число: {r_number}')

def check_guess(guess, r_number):
    if guess == r_number:
        return 'same'
    elif guess < r_number:
        return 'bellow'
    elif guess > r_number:
        return 'above'
```

