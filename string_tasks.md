Примеры простых задач на строки

Задача 1: Перевернуть строку.

Запросите у пользователя ввод строки и выведите ее в обратном порядке.

```
import java.util.Scanner;

public class ReverseString {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введите строку: ");
        String input = scanner.nextLine();
        String reversed = new StringBuilder(input).reverse().toString();
        System.out.println("Перевернутая строка: " + reversed);
    }
}
```

Задача 2: Подсчитать количество слов.

Пользователь вводит строку. Подсчитайте и выведите количество слов в этой строке.

```
import java.util.Scanner;

public class WordCount {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введите строку: ");
        String input = scanner.nextLine();
        String[] words = input.split("\\s+");
        int wordCount = words.length;
        System.out.println("Количество слов в строке: " + wordCount);
    }
}
```

Задача 3: Заменить подстроку.

Замените все вхождения подстроки в строке другой подстрокой.

```
public class ReplaceSubstring {
    public static void main(String[] args) {
        String original = "Это пример текста с подстрокой, которую нужно заменить.";
        String replaced = original.replace("подстрока", "новая подстрока");
        System.out.println(replaced);
    }
}
```

Задача 4: Проверить наличие подстроки.

Проверьте, содержит ли строка заданную подстроку.

```
public class ContainsSubstring {
    public static void main(String[] args) {
        String text = "Это строка, которую нужно проверить.";
        String substring = "строка";
        if (text.contains(substring)) {
            System.out.println("Строка содержит подстроку.");
        } else {
            System.out.println("Строка не содержит подстроку.");
        }
    }
}
```

Задача 5: Извлечь подстроку.

Извлеките подстроку из строки по заданным индексам.

```
public class ExtractSubstring {
    public static void main(String[] args) {
        String text = "Это пример строки для извлечения подстроки.";
        int startIndex = 10;
        int endIndex = 26;
        String substring = text.substring(startIndex, endIndex);
        System.out.println(substring);
    }
}
```

Задача 6: Преобразовать регистр.

Преобразуйте строку в верхний или нижний регистр.

```
public class ChangeCase {
    public static void main(String[] args) {
        String text = "Этот текст нужно преобразовать в верхний регистр.";
        String upperCase = text.toUpperCase();
        String lowerCase = text.toLowerCase();
        System.out.println("Верхний регистр: " + upperCase);
        System.out.println("Нижний регистр: " + lowerCase);
    }
}
```

Задача 7: Проверить палиндром.

Проверьте, является ли строка палиндромом (читается одинаково в обоих направлениях).

```
public class IsPalindrome {
    public static void main(String[] args) {
        String text = "ротор";
        String reversed = new StringBuilder(text).reverse().toString();
        if (text.equals(reversed)) {
            System.out.println("Строка является палиндромом.");
        } else {
            System.out.println("Строка не является палиндромом.");
        }
    }
}
```

Задача 8: Удалить пробелы.

Удалите все пробелы из строки.

```
public class RemoveSpaces {
    public static void main(String[] args) {
        String text = "Это строка с пробелами.";
        String noSpaces = text.replace(" ", "");
    }
}
```

Задача 1: Объединение строк.

Создайте две строки, а затем объедините их в одну строку.

```
String str1 = "Привет, ";
String str2 = "мир!";
String result = str1 + str2;
System.out.println(result);
```

Задача 6: Разделение строки на подстроки.

Разделите строку на подстроки на основе определенного разделителя (например, запятой).

```
String исходнаяСтрока = "яблоко,груша,апельсин";
String[] подстроки = исходнаяСтрока.split(",");
for (String подстрока : подстроки) {
    System.out.println(подстрока);
}
```

Задача 9: Обрезка строки.

Обрежьте строку так, чтобы она не превышала определенную длину, и, если обрезана, добавьте многоточие в конец.

```
String исходнаяСтрока = "Это очень длинная строка, которую нужно обрезать.";
int максимальнаяДлина = 20;
if (исходнаяСтрока.length() > максимальнаяДлина) {
    String обрезаннаяСтрока = исходнаяСтрока.substring(0, максимальнаяДлина) + "...";
    System.out.println(обрезаннаяСтрока);
} else {
    System.out.println(исходнаяСтрока);
}
```
