Задачи на использование HashSet

Задача 1: Уникальные элементы.

Создайте HashSet, добавьте в него несколько элементов, и убедитесь, что в нем хранятся только уникальные элементы.

Задача 2: Поиск элемента.

Создайте HashSet чисел и проверьте, содержится ли определенное число в множестве.

Задача 3: Удаление элемента.

Создайте HashSet строк и удалите определенную строку из множества.

Задача 4: Объединение множеств.

Создайте два HashSet и объедините их в одно множество.

Задача 5: Пересечение множеств.

Создайте два HashSet и найдите их пересечение (содержание общих элементов).

Задача 6: Определение подмножества.

Создайте два HashSet и проверьте, является ли одно из них подмножеством другого.

Задача 7: Очистка множества.

Создайте HashSet, добавьте элементы, и затем очистите его, удалив все элементы.

```
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> set = new HashSet<>();
        set.add("apple");
        set.add("banana");
        
        set.clear();
        
        System.out.println(set);
    }
}
```

Задача 8: Перевод в массив.

Создайте HashSet чисел и преобразуйте его в массив чисел.

```
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<Integer> numbers = new HashSet<>();
        numbers.add(5);
        numbers.add(10);
        numbers.add(15);
        
        Integer[] array = numbers.toArray(new Integer[0]);
        
        for (Integer number : array) {
            System.out.println(number);
        }
    }
}
```

Задача 9: Клонирование множества.

Создайте HashSet, добавьте элементы, и затем создайте его копию.

```
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> originalSet = new HashSet<>();
        originalSet.add("apple");
        originalSet.add("banana");
        
        HashSet<String> cloneSet = new HashSet<>(originalSet);
        
        System.out.println(cloneSet);
    }
}
```

Задача 10: Удаление элементов по условию.

Создайте HashSet чисел и удалите все числа, которые больше заданного значения.

```
import java.util.HashSet;
import java.util.Iterator;

public class Main {
    public static void main(String[] args) {
        HashSet<Integer> numbers = new HashSet<>();
        numbers.add(5);
        numbers.add(10);
        numbers.add(15);
        
        int maxValue = 10;
        
        Iterator<Integer> iterator = numbers.iterator();
        while (iterator.hasNext()) {
            int number = iterator.next();
            if (number > maxValue) {
                iterator.remove();
            }
        }
        
        System.out.println(numbers);
    }
}
```
