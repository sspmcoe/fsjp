# Final Practical: Program 1 to 6

* **Programs 1–3:** Save each program with its class filename (e.g., `Student.java`, `Demo.java`, `B.java`), compile using `javac`, and run using `java`.
* **Programs 4–6:** Save each program in a separate `.html` file (e.g., `program4.html`) and open it in a web browser.

---

## Program 1: Classes and Objects in Java
**Aim:** To create a class and object in Java.

```java
class Student {
    void display() {
        System.out.println("Hello Student");
    }

    public static void main(String[] args) {
        Student s = new Student();
        s.display();
    }
}
```

---

## Program 2: Method and Constructor Overloading in Java
**Aim:** To demonstrate method and constructor overloading.

```java
class Demo {
    Demo() {
        System.out.println("Default Constructor");
    }

    Demo(int a) {
        System.out.println(a);
    }

    void show(int a) {
        System.out.println(a);
    }

    void show(String s) {
        System.out.println(s);
    }

    public static void main(String[] args) {
        Demo d = new Demo();
        Demo d2 = new Demo(10);
        d.show(5);
        d.show("Hello");
    }
}
```

---

## Program 3: Inheritance and Exception Handling in Java
**Aim:** To demonstrate single inheritance and exception handling.

```java
class A {
    void display() {
        System.out.println("Parent Class");
    }
}

class B extends A {
    public static void main(String[] args) {
        B obj = new B();
        obj.display();
        try {
            int x = 10 / 0;
        } catch (ArithmeticException e) {
            System.out.println("Error Handled");
        }
    }
}
```

---

## Program 4: Create a Website Using HTML, CSS and JavaScript
**Aim:** To create a simple website using HTML, CSS and JavaScript.

```html
<!DOCTYPE html>
<html>
<head>
<title>My Website</title>
<style>
body {
    text-align: center;
    font-family: Arial;
}
h1 {
    color: blue;
}
</style>
</head>
<body>
<h1>My Website</h1>
<button onclick="show()">Click Me</button>
<script>
function show() {
    alert("Welcome to My Website");
}
</script>
</body>
</html>
```

---

## Program 5: Email Validation Using JavaScript
**Aim:** To validate an email address by checking the presence of `@` and `.`

```html
<!DOCTYPE html>
<html>
<body>
<h2>Email Validation</h2>
<input type="text" id="email" placeholder="Enter Email">
<button onclick="checkEmail()">Submit</button>
<script>
function checkEmail() {
    let e = document.getElementById("email").value;
    if (e.includes("@") && e.includes(".")) {
        alert("Email Accepted");
    } else {
        alert("Invalid Email. Enter Again");
    }
}
</script>
</body>
</html>
```

---

## Program 6: Change Background Color Every 5 Seconds Using DOM
**Aim:** To change the background color of a web page automatically every 5 seconds.

```html
<!DOCTYPE html>
<html>
<body>
<h2>Background Color Change</h2>
<script>
let colors = ["red", "blue", "green", "yellow"];
let i = 0;
setInterval(function() {
    document.body.style.backgroundColor = colors[i];
    i = (i + 1) % colors.length;
}, 5000);
</script>
</body>
</html>
```
