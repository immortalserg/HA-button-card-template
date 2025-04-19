# HA-button-card-template
![Image alt](20241618.png)

минимальныя конфигурация:
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
### Параметры, которые можно задавать:

--card-padding — отступы для всей карточки.

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
