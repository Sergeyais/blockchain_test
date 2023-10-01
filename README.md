Этот файл Readme предназначен для описания кода, представленного выше. Код реализует простой блокчейн с использованием JavaScript. Ниже представлено краткое описание классов и методов в коде.

## Класс Block

Класс `Block` представляет собой основную единицу данных в блокчейне. Он имеет следующие атрибуты:

- **timestamp (Временная метка блока)**: Передается при создании блока и представляет временную метку момента создания блока.
- **data (Данные блока)**: Это массив данных, который можно добавлять к блоку.
- **hash (Хеш блока)**: Этот хеш вычисляется на основе предыдущего хеша, временной метки и данных блока.
- **prevhash (Хеш предыдущего блока)**: Этот атрибут содержит хеш предыдущего блока в цепочке.

## Класс Blockchain

Класс `Blockchain` представляет собой цепочку блоков. Он имеет следующие методы:

- **constructor()**: Создает начальный блок в цепочке с текущей временной меткой.
- **getLastBlock()**: Возвращает последний блок в цепочке.
- **addBlock(block)**: Добавляет новый блок в цепочку. Вычисляет хеш для нового блока, устанавливает хеш предыдущего блока и добавляет его в цепочку.
- **isValid(blockchain)**: Проверяет целостность цепочки блоков. Проверяет, что хеши блоков соответствуют ожидаемым значениям и цепочка действительна.
