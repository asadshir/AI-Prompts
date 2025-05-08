graph TD;
    A[شروع] --> B(عملیات ۱);
    B --> C{شرط};
    C -->|بله| D[پایان];
    C -->|خیر| B;

graph LR;
    A --> B --> C;

graph TB;
    A --> B --> C;

classDiagram
    class Person {
        -name: String
        +getName(): String
    }
    class Student {
        -id: Int
        +getID(): Int
    }
    Person <|-- Student

gantt
    title نمودار گانت نمونه
    dateFormat  YYYY-MM-DD
    section بخش ۱
    تسک ۱           :a1, 2023-01-01, 30d
    تسک ۲           :after a1, 20d
    section بخش ۲
    تسک ۳           :2023-02-01, 12d
    تسک ۴           :24d



sequenceDiagram
    Alice->>Bob: سلام!
    Bob-->>Alice: سلام چطوری؟
    Alice->>Bob: خوبم!


stateDiagram-v2
    [*] --> حالت۱
    حالت۱ --> حالت۲: رویداد
    حالت۲ --> [*]

pie
    title توزیع داده‌ها
    "بخش ۱" : 40
    "بخش ۲" : 25
    "بخش ۳" : 35

