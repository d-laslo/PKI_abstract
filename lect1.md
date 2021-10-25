# Лекція 1
## 01-1: Загальне поняття про PKI

* Головна проблема СК: транспортування ключа (дану проблему розв'язано в АК)
* Головна проблема АК: автентифікація ключів (незахищена від атаки "людина по середині")
* Вводинмо новий атрибут для ключа "Довіра" шляхом формування **сертифіката відкритого** ключа

Керування сертифікатами зводиться до PKI

**PKI** --- набір засобів та сервісів, які використовуються для прив'язування ключів до їх власників і для надійного транспортування ключів між учасниками взаємодії 

**Задачі PKI:**
* розв'язання задачі автентифікації сутностей (entity) та автентифікації данних (data origh)
* цілісність даних
* конфеденційність

**Чого чекаємо від PKI:**
1. механізм всановлення довіри у заданій моделі довіри
2. механізм унікального іменування сутностей всередині системи
3. механізм розподілу та поширення інформації про коректність прив'язки ключів до сутностей

**Що дає PKI:**
1. сильна сертифікація
2. легкість у використанні для кінцевих користувачів
3. дешеві операції
4. захист від пробробки особистості
5. відстежуваність дій, як для систем авторизації та систем аудиту
6. керована стійкість для криптографічних операцій

**Що _НЕ_ дає PKI:**
1. не проводить авторизацію сутностей
2. не встановлює довіру сутностям (лише довіру до прив'язкуключів до сутностей)
3. не іменує суб'єкт (роздає імена лише для внутрішнього використання)
4. не робить систему безпечною
5. не виправляє поведінку людей

---

## 01-02: класифікація електронних підписів

**Електронний підпис (ЕП)**  --- підпис, що має електронну форму

**Цифровий підпис (ЦП)** --- підпис, що був одержаний в результаті певного математичного перетворення

Директива **1999/93/EC** (про урівняння в правах звичайних і електронних підписів) вносить наступні категорії ЕП:
1. ЕП -- дані в електроній формі, які приєднані або логічно пов'язані з іншими даними, як метод автентифікації
2. Розширений ЕП (РЕП): // Why not Rock? 
    * унікально пов'язаний із підписником
    * може ідентифікувати підписника
    * зроблений засобами, які підписувач повністю контролює
    * легко виявляємо будь-які зміни після підписання
3. РЕП + посилений сертифікат (youtube 16:15)
4. РЕП + посилений сертифікат + SSCD (Secure Signature Crection Device)
5. Посилений ЕП (ПЕП) (можна іти в суд)
6. ПЕП + акредитований видавець сертифікатів