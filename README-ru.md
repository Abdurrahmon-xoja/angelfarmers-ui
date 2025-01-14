## F12+ комплект инструментов для игроков в FarmersWorld.io от Гильдии AngelFarmers
> Играй профессионально.
> Добывай ресурсы и учавствуй в строительстве Метавселенной.
> Участвуй в гильдии фармеров АнгелФармеры, повышай свой уровень игры, получи финансирование для построения доходных ферм

![Снимок экрана 2022-03-02 в 21 02 47](https://user-images.githubusercontent.com/6615/156410931-bcb73461-9983-471f-9d1d-ed6ae6b3a946.png)

F12+ - дапп, веб-приложение с открытыми исходными кодами для помощи игрокам FarmersWorld.io в фарминге ресурсов и торговле на Атомик и Алькор рынках.

https://fw.angelfarmers.com - официальная версия для участников Гильдии AngelFamers.


### Обзор возможностей:
1. Расчет текущей стоимости фермы и отдельных ее активов
2. Оценка доходности с разбивкой и оценкой ROI - окупаемости
3. Автоматизация рутинных операций - сбор, починка, восстановление энергии, кормление животных и тд.
4. Удобные интерфейсы для управление фермой - вводы/вывод токенов, обмен токенов на Алькор, Крафт и покупка на игровом рынке, перевод токенов и NFT между фермами, обмен и продажа урожая, продажа NFT на Атомик и т.д.
5. Управление несколькими фермами с одного окна, с помощью одного аккаунта. Расчет общей стоимости и доходности всех ферм.
6. Безопасное управление фермими с приватными ключами без использования WAX Cloud Wallet
7. Мониторинг состояния ферм через Телеграм бот. 
8. Анализ цен и торговля на Атомик рынке.
9. Анализ стакана и торговля на Алькор рынке
10. something something 


### Гильдия АнгелФармеров (AngelFarmers)
Мы игровая гильдия, инвесторов и игроков в игру [FarmwersWorld.io](https://farmersworld.io) на блокчейне WAX. 

Наша цель - поддержка участников Гильдии с помощью инструментов, обучения и финансирования.
Для сбора средств в общий инвестиционный пул у нас есть инвестиционный токен AWAX. 

AWAX или Ангел WAX это сберегательный/инвестиционный токен гильдии с правами получения дивидендов и голосования по вопросам Гильдии.

AWAX это нативный токен на блокчейне WAX. AWAX торгуется на бирже Алькор и может быть также приобретен на предпродаже через смарт-контракт awaxpresales или через https://fw.angelfarmers.io

Новости в Телеграм - https://t.me/angelfarmers_news_ru
Сервер на Дискорд - https://discord.gg/xd8YZQbu

[Алькор Обмен WAX/AWAX](https://wax.alcor.exchange/swap?output=WAX-eosio.token&input=AWAX-awaxdaotoken)

[Алькор Торговля WAX/AWAX](https://wax.alcor.exchange/trade/awax-awaxdaotoken_wax-eosio.token)

Каждый участник гильдии обязуется инвестировать 5% от дохода полученного с помощью F12+ инстументария в токен AWAX, что открывает следующие возможности:
1. Предлагать новые функции и определять направление разработки F12+ инструментов
2. Голосовать по вопросам Гильдии и разработки инструментов
3. Получать айрдропы с NFTs и токенами, полученными от вложения WAX токенов собранных на продаже AWAX
4. Получать дивиденды от Инвестиционного Фонда Гильдии
5. Получать в управление средства из Инвестиционного Фонда Гильдии


### Telegram bot
https://t.me/angelfarmers_bot 

телеграм бот-компаньон связан с F12+ с помощью базы данных и может следующее:
1. оповещать о транзакциях переводов токенов и NFT на указанных аккаунтах (мониторинг аккантов)
2. показывать текущее состояние ферм
3. оповещать когда наступит час льготного вывода токенов из игры (5%)
4. оповещать если авто управление фермой с помощью F12+ перестало откликаться и есть вероятность пропустить действия

Команды:
- **add имяфермы** - добавляет ферму для мониторинга 
- **delete имяфермы** - убирает ферму из списка 
- **farms** - список ферм 
- **on** - включить режим уведомления 
- **off** - выключить режим уведомления 
- **5%** - уведомить когда будет 5% (делает только один раз) 
- **status** - состояние ваших ферм (там видно работает ли бот и как давно он "отмечался") в режиме -'on' - должны приходить уведомления если бот на ферме не "отмечался" больше 10 минут. Бот (клиент в браузере) когда обслуживает ферму каждые 60 секунд сохраняет состояние в базе, по этому обновлению телеграм бот знает как давно было обслуживание и не выключился ли бот
----
### Запуск
#### Настройка проекта
```
npm install
```

#### Компиляция и запуск проекта локально
```
npm run serve
```

### Компиляция и минификация проекта для публикации
```
npm run build
```

### Настройки ключей:
Для полноценной работы приложения ему необходимо дать доступ к базе данных на Firebase. Firebase это облачный сервис от Google, где можно получить бесплатную (для небольших проектов) базу данных Firestore Database.

Необоходимо создать такой проект здесь - https://console.firebase.google.com. И указать данные конфигурации в файле .keys.js в корневой папке проекта. 

Вот пример как должен выглядеть файл .keys.js

```
export const FB_APIKEY="..."
export const FB_authDomain="..."
export const FB_projectId="..."
export const FB_storageBucket="..."
export const FB_messagingSenderId="..."
export const FB_appId="..."
export const FB_measurementId="..."
```
