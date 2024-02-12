# OOP Basics with Java questions

## Java ecosystem

- What is the JVM?
    Java Virtual machine, egy abstrack virtuális gép ami futtatja a java applicationöket lehetővé téve h bármilyen hardware-en wagy op rendszeren elfusson
    a bytekódot  gépi kódra fordítja az adot géphez
    memóriakezelés garbage collectior, töbszálú végrehajtás

- What does Java compilation mean?
    amikor a forráskódot bytecode-á alakítunk  compiller segítségével történik

- What is Java bytecode?
    egy köztes kód a forráskód és a machinecode közt, a jvm csinlja a forráskódból

- What is the difference between the JRE and the JDK?
    Java Runtime Environment: Library-k, JVM és más komponenesek amik a java programok futtatásához kell
    Java Development Kit:java programok létrehozásához debugolásához és fordításához szükséges dolgok

- What is the `Iterable` interface?
    lehetővé teszi h végigiteráljunk egy collection elemein advanced for looppal(for-each) van egy iteraror() abstrack methodja, ami egy iterator objectet ad vissza, 

- What is the `Collection` interface?
    a collections hierarchy rootja, minden specifikusabb collection ebből származik le, 
    a Java Collections Framework része(egy adag class és interface collectionök representálására és manipulálására)
    extendeli az iterator interface-t
    altipusok: Set, List Queue stb (a map NEM)
    methods: size(), contains, add, remove

- What is the `Map` interface?
    lehetővé teszi h kulcs-érték párokkal dolgozzunk, duplikált key-ek nem lehetnek
- Compare sets, lists, and queues in Java.
- Compare `ArrayList` and `LinkedList` in Java.
- Are sets sorted in Java?
- How would you implement a HashMap with the use of HashSet?


## Language features

- What control statements are available in Java?
    Decision making statements(if, if-else, switch,)
    Loops: while, do-while, for for-each
    Jump statements: break, continue

- Compare the different looping constructs in Java.
- Compare the different conditional constructs in Java.
- What is a `while` loop?
- How do you manually break out of a loop?
- What does the `var` keyword mean?
- What are _lambda expressions_? How are they used in Java development?


## Type system

- What are primitive types in Java? Give some examples.
    byte, int, long, float, double, char, boolean

- What is the difference between primitive types and reference types?
- What are the wrapper classes in Java?
    Olyan classok amik enkapszulálják/becsomagolják a primitíveket hogy objectként tudjuk kezelni azokat.
- Miért jó ez?
    oop principleökkel tudjuk őket kezelni(Inheritence, Polymorphism, methods) és sok feature van a nelyven ami csak objectumokat tud kezelni(pl: Collections, a java.util utility class-ai, stb)
- What is autoboxing/unboxing?
    lehetővé teszi h automatikusan convertáljunk primitívek és a wrapper classuk közt, cleanebbé és könnyebben olvashatóvá téve a kódot
    - Autoboxing: amikor a compiler váltja a primitívet a wrapper classává, akkor történik amikor paraméterkén primitívet adunk át egy olyan methodnak ami wrapper obj-jét várja annak a primitívnek
    - Unboxing: az autoboxing reverse-je, a compiler a wraper obj-et primitívvé alakítja, ammikor wrapper obj-et adunk át és a method a coresponsive primitívet várja

- What is a class in Java?
- What is an object in Java?
- What is a constructor?
- What is an `enum` in Java?
- Explain the difference between a class and an enum.
- Explain the difference between a class and a record.
- What are interfaces? Why should we use them?
- What is inheritance?
- Is multiple inheritance allowed in Java?
- What is a static class member?
- Can a static method use non-static members?
- What does the `final` keyword mean in Java?
- What does the `abstract` keyword mean in Java?
    Non-access modifier, classochoz és methodokhoz lehet használni(fieldhez nem)
    Abstract Method: Csak abstract classban lehet, methodnak nincs body-ja, a class subclassának kell implementálni
    Abstract class: nem lehet példányosítani, egy instance létrehozásához extendelni kell. tartalmazhat abstract és nem abstract methodokat is

- What is _overloading_ in Java?
    ugyanaz a methodnév, eltérő paraméterezés, compile-time polymorphism, a compile-olás alatt dől el h melyik methodot használja, nem kell leszármazni
- What is _overriding_ in Java?
    Run-time polymorphsm, amikor egy child class felülír egy megörökölt methodot (vagy implementál egy abstract methodot)
- What is the difference between overloading and overriding?
- What is `null`?
- Compare the access modifiers in Java.
- What is the default access modifier in a class?
- What is the purpose of the `equals()` method?
- What is the difference between `==` and `equals()`?
- What is the difference between `long` and `Long`?
- Which can store bigger numbers, `long` or `Long`?
- What kind of packages do you know under `java.util.*` ? Bring at least 3 examples.


## Architecture

- Explain the Single Responsibility Principle.
- Explain the Interface Segregation Principle.
- What is _composition over inheritance_?
- What is a model class?
- What is a service class?
- Explain the Open/Closed principle.
- Explain the Liskov Substitution Principle.
- Explain the Dependency Inversion Principle.
- What do we mean by the Gang of Four (GoF) Design Patterns? Can you name some of these patterns?
- What are the risks associated with using the GoF design patterns?
- What do we mean by YAGNI?
- What do we mean by SLAP?
- What do we mean by KISS?
- What is the Repository Pattern?
- What is a CRUD interface?


## Unit testing
- Why is unit testing a good practice?
- What is JUnit?
- What is a parameterized test?
- What options do you have in NUnit to create parameterized tests?
- What is _mocking_?
- What is the difference between _mocking_, _stubbing_ and _faking_?


## Databases

- What are relational databases? What are their advantages and disadvantages?
- How do you associate entities to each other in a relational database model?
- What are tables in a relational database?
- What is a _primary key_?
- What is a _foreign key_?
- What does the SQL abbreviation stand for?
- What are some of the SQL database providers that you’ve heard of?
- What are SQL data types? Are there any differences in data types between different SQL databases?
- What are _constraints_ in SQL?
- How can we program different SQL databases in Java? 
- Which SQL statement is used to create tables? Describe the syntax briefly.
- Which SQL statement can be used to insert values? Describe the syntax briefly.
- Which SQL statement can be used to update values? Describe the syntax briefly.
- Which SQL statement can be used to delete rows?. Describe the syntax briefly.
- Which SQL statement can be used to create queries?. Describe the syntax briefly.
- How can you join tables together in SQL? When should you do it?





