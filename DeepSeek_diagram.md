[سایت مرجع مرمید](https://mermaid.js.org/)
---
[نمونه ها](https://mermaid.js.org/syntax/examples.html)
---
[آزمایشگاه دیاگرام](https://mermaid.live/edit#pako:eNp1jUtOwzAQhq9izQqktMqzSb1Aoi2cgBVJF1bjPkSTVCYRjyQLpKbqIvcAdUFUHgs2nMMml8FtqNjASJZmPN__TQqjyKeAYTyPbkZTwmJ0MfBCJOvU5R91ySskVmLNt_K9DFGrdZLxim_l4lE88A1qmLrMUO-IP-8X1XEj6O1o1E_5hr-Loi5FgQ5E3hD9xvfziaRyLZYZGrhiKT6RzD3yp-HfaCXRIkNn7pfs-Ftd_sO9Nty5OyZ4TFojwpAopFcmxGoICkzYzAccs4QqEFAWkN0I6c7mQTylAfUAy9Yn7MoDL8xlZkHCyygKDjEWJZMpSP38Wk7JwicxHczIhJFfhIY-Zf0oCWPA1t4AOIVbwLrhtB3TMU1N1TRVNzu6AneAu1a7Y3Rt3bBN3coVuN_fU9u245hdTbVV3VYtw9Hzb_uQu2Y)
---

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

