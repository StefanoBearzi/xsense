# ha-xsense-component_test

<p align="center">
<img src="https://github.com/user-attachments/assets/8e05446e-bc14-4a21-9f6d-8e9f9defd630" alt="Image">
</p>

## Обзор
Эта интеграция для Home Assistant позволяет использовать устройства Xsense в системе умного дома. Она была создана на основе оригинального кода [Theo Snel](https://github.com/theosnel/homeassistant-core/tree/xsense/homeassistant/components/xsense) и опубликована с его разрешения и в сотрудничестве с ним.

Пока не будет доступна официальная интеграция Home Assistant от Theo, будет использоваться эта интеграция HACS, которая регулярно обновляется для добавления новых функций и устранения существующих проблем. Эта интеграция позволяет пользователям легко интегрировать свои устройства Xsense в Home Assistant и использовать их для различных автоматизаций и мониторинга.

<p align="center">
  <img src="https://github.com/user-attachments/assets/fbe7e69b-9204-4de4-a245-e0e2bdbd7f73" alt="Image">
</p>

## Функции
- Интеграция различных устройств Xsense в Home Assistant.
- Поддержка автоматизаций на основе данных датчиков Xsense.
- Поддержка следующих типов устройств: базовые станции, датчики дыма, датчики угарного газа, тепловые датчики, датчики протечки воды и гигрометры.
- Простая установка через HACS (Home Assistant Community Store).

## Требования
- Рабочий сервер Home Assistant (рекомендуется последняя версия).
- Учетная запись Xsense с поддерживаемыми устройствами.
- Для установки интеграции необходимо установить HACS в Home Assistant.

## Видеоруководство
Для подробного руководства по установке и настройке интеграции вы можете посмотреть следующее видео:

[![X-Sense Home Assistant Integration](https://img.youtube.com/vi/3CCKK-qX-YA/0.jpg)](https://www.youtube.com/watch?v=3CCKK-qX-YA)

____________________________________________________________

## Подготовка
Перед установкой интеграции необходимо выполнить несколько подготовительных шагов:

- **Создайте вторую учетную запись в приложении X-Sense (для использования с Home Assistant)**: Так как невозможно одновременно войти в приложение и в Home Assistant с одной и той же учетной записью, мы рекомендуем использовать отдельную учетную запись для Home Assistant. Это предотвратит постоянный выход из приложения или Home Assistant. Дополнительная учетная запись обеспечивает плавную интеграцию и непрерывное использование без повторных отключений.

- **Поделитесь поддерживаемыми устройствами из основной учетной записи с учетной записью Home Assistant**: Используйте приложение X-Sense, чтобы поделиться **только поддерживаемыми устройствами** с вновь созданной учетной записью. Таким образом, вы сможете легко использовать интеграцию в Home Assistant, продолжая управлять устройствами через свою основную учетную запись.

![image](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/9cc18693-5f37-49c5-a67d-22602fa7eef5)

____________________________________________________________

## Установка через HACS
1. **Откройте HACS в Home Assistant**:
   HACS - это важное расширение для Home Assistant, которое позволяет легко устанавливать пользовательские интеграции.

   ![Download (1)](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/3220c686-f53f-4766-9523-e3272a6ff104)

2. **Перейдите в пользовательские репозитории**:
   Перейдите на панели HACS в настройки и добавьте репозиторий в качестве пользовательского источника.

3. **Добавьте репозиторий**:
   Введите URL репозитория: `https://github.com/Jarnsen/ha-xsense-component_test`

   ![image](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/48c23cf0-a212-4889-8d08-f995ff2fd5d7)

4. **Загрузите и установите интеграцию**:
   Найдите интеграцию в HACS, скачайте и установите её. После установки настройка может быть выполнена через интерфейс Home Assistant.

   ![image](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/5bd2d567-6568-47c5-a45e-6af7228ff30e)
   
   ![image](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/33cd7bfa-eec2-44f5-af30-4f21269f0081)

____________________________________________________________

## Настройка
После установки необходимо выполнить базовую настройку, чтобы правильно настроить интеграцию:
- **Имя пользователя и пароль**: Используйте данные для входа из вновь созданной учетной записи X-Sense, чтобы установить соединение.

    ![image](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/48c5e923-a6a0-4a47-8f26-8ef3954ea34b)
  
- **Обзор устройств**: После успешной настройки общие устройства будут доступны в Home Assistant и могут быть использованы для автоматизаций.

    ![image](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/42b33b6b-ecd9-45f6-99fc-314a0abd9bbe)
## Просмотр в Home Assistant
После успешной установки и настройки интеграция будет видна в Home Assistant. Устройства будут доступны на панели и могут быть использованы для автоматизаций, уведомлений и других случаев использования.


![Форум](https://github.com/Elwinmage/ha-xsense-component/assets/15807572/2d271b78-39d9-4bbd-837d-8593cf1933bd)

____________________________________________________________

## Поддерживаемые устройства
Эта интеграция поддерживает различные устройства Xsense. Вот список подтвержденных и протестированных устройств:
- **Базовая станция (SBS50)**: Центральный узел для устройств Xsense.
- **Тепловой датчик (XH02-M)**: Обнаружение необычно высоких температур.
- **Датчик угарного газа (XC01-M; XC04-WX)**: Обнаруживает опасные концентрации угарного газа.
- **Датчик дыма (XS01-M, WX; XS03-WX; XS0B-MR)**: Раннее обнаружение дыма.
- **Комбинированный датчик угарного газа и дыма (SC07-WX; XP0A-MR (частично поддерживается))**: Обнаруживает как угарный газ, так и дым.
- **Датчик протечки воды (SWS51)**: Обнаруживает наличие воды в нежелательных местах.
- **Гигрометр-термометр (STH51)**: Мониторинг температуры и влажности.

Эти устройства могут быть использованы для создания автоматизаций и оповещений после интеграции в Home Assistant.

____________________________________________________________

## Примеры автоматизаций
С помощью этой интеграции можно создать различные автоматизации. Вот несколько примеров:

### Пример 1: Предупреждение о температуре
Если температура на термометре Xsense становится слишком высокой, отправляется уведомление:

```yaml
automation:
  - alias: "Предупреждение о температуре Xsense"
    trigger:
      platform: numeric_state
      entity_id: sensor.xsense_temperature
      above: 30
    action:
      service: notify.notify
      data:
        message: "Температура превышает 30 градусов!"
```

### Пример 2: Сигнализация датчика протечки воды
Когда датчик протечки воды обнаруживает воду, активируется предупреждение:

```yaml
automation:
  - alias: "Сигнализация датчика протечки воды"
    trigger:
      platform: state
      entity_id: binary_sensor.xsense_waterleak
      to: "on"
    action:
      service: notify.notify
      data:
        message: "Обнаружена утечка воды!"
```

____________________________________________________________

## Нам нужна ваша помощь
Мы всегда ищем поддержку для дальнейшей разработки и улучшения этой интеграции. Вот несколько способов, как вы можете помочь:

1. **Тестирование устройств**: Если у вас есть устройство Xsense, которое работает с этой интеграцией, дайте нам знать, чтобы мы могли добавить его в список поддерживаемых устройств.

2. **Отзыв о неподдерживаемых устройствах**: Если устройство не работает, сообщите нам, чтобы мы могли предоставить поддержку или включить его в будущие версии интеграции.

3. **Совместное использование устройств для тестирования**: Лучший способ тестирования новых устройств - это совместное использование устройства через приложение X-Sense. Так мы сможем убедиться, что поддерживаются как можно больше устройств.

4. **Поддержка сообщества**: Участвуйте в обсуждениях в нашем сообществе. Если у вас есть предложения по улучшению или вы помогаете другим пользователям с их установкой - любая помощь приветствуется!

Для обсуждений и поддержки вы можете присоединиться к нашему серверу Discord или форуму Home Assistant:

[Discord](https://discord.gg/5phHHgGb3V)

[Форум](https://community.home-assistant.io/t/x-sense-security-is-it-possible-to-create-an-integration/534119/110)
