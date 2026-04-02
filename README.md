<p align="center">Русский&nbsp;&nbsp;|&nbsp;&nbsp;<a href="https://github.com/L0wl/JBKF/blob/main/README_en.md">English</a></p>

# JetBrains Key Factory

Простое и легкое расширение для браузера, которое позволяет генерировать коды продуктов JetBrains (включая плагины), с поддержкой до **10 языков**.

# Возможности

- [x] Выделенный компоновщик нетфильтра (через скрипт)
- [x] Нетфильтр локальной эмуляции лицензии
- [x] Поддержка до `2024.x`, `2025.x`, `2026.x` версий

# Установка

- [x] Скачайте ветку [`agent`](https://github.com/L0wl/JBKF/archive/refs/heads/agent.zip)
- [x] Скопируйте папку `jetbra` в корневой каталог диска
- [x] Откройте папку `jetbra/scripts` и запустите скрипт установки, подходящий для вашей системы

| Имя файла | Описание | Платформа |
| --------- | ----------- | -------- |
| `install-all-users.vbs` | Установка javaagent для всех пользователей | Windows |
| `install-current-user.vbs` | Установка javaagent для текущего пользователя | Windows |
| `uninstall-all-users.vbs` | Удаление javaagent для всех пользователей | Windows |
| `uninstall-current-user.vbs` | Удаление javaagent для текущего пользователя | Windows |
| `install.sh` | Установка службы javaagent для пользователя среды выполнения | Linux/Mac |
| `uninstall.sh` | Удаление службы javaagent для пользователя среды выполнения | Linux/Mac |

> [!NOTE]
> На этом этапе у вас уже будут работать ключи активации IDE

### Модуль активации плагинов

- [x] Скачайте и установите [tampermonkey](https://www.tampermonkey.net/)
- [x] [Установите скрипт](https://raw.githubusercontent.com/L0wl/JBKF/resources/script/jetbra.user.js)

> [!IMPORTANT]
> Tampermonkey должен быть установлен


# Активация

### Среды разработки

Для активации IDE перейдите в чекер [Jetbra](https://3.jetbra.in/)

### Плагины

Для начала перейдите на [Jetbrains Marketplace](https://plugins.jetbrains.com/).

Перейдите к нужному плагину - и если он платный - появятся две кнопки, обьявляющие сроки действия лицензии

![Пример](https://raw.githubusercontent.com/L0wl/JBKF/resources/examples/image.png)

При нажатии на кнопку скрипт выведет уведомление о состоянии текущей задачи.
Если задача успешно завершена, вы получите сообщение, подобное этому: "**Скопировано в буфер обмена**... и т.д.", и код, который был скопирован!
После этого шага вы можете открыть свою любимую IDE JetBrains и активировать свой плагин!

> [!NOTE]
> Если плагин не платный или недоступен, вы получите соответствующее сообщение.