# Women's History Project API

## Описание

Этот проект представляет собой REST API для управления данными о знаменитых женщинах в истории. API позволяет создавать, просматривать, изменять и удалять записи о знаменитых женщинах, а также управлять категориями, к которым они относятся.

## Технологии

- Django & Django REST Framework для создания API
- Token Authentication для аутентификации запросов
- Пользовательские разрешения для контроля доступа

## Модели

- `Women`: Основная модель, содержащая информацию о знаменитых женщинах.
- `Category`: Модель для категорий, к которым относятся женщины.

## Сериализаторы

- `WomenSerializer`: Сериализатор для модели `Women`.

## Права доступа

- `IsAdminOrReadOnly`: Предоставляет доступ на чтение всем пользователям и полный доступ только администраторам.
- `IsOwnerOrReadOnly`: Предоставляет полный доступ владельцу записи и доступ на чтение всем остальным.

## Вьюсеты

- `WomenAPIList`: Вьюсет для списка женщин с пагинацией.
- `WomenAPIUpdate`: Вьюсет для обновления данных о женщинах.
- `WomenAPIDestroy`: Вьюсет для удаления записей о женщинах.

Инструкции по запуску и использованию API будут зависеть от конкретной конфигурации и окружения.
