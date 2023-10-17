Задача 1: Сортировка чисел.

Создайте ArrayList чисел и отсортируйте его в порядке возрастания.

```
import java.util.ArrayList;
import java.util.Collections;

public class Main {
    public static void main(String[] args) {
        ArrayList<Integer> numbers = new ArrayList<>();
        numbers.add(5);
        numbers.add(2);
        numbers.add(9);
        numbers.add(1);
        
        Collections.sort(numbers);
        
        System.out.println(numbers);
    }
}
```

Задача 2: Удаление дубликатов.

Удалите все дубликаты из ArrayList строк.

```
import java.util.ArrayList;
import java.util.HashSet;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        ArrayList<String> strings = new ArrayList<>();
        strings.add("apple");
        strings.add("banana");
        strings.add("apple");
        strings.add("cherry");
        
        List<String> uniqueStrings = new ArrayList<>(new HashSet<>(strings));
        
        System.out.println(uniqueStrings);
    }
}
```

Задача 3: Поиск элемента.

Создайте ArrayList и найдите индекс первого вхождения определенного элемента в списке.

```
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) {
        ArrayList<String> names = new ArrayList<>();
        names.add("Alice");
        names.add("Bob");
        names.add("Charlie");
        
        String targetName = "Bob";
        int index = names.indexOf(targetName);
        
        if (index != -1) {
            System.out.println(targetName + " found at index " + index);
        } else {
            System.out.println(targetName + " not found in the list.");
        }
    }
}
```

Задача 4: Объединение списков.

Объедините два ArrayList в один.

```
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        ArrayList<String> list1 = new ArrayList<>();
        list1.add("apple");
        list1.add("banana");
        
        ArrayList<String> list2 = new ArrayList<>();
        list2.add("cherry");
        list2.add("date");
        
        list1.addAll(list2);
        
        System.out.println(list1);
    }
}
```

Задача 5: Оценки студентов.

Создайте список оценок студентов (целых чисел) и вычислите средний балл.

```
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) {
        ArrayList<Integer> grades = new ArrayList<>();
        grades.add(85);
        grades.add(92);
        grades.add(78);
        
        int total = 0;
        for (int grade : grades) {
            total += grade;
        }
        
        double average = (double) total / grades.size();
        
        System.out.println("Average grade: " + average);
    }
}
```

Задача 6: Фильтрация списка.

Создайте список строк и удалите все строки, которые начинаются с определенной буквы.

Задача 7: Определение максимума и минимума.

Найдите максимальное и минимальное значения в ArrayList чисел.

Задача 8: Перемешивание списка.

Перемешайте элементы в ArrayList случайным образом.

Задача 9: Обратный порядок.

Инвертируйте порядок элементов в ArrayList.

Задача 10: Разделение списка.

Разделите ArrayList на два списка: один с четными числами, другой с нечетными числами.