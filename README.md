# Финальный проект 6 спринта

Тебя пригласили помочь зоологам: они исследуют семейство кошачьих. Чтобы записывать наблюдения, учёные используют специальную программу. Тебе предстоит протестировать часть программы.

Загляни в шпаргалки, чтобы вспомнить материал спринта.

Чтобы увеличить покрытие, нужно вызвать каждый метод каждого класса в отдельном тесте. Для каждой ветки условия напиши отдельный тест. Некоторым веткам понадобится параметризованный тест.

**Обязательное задание:**

1. Привяжи GitHub к тренажёру. Как только ты это сделаешь, в списке репозиториев автоматически появится qa_java. Там будет заготовка проекта, в которой нужно дописать код.
2. Собери Maven-проект: подключи Jacoco, Mockito и JUnit.
3. Класс Lion не должен зависеть от класса Feline. Используй принцип инъекции зависимостей.
4. Напиши моки с помощью Mockito.
5. Напиши тесты на классы Feline, Cat и Lion.
6. Подумай, где можно применить параметризацию. Реализуй параметризованные тесты.
7. Оцени покрытие с помощью Jacoco: оно должно быть не менее 100% для классов Feline, Cat и Lion.

**Дополнительное задание:**

1. Создай класс льва Алекса из мультфильма «Мадагаскар». Он будет наследником обычного льва.
2. Реализуй необходимые методы и конструктор для класса льва Алекса.
3. Покрой тестами созданный класс.

## Оценка работы:

**Для обязательного задания:**
- Нейминг элементов корректный.
- В pom.xml подключены Jacoco, Mockito и JUnit.
- Тесты лежат в src/test/java.
- Класс Lion не зависит от класса Feline.
- В тестах используются моки.
- В тестах используется параметризация.
- Классы Feline, Cat и Lion покрыты тестами на 100%.
- Сделан отчёт с помощью Jacoco.

**Для дополнительного задания:**
- Создан дополнительный класс — лев Алекс.
- Класс лев Алекс покрыт тестами.


## Информация о проекте

### Зависимости
- Jacoco для отчетов о покрытии тестами
    - Group ID: org.jacoco
    - Artifact ID: jacoco-maven-plugin
    - Version: 0.8.7

- Mockito для создания заглушек объектов в тестах
    - Group ID: org.mockito
    - Artifact ID: mockito-core
    - Version: 3.9.0
    - Область действия: тесты

- JUnit для модульного тестирования
    - Group ID: junit
    - Artifact ID: junit
    - Version: 4.13.2
    - Область действия: тесты

## Конфигурация сборки
- Директория с исходным кодом: src/main/java

### Плагины
- Настройка плагина Jacoco: Настройки плагина Jacoco для отчетов о покрытии тестами
- Настройка плагина Maven Compiler: Настройки плагина Maven Compiler

### Плагин Jacoco
- Версия: 0.8.7
- Этапы выполнения:
    - Prepare-agent: Подготовка агента для генерации отчетов о покрытии тестами
    - Report: Генерация отчетов о покрытии тестами во время этапа тестирования

## Требования

Перед началом работы убедитесь, что у вас установлены следующие компоненты:

Для версии Java проверки установленной версии Java на вашем компьютере, выполните следующую команду:

1. **Java**: Команда  используется для проверки установленной версии Java на вашем компьютере. После её выполнения вы увидите информацию о текущей установленной версии Java на вашей системе:
    ```sh
    java -version
    ```

2. **mvn**: Эта команда используется для очистки проекта и запуска тестов с использованием Apache Maven:
    ```sh
    mvn clean test
    ```