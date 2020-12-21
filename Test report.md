Краткое описание
=================
Проверить работу банковского приложения, при пополнении счета клиента  

Дата начала: 21.12.2020  
Дата окончания: 21.12.2020  
На тестирование затрачено: 30 минут  

В результате тестирования выявлены следующие дефекты:  
  • Итоговая сумма считается неверно <https://github.com/rahel81/Java-task2.1/issues/1>

Описание процесса тестирования:
------------------
#### В процессе тестирования использовались следующие артефакты:  
  • Программа IntelliJ IDEA  
  • Код 
  ``` java
Public class Main {
   public  static  void  main ( String [] args ) {
               int balance =  2_000_000_000 ;
        int transfer =  500_000_000 ;
        int total = balance + transfer;
        System.out.println(total);
    }
  }
  ```
  Входные данные:  
    •	текущий баланс счёта клиента - 2_000_000_000 (два миллиарда рублей)  
    •	сумма перевода - 500_000_000 (пятьсот миллионов рублей)  

### Ожидаемый результат тестирования:  
Баланс счета пополнится на 500_000_000 (пятьсот миллионов рублей) и    
составит 2_500_000_000 (два миллиарда пятьсот миллионов рублей)

### Фактический результат тестирования:  
"C: \ Program Files \ AdoptOpenJDK \ jdk-11.0.9.101-hotspot \ bin \ java.exe" -javaagent: C: \ Users \ user \ AppData \ Local \ JetBrains \ Toolbox \ apps \ IDEA-C \ ch-0 \ 203.5981.155 \ lib \ idea_rt.jar = 52532: C: \ Users \ user \ AppData \ Local \ JetBrains \ Toolbox \ apps \ IDEA-C \ ch-0 \ 203.5981.155 \ bin -Dfile.encoding = UTF- 8 -classpath "C: \ Users \ user \ Desktop \ Тесты \ JAVA \ Task 2 \ Task 2.1 \ out \ production \ src" Main
-1794967296

#### Тестирование производилось в следующем окружении:  
• Windows 7 Professional, x64  
• версия Java 11.0.9.1  
• браузер Google Chrome версия 87.0.4280.88 (Официальная сборка), (64 бит)
