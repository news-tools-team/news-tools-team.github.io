---
icon: skip-24
label: Управление редакторами
layout: default
order: 100
---

# Управление редакторами /maker

## `/maker register`

[!badge variant="warning" text="Необходимый уровень доступа: **2**"]

!!!info Описание команды
Команда служит для регистрации нового редактора в системе.
!!!

### `Параметры`

|   Параметр   |                Значение               | Обязательный | Примечание |
|:------------:|:-------------------------------------:|:------------:|:----------:|
|   **maker**  | Пользователь из списка или Discord ID |      Да      |      -     |
| **nickname** |      Никнейм редактора в системе      |      Да      |      -     |

### `Ограничения`

1. У вас не получится зарегистрировать редактора, если он уже существует в системе.

### `Пример`

[!embed](/static/examples/maker-register.gif)


## `/maker activate`

[!badge variant="warning" text="Необходимый уровень доступа: **2**"]

!!!info Описание команды
Команда служит для активации редактора в системе.
!!!

### `Параметры`

|   Параметр   |                Значение               | Обязательный | Примечание |
|:------------:|:-------------------------------------:|:------------:|:----------:|
|   **maker**  | Пользователь из списка или Discord ID |      Да      |      -     |
| **nickname** |      Никнейм редактора в системе      |      Да      |      -     |

### `Ограничения`

1. У вас не получится активировать редактора, если он не зарегистрирован в системе.
2. У вас не получится активировать редактора, если он уже активен.

### `Пример`

[!embed](/static/examples/maker-activate.gif)


## `/maker deactivate`

[!badge variant="warning" text="Необходимый уровень доступа: **2**"]

!!!info Описание команды
Команда служит для деактивации аккаунта редактора.
!!!

### `Параметры`

|  Параметр  |                Значение               | Обязательный |      Примечание      |
|:----------:|:-------------------------------------:|:------------:|:--------------------:|
|  **maker** | Пользователь из списка или Discord ID |      Да      |           -          |
| **reason** |          Причина деактивации          |      Да      | Отображается в логах |

### `Ограничения`

1. У вас не получится деактивировать редактора, если он не зарегистрирован в системе.
2. У вас не получится деактивировать редактора, если он уже деактивирован.
3. У вас не получится деактивировать редактора, уровень которого равен или выше вашего.

### `Пример`

[!embed](/static/examples/maker-deactivate.gif)


## `/maker setdiscord`

[!badge variant="warning" text="Необходимый уровень доступа: **2**"]

!!!info Описание команды
Команда служит для смены привязки аккаунта в системе News Tools к аккаунту Discord.
!!!

### `Параметры`

|  Параметр |                   Значение                  | Обязательный | Примечания |
|:---------:|:-------------------------------------------:|:------------:|:----------:|
| **maker** |    Пользователь из списка или Discord ID    |      Да      |      -     |
|  **user** | Новый пользователь из списка или Discord ID |      Да      |      -     |

### `Ограничения`

1. У вас не получится сменить привязку, если пользователь не зарегистрирован в системе.
2. У вас не получится сменить привязку, если **новый пользователь** уже зарегистрирован в системе.
3. У вас не получится сменить привязку, если уровень пользователя равен или выше вашего.

### `Пример`

[!embed](/static/examples/maker-setdiscord.gif)


## `/maker setnickname`

[!badge variant="warning" text="Необходимый уровень доступа: **2**"]

!!!info Описание команды
Команда служит для смены никнейма редактору.
!!!

### `Параметры`

|   Параметр   |                Значение               | Обязательный | Примечания |
|:------------:|:-------------------------------------:|:------------:|:----------:|
|   **maker**  | Пользователь из списка или Discord ID |      Да      |      -     |
| **nickname** |             Новый никнейм             |      Да      |      -     |

### `Ограничения`

1. У вас не получится сменить никнейм, если редактор не зарегистрирован в системе.
2. У вас не получится сменить никнейм, если уровень редактора равен или выше вашего.

### `Пример`

[!embed](/static/examples/maker-setnickname.gif)