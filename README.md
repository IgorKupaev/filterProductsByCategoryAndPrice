# Условие задачи

Необходимо написать функцию `filterProductsByCategoryAndPrice`, которая будет принимать на вход массив объектов `products`, а также два аргумента: `category` (строка) и `priceRange` (массив из двух чисел - минимальная и максимальная цена).

Функция должна вернуть новый массив, содержащий объекты продуктов, которые относятся к указанной категории и имеют цену в указанном диапазоне (включительно).

Для каждого объекта продукта в результирующем массиве функция должна также вычислять средний рейтинг на основе всех отзывов. Результат должен содержать поле `averageRating` в каждом объекте продукта.

Пример вызова функции:
```javascript
const filteredProducts = filterProductsByCategoryAndPrice(products, 'электроника', [10000, 40000]);
console.log(filteredProducts);
```
Ожидаемый результат:

```javascript
[
  {
    name: "Ноутбук",
    price: 50000,
    category: "электроника",
    available: true,
    photo: "https://example.com/notebook.jpg",
    reviews: [
      { author: "Иван", text: "Отличный ноутбук!", rating: 5 },
      { author: "Петр", text: "Не очень...", rating: 2 },
      { author: "Мария", text: "Мне понравился", rating: 4 },
      { author: "Алексей", text: "Очень хороший ноутбук", rating: 5 }
    ],
    averageRating: 4.0
  },
  {
    name: "Телевизор",
    price: 30000,
    category: "электроника",
    available: true,
    photo: "https://example.com/tv.jpg",
    reviews: [
      { author: "Александра", text: "Отличный телевизор!", rating: 5 },
      { author: "Денис", text: "Неплохой выбор", rating: 3 },
      { author: "Сергей", text: "Хороший телевизор", rating: 4 },
      { author: "Наталья", text: "Классный телек", rating: 5 }
    ],
    averageRating: 4.25
  }
]

```
