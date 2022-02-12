# project_group_2-front

## Tasks

| Компоненты             | Задачи                                                                                         |
| ---------------------- | ---------------------------------------------------------------------------------------------- |
| RegistrationForm [^1]. | [^1]: Верстка мобилка, планшет, десктоп                                                        |
|                        | Провалидировать поля формы, использовать: 1) библиотеку formik и yup или 2) indicative.        |
|                        | Пароль и емейл обязательные поля, емейл проверить на валидность, пароль 6 и более до 12        |
|                        | включительно символов, пароли должны совпадать, имя минимум 1 символ, максимум 12              |
|                        | включительно                                                                                   |
|                        | Классовый или хук компонент, хранящий в своем стейте состояние инпутов                         |
|                        | Написать операцию на регистрацию, она должна срабатывать на сабмит формы                       |
|                        | Если ответ от сервера успешен то в ответ вы получите токен и объект юзера.                     |
|                        | Запишите токен и объект юзера в redux store, а также изменить ключ в session.isAuth на true    |
|                        | Если в ответ от сервера приходит ошибка, ее нужно определить в redux store session.error и     |
|                        | предусмотреть отрисовку данной ошибки                                                          |
|                        | Ссылка "Войти" это компонент Link из react-router-dom и переход на "/login"                    |
| `RegistrationPage`     | Верстка мобилка, планшет, десктоп                                                              |
|                        | Обеспечиваешь нужное позиционирование элементов на странице                                    |
|                        | Принимает в себя компонент RegistrationForm                                                    |
|                        | Обернуть страницу в HOC withAuthRedirect                                                       |
| `LoginForm`            | Верстка мобилка, планшет, десктоп                                                              |
|                        | Провалидировать поля формы, использовать: 1) библиотеку formik и yup или 2) indicative.        |
|                        | Пароль и емейл обязательные поля, емейл проверить на валидность, пароль 6 и более до           |
|                        | 12 включительно символов                                                                       |
|                        | Классовый или хук компонент, хранящий в своем стейте состояние инпутов                         |
|                        | Написать операцию на логинизацию, она должна срабатывать на сабмит формы                       |
|                        | Если ответ от сервера успешен то в ответ вы получите токен и объект юзера. Запишите токен и    |
|                        | объект юзера в redux store, а также изменить ключ в session.isAuth на true                     |
|                        | Если в ответ от сервера приходит ошибка, ее нужно определить в redux store session.error и     |
|                        | предусмотреть отрисовку данной ошибки                                                          |
|                        | Ссылка "Регистрация" это компонент Link из react-router-dom и переход на "/register"           |
| `LoginPage`            | Верстка мобилка, планшет, десктоп                                                              |
|                        | Обеспечиваешь нужное позиционирование элементов на странице                                    |
|                        | Принимает в себя компонент LoginForm                                                           |
|                        | Обернуть страницу в HOC withAuthRedirect                                                       |
| `DashboardPage`        | По верстке тут расположение всех дочерних элементов согласно макету                            |
|                        | Подключить все дочерние компоненты и реализовать логику их рендера в зависимости от разрешения |
|                        | экрана. Для этого подойдет библиотека react-media                                              |
|                        | Написать операцию которая забирает данные по транзакциям                                       |
|                        | Написать операцию которая забирает состояние баланса                                           |
|                        | В дидмаунте компонента запускать операции из пункта 2 и 3                                      |
