# Coina

![](https://github.com/Yazan98/KMM-Cryptocurrency/blob/main/resources/app_landing_screen.png?raw=true)

> Криптовалютное мобильное приложение

![](https://github.com/Yazan98/Coina/blob/main/resources/Screenshot%202022-12-30%20at%2010.32.59%20AM.png?raw=true)

![](https://github.com/Yazan98/Coina/blob/main/resources/Screenshot%202022-12-30%20at%2011.29.07%20AM.png?raw=true)


## Описание

Данный проект представляет собой мультиплатформенное мобильное приложение на Kotlin, построенное на платформах Android и IOS для отображения информации о криптовалютах на основе бесплатного [Api](https://www.coingecko.com/en/api/documentation).
Это приложение является простой демонстрацией того, как я могу интегрировать общую логику между двумя платформами для сохранения данных с/без сессии, Api запросов, запросов к базе данных.


## Общие части

Это приложение имеет общий модуль, который содержит код, разделяемый между двумя платформами
1. Запросы к базе данных (запись, чтение, пользовательские запросы)
2. Хранилище ключей и значений (UserDefaults, SharedPrefs)
3. Api-запросы (все API)
4. UseCases (каждый UseCase для каждого экрана)


## Особенности приложения

1. Экран входа в систему
2. Главный экран
3. Список монет
4. Список бирж
5. Список категорий
6. Список монет категории


## Компоненты, использованные для создания этого приложения

### Общий модуль

1. Клиент Ktor
2. Realm Kotlin SDK
3. Kotlinx-Serialization
4. Нативные кокоаподы

### Модули для Android

1. Многомодульное приложение (каждая функция имеет свой модуль)
2. Jetpack Compose
3. Материал 3
4. Клиент Ktor для Android
5. Жизненный цикл - ViewModels
6. Hilt
7. Kapt
8. Сервисы Google Play
9. Jetpack Compose - компоненты навигации
10. Jetpack Compose Accompanist - контроллер пользовательского интерфейса
11. Coil - загрузка изображений
12. Timber
13. MultiDexMerge
14. Firebase
15. MPAndroidChart

### Приложение для IOS
1. SwiftUI
2. Google MaterialComponents - Snackbar
3. ObjectMapper
4. Общий модуль
5. Зависимости Cocoapods
6. Клиент Ktor Darwin


## Учебные части приложения

1. Экран авторизации для тестирования (SharedPrefs, UserDefault) с тем же менеджером значений ключей
2. Список монет Моделирование нескольких сценариев использования и действий в одной модели представления
3. Список монет Моделирование одного и того же запроса к базе данных для поиска в монетах
4. Список категорий Моделирование навигации между экранами в каждой платформе
5. Авторизация, главный экран Поддержка темного и белого режимов в каждой платформе
6. Структура проекта построена на основе cocoapods для импорта общей библиотеки 


## Информация о потоке приложений


1. Поток пользователей в приложении
![](https://github.com/Yazan98/Coina/blob/main/resources/User%20Flow.jpg?raw=true)
2. Поток функций на каждом экране
![](https://github.com/Yazan98/Coina/blob/main/resources/Feature%20Flow.jpg?raw=true)


## Информация о скриншотах

1. [Изображения приложения](https://github.com/Yazan98/Coina/tree/main/resources)
2. [Видео сравнения Android, IOS](https://github.com/Yazan98/Coina/blob/main/resources/Compare%20Platforms.mp4)


## Требования к IDE

1. Android Studio Версия: Android Studio Flamingo | 2022.2.1 Canary 5
2. XCode Версия: Версия 14.2 (14C18)


## Шаги для запуска проекта

```
1. Откройте Android Studio с приложением Root
2. Откройте терминал и выполните команду (pod install).
Если сборка Gradle не удалась в первый раз
3. Выполните команду (cd iosApp)
4. Выполните команду (pod install)
5. Запустите приложение Android
6. Откройте XCode с папкой iosApp
7. Выполните команду (pod update shared)
8. Запустите приложение IOS
```


## Полезные ресурсы

1. [Key Value Store](https://medium.com/@shmehdi01/shared-preference-in-kmm-kotlin-multiplatform-2bca14214093)
2. [SwiftUI](https://www.youtube.com/watch?v=TTYKL6CfbSs&list=PLwvDm4Vfkdphbc3bgy_LpLRQ9DDfFGcFu)
3. [Shared ViewModels](https://proandroiddev.com/kotlin-multiplatform-mobile-and-how-share-viewmodel-an-architecture-proposal-b6f86b61abf9)
4. [Shared ViewModels](https://medium.com/double-symmetry/kotlin-multiplatform-tales-a-shared-viewmodel-f9d0792f69f9)
5. [Ktor Documentation](https://ktor.io/docs/getting-started-ktor-client-multiplatform-mobile.html)
6. [KMM Documentation](https://kotlinlang.org/docs/multiplatform-mobile-ktor-sqldelight.html)
7. [Api Link](https://www.coingecko.com/en/api/documentation)
8. [Android Charts Library](https://github.com/PhilJay/MPAndroidChart)
9. [Realm Kotlin SDK](https://www.mongodb.com/docs/realm/sdk/kotlin/install/kotlin-multiplatform/)
10. [XCode-Kotlin Plugin](https://github.com/touchlab/xcode-kotlin)
