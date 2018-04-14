<meta name="text" content="Use loops and conditions to create a painting application.">
<meta name="objective" content="create an application to draw on the window with the mouse">

---

# Painting

Create a class named `Painting` that has a `main` method, as shown on the right. Like the two previous labs, all the code you write will be in the `main` method.

This lab will build off the [painting animation in the previous lab](../animation/#_painting).

---

# If

> An <code>if</code> statement performs a block if a certain condition is true.

The condition must be a `true` or `false` (boolean) statement.

```java
int age = 15;

if (age >= 18) {
	System.out.println("You can vote.");
}
```

Multiple `if` statements can be written one after another.

```java
int age = 20;

if (age >= 16) {
	System.out.println("You can drive.");
}
if (age >= 18) {
	System.out.println("You can vote.");
}
if (age >= 25) {
	System.out.println("You can rent a car.");
}
```


---

# Paint Color

> Change the paint color based on the mouse's x position.

For example, draw in one color for one half of the window, and in another color for the other half. **Can you think of other ways to use `if` statements to create more sophisticated coloring schemes?**

---

# Booleans

> A boolean is a true or false value.

Since it is a **data type** (like `int`), we can [declare a variable](../animation/#_variables) that stores `boolean` values. Notice that you can only
store `true` or `false` in a `boolean` variable.

The condition of an `if` statement can be any boolean expression. In the example on the right, we used the value stored in a boolean to determine whether
a certain print instruction is performed.


---

# Mouse input

> The <code>Window.mouse.clicked</code> method returns <code>true</code> if the mouse is clicked.

---

# Click to paint

> Click on the window to draw a circle at the mouse position.

---

# Else

> An `else` statement performs a block if the condition of the previous if statement is false.

---

# Nested if

> Branching statements can be placed in any block.

---

# Key presses

> The <code>Window.key.pressed</code> method returns <code>true</code> if the given key is pressed.

---

# Else if

> An `else if` statement checks its condition if the conditions of the previous `if` and `else if` statements are false.
