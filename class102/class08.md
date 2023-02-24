# Operators And Loops

## Expressions

An expression is a valid unit of code that resolves to a value.

> Ex: x = 7 assigning the value 7 to x.

## Assignment Operators

Assigns a value to its left **operand** based on the value of its right **operand**.

> Note: An operand is the part of an instruction representing the data manipulated by the operator. For example, when you add two numbers, the numbers are the operand and "+" is the operator.

## Comparison Operators

A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values.

## Loops

Loops offer a quick and easy way to do something repeatedly. There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times.

## for Statement

A **for** loop repeats until a specified condition evaluates to false.

> Ex: for (initialization; condition; afterthought)
statement.

When a **for** loop executes, the following occurs:

1. *Initialization*, if any, is executed. This expression can also declare variables.
2. The *condition* expression is evaluated. If the value of condition is true, the loop statements execute. Otherwise, the for loop terminates.
3. The *statement* executes.
4. If present, the update expression *afterthought* is executed.
5. Control returns to Step 2.

## do..while Statement

Repeats until a specified condition evaluates to false.

- **statement** is always executed once before the condition is checked.
- If condition is true, the statement executes again. At the end of every execution, the condition is checked. When the condition is false, execution stops, and control passes to the statement following "do...while".

> Ex: do statement while (condition);

> Ex: let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);

## while Statement

A **while** statement executes its statements as long as a specified condition evaluates to true.

> while (condition) statement

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.