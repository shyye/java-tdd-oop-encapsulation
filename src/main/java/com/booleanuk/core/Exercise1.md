# Exercise 1
Class diagrams created with different tools.

## Gleek_
https://gleek.io/

Image:  
![](/assets/exercises/Exercise1_gleek.png)

Code:  
```
Bank
	- balance = 620.14

	+ deposit(date, amount) boolean
	+ withdraw(date, amount) boolean
	+ generateStatementPDF() Pdf
	
Diary
	- owner = "John Smith"
	
	+ lock() void
	+ unlock() void
	+ addEntry(entry) boolean
	+ getEntries() ArrayList<Entry>
	
Calculator
	+ add(num1, num2) int
	+ subtract(num1, num2) int
	+ print(message) String
```

## Mermaid
https://mermaid.js.org/intro/getting-started.html

Image:  
![](/assets/exercises/Exercise1_mermaid.png)

Code:  
```
classDiagram
    class Bank{
        -String balance = 620.14

        +boolean deposit(date, amount) 
        +boolean withdraw(date, amount) 
        +Pdf generateStatementPDF() 
    }

    class Diary {
        -Person owner = "John Smith"
	
        +void lock()
        +void unlock()
        +boolean addEntry(entry)
        +ArrayList getEntries()
    }

    class Calculator {
       	+int add(num1, num2) 
        +int subtract(num1, num2) 
        +String print(message) String 
    }
```