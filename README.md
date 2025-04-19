# HA-button-card-template
![Image alt](20241618.png)
### Установка
Необходимо чтобы был установлен [Button card](https://github.com/custom-cards/button-card). 

Войдите в режим редактирования панели Lovelace, нажмите три точки в верхнем правом углу, выберите: "Текстовый редактор"

вставьте код в начало из файла lovelace-template.yaml

### Добавление карточки
добавьте карточку, минимальныя конфигурация:
```
type: custom:button-card
entity: sensor.s20_5_ik_month_energy
template: meter_template
```
с параметрами:
```
type: custom:button-card
entity: sensor.s20_5_ik_month_energy
template: meter_template
styles:
  card:
    - "--card-width": 80px
    - "--card-height": 60px
  custom_fields:
    meter:
      - "--meter-font-size": 20px
      - "--meter-padding": 6px 7px
      - "--meter-width": 16px
      - "--meter-height": 25px
```
с текстом:
```
type: custom:button-card
template: meter_template
entity: sensor.s20_5_ik_month_energy
title: Электроэнергия
variables:
  text1: Кухня
  text1_color: "#00ccff"
  text1_size: 18px
  text1_position: top
  text1_align: center
  text2: кВт⋅ч
  text2_color: "#ff8844"
  text2_size: 16px
  text2_position: bottom
  text2_align: right
styles:
  card:
    - padding: 6pt 6pt 6pt 6pt
  custom_fields:
    meter:
      - font-size: 24px
      - padding: 6px 8px
      - "--meter-width": 20px
      - "--meter-height": 30px
```


### Параметры, которые можно задавать:

любые стили, плюс:

--card-background — фоновый градиент или цвет карточки.

--card-border — рамка карточки.

--card-border-radius — радиус углов карточки.

--card-box-shadow — тень карточки.

--card-height — высота карточки.

--card-width — ширина карточки.

Для кастомного поля meter:

--meter-gap — расстояние между цифрами.

--meter-font-size — размер шрифта цифр.

--meter-color — цвет цифр.

--meter-padding — отступы внутри кастомного поля.

--meter-border-radius — радиус углов кастомного поля.

--meter-box-shadow — тень кастомного поля.

Для цифр:

--meter-background — фон цифры.

--meter-color — цвет цифры.

--meter-width — ширина цифры.

--meter-height — высота цифры.

--meter-margin — отступ между цифрами.

--meter-border — рамка цифры.

--meter-border-radius — радиус углов цифры.

Для точки:

--meter-dot-width — ширина точки.

--meter-dot-font-size — размер шрифта точки.

--meter-dot-color — цвет точки.

--meter-dot-background — фон точки.
