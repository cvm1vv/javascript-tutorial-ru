importance: 4

---

# Подсказка, следующая за курсором

Создайте всплывающую подсказку, следующую за курсором.

- Подсказка должна появляться при наведении на элемент, на небольшом расстоянии справа-снизу от курсора.
- При передвижении курсора подсказка следует за ним.
- Если курсор слишком низко/справа, то чтобы подсказка не вылезла за нижнюю/правую границу экрана -- пусть отображается сверху/слева от курсора.

Вы можете посмотреть поведение подсказки в ифрейме ниже, наведя курсор на правый-нижний угол.

[iframe src="solution" height=200 link border=1]

Способ добавления подсказки к элементу:

```js
new Tooltip({
  elem: $('#elem'),
  html: "Вот <b>такая</b> подсказка!")
});
```

Естественные пожелания:

- Подсказка не должна "моргать" при движении мыши.
- Подсказка должна правильно работать, если у страницы есть прокрутка.
- В подсказке и элементе, на который она поставлена, может быть произвольный HTML. Оформление подсказки должно задаваться CSS.
- Объект подсказки не должен иметь публичных методов, только приватные.

