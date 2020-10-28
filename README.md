## Установка
### Heroku 
_Инструкцию ~~любезно~~ предоставил [Юн Дэмин](https://vk.com/id616052556)_

`<nick>` - ваш ник в гитхабе.<br>
`<name>` - имя репозитория.

1. Регистрируемся на [GitHub](https://github.com)
2. Создаем закрытый репозиторий
    ![](https://sun9-5.userapi.com/ZdunWUy0_UtICPscb8DDDXlKXrYpjY2GRHZK1Q/-tt19NoXdC4.jpg)
3. Заходим в термукс или гит на ПК и пишем следующие команды:
    ```shell script
    git clone --bare https://github.com/lordralinc/idm_lp.git
    cd idm_lp.git
    git push --mirror https://github.com/<nick>/<name>.git
    ```
    _Может появится просьба войти в аккаунт, вводим логин и пароль от аккаунта и все готово_
    ```shell script
    cd ..
    rm -rf idm_lp.git
    ```
4. Заходим на наш закрытый репозиторий и там где написано `2.0` изменяем на `master`.<br>
5. Далее заходим в `config.json`, вставляем токен от Kate Mobile и секретный код IDM.
6. Регистрируемся на [Heroku](https://heroku.com) и выбираем python.
7. Переходим по ссылке: [dashboard.heroku.com/apps](https://dashboard.heroku.com/apps) и создаем приложение. 
    Выбираем европу и название приложение любое, чтоб угодить хероку.
8. После создания мы окажемся в панели управления, нажимаем на GitHub и входим в аккаунт.
    ![](https://sun9-47.userapi.com/pLLeZCAo1P4sQR1brlFdBwHtfBWhBQGfuILR-g/edHTCYYZ2CE.jpg)
9. Нам нужно имя закрытого репозитория, вставляем и нажимаем `Search`, выбираем нужный нам репозиторий и нажимаем на `Connect`.
10. Листаем вниз и видим кнопку `Deploy Branch`, рядом с кнопкой будет `2.0`, нажимаем и выбираем `master`, далее тыкаем на кнопку `Deploy Branch` и ждем.
11. Вверху нажимаем на кнопку `Resources`.
12. Нажмаем на карандашик слева, включаем и тыкаем на `Confirm`.
13. Переходим обратно в `Deploy` и мотаем вниз делаем все как по пункту 10

### Windows
