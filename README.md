# goit-js-hw-02

GOIT JS Homework 2 Задача 1. Замовлення дроїдів

Виконуй це завдання у файлі task-1.js

Станція з продажу ремонтних дроїдів готова до запуску, залишилося написати
програмне забезпечення для відділу продажів. Оголоси функцію makeTransaction,
яка очікує три параметри:

quantity — кількість замовлених дроїдів pricePerDroid — ціна одного дроїда
customerCredits — сума коштів на рахунку клієнта

Доповни функцію так:

Обчисли загальну суму замовлення (кількість дроїдів, помножена на ціну одного
дроїда). Перевір, чи клієнт може оплатити замовлення. Якщо сума до сплати
перевищує кількість кредитів на рахунку клієнта, функція повертає рядок
"Insufficient funds!". В іншому випадку функція повертає рядок: You ordered
<quantity> droids worth <totalPrice> credits!

де:

<quantity> — кількість замовлених дроїдів <totalPrice> — загальна вартість
замовлення Візьми код нижче і встав після оголошення своєї функції для перевірки
коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(makeTransaction(5, 3000, 23000)); // "You ordered 5 droids worth
15000 credits!" console.log(makeTransaction(3, 1000, 15000)); // "You ordered 3
droids worth 3000 credits!" console.log(makeTransaction(10, 5000, 8000)); //
"Insufficient funds!" console.log(makeTransaction(8, 2000, 10000)); //
"Insufficient funds!" console.log(makeTransaction(10, 500, 5000)); // "You
ordered 10 droids worth 5000 credits!"

Оголоси функцію formatMessage, яка очікує два параметри:

message — рядок повідомлення maxLength — максимальна довжина рядка

Доповни функцію так:

Якщо довжина message дорівнює або менша за maxLength, функція повертає
початковий рядок без змін. Якщо довжина перевищує maxLength, функція обрізає
рядок до maxLength символів і додає трикрапку "..." в кінці.

Візьми код нижче і встав після оголошення своєї функції для перевірки
коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(formatMessage("Curabitur ligula sapien", 16)); // "Curabitur
ligula..." console.log(formatMessage("Curabitur ligula sapien", 23)); //
"Curabitur ligula sapien" console.log(formatMessage("Vestibulum facilisis purus
nec", 20)); // "Vestibulum facilisis..." console.log(formatMessage("Vestibulum
facilisis purus nec", 30)); // "Vestibulum facilisis purus nec"
console.log(formatMessage("Nunc sed turpis a felis in nunc fringilla", 15)); //
"Nunc sed turpis..." console.log(formatMessage("Nunc sed turpis a felis in nunc
fringilla", 41)); // "Nunc sed turpis a felis in nunc fringilla"

Функція checkForSpam очікує один параметр message — рядок повідомлення. Слова в
рядку можуть бути в довільному регістрі, наприклад SPAM або sAlE.

Доповни функцію так:

Якщо в message знайдено заборонене слово spam або sale, функція повертає логічне
значення true. Якщо заборонених слів немає, функція повертає логічне значення
false.

Візьми код нижче і встав після оголошення своєї функції для перевірки
коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(checkForSpam("Latest technology news")); // false
console.log(checkForSpam("JavaScript weekly newsletter")); // false
console.log(checkForSpam("Get best sale offers now!")); // true
console.log(checkForSpam("Amazing SalE, only tonight!")); // true
console.log(checkForSpam("Trust me, this is not a spam message")); // true
console.log(checkForSpam("Get rid of sPaM emails. Our book in on sale!")); //
true console.log(checkForSpam("[SPAM] How to earn fast money?")); // true

Оголоси функцію getShippingCost, яка очікує один параметр country — країну
доставки. Обов'язково використай інструкцію switch.

Функція повертає рядок:

Shipping to <country> will cost <price> credits

де <country> і <price> — країна та вартість доставки з таблиці нижче.

Список країн і вартість доставки:

China — 100 кредитів Chile — 250 кредитів Australia — 170 кредитів Jamaica — 120
кредитів

Якщо зазначеної країни немає у списку, функція повертає рядок "Sorry, there is
no delivery to your country".

Візьми код нижче і встав після оголошення своєї функції для перевірки
коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(getShippingCost("Australia")); // "Shipping to Australia will cost
170 credits" console.log(getShippingCost("Germany")); // "Sorry, there is no
delivery to your country" console.log(getShippingCost("China")); // "Shipping to
China will cost 100 credits" console.log(getShippingCost("Chile")); // "Shipping
to Chile will cost 250 credits" console.log(getShippingCost("Jamaica")); //
"Shipping to Jamaica will cost 120 credits"
console.log(getShippingCost("Sweden")); // "Sorry, there is no delivery to your
country"
