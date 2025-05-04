# Домашнее задание 

Получение и отображение категорий товаров

- Создать компонент <categoryList>
при загруске компонент должен получить данные из этого апи
https://dummyjson.com/docs/products#products-category_list
и вывести их списком

- для начала данные можно сохранить в "мок" файлик и вывести их от туда 
```
[
  "beauty",
  "fragrances",
  "furniture",
  "groceries",
  "home-decoration",
  "kitchen-accessories",
  "laptops",
  "mens-shirts",
  "mens-shoes",
  "mens-watches",
  "mobile-accessories",
  "motorcycle",
  "skin-care",
  "smartphones",
  "sports-accessories",
  "sunglasses",
  "tablets",
  "tops",
  "vehicle",
  "womens-bags",
  "womens-dresses",
  "womens-jewellery",
  "womens-shoes",
  "womens-watches"
]
```

- нам нужно использовать ХУК useState
для создания состояния
```
const [state, setState] = useState(initialState);
state         — текущее значение состояния.
setState      — функция, которая обновляет это значение.
initialState  — начальное значение состояния.
```
 ХУК useEffect запуск после рендера 
```
useEffect(() => {
  // эффект
  return () => {
    // очистка эффекта (опционально)
  };
}, [dependencies]);

Эффект выполняется после рендера.
Если передать [] в зависимости — эффект выполнится только один раз при маунте.
Если зависимости изменятся     — эффект будет перезапущен.
```


Так же мы можем добавить стейт loading 
и показывать экран загруски пока ждем данные с апи
