# Boolean Algebra

## Objective

The objective of this activity is to apply Boolean algebra rules to simplify logical expressions.

## Flowchart

<img width="235" height="597" alt="image" src="https://github.com/user-attachments/assets/8d853fa8-8d52-4cd5-bb33-ea38da832250" />


## Question 1

Simplify the Boolean expression:

```text
F = A'B'C' + A'B'C + A'BC + AB'C + ABC'
```

## Step-by-Step Simplification

Original expression:

```text
F = A'B'C' + A'B'C + A'BC + AB'C + ABC'
```

First, group the first two terms:

```text
A'B'C' + A'B'C
```

Factor out the common part:

```text
A'B'(C' + C)
```

Since:

```text
C' + C = 1
```

then:

```text
A'B'(1) = A'B'
```

So now:

```text
F = A'B' + A'BC + AB'C + ABC'
```

Some minterms can be used more than once during simplification. This helps create more grouping opportunities.

Use the minterm `A'B'C` again to group with `A'BC`:

```text
A'B'C + A'BC
```

Factor out the common part:

```text
A'C(B' + B)
```

Since:

```text
B' + B = 1
```

then:

```text
A'C(1) = A'C
```

Use the minterm `A'B'C` again to group with `AB'C`:

```text
A'B'C + AB'C
```

Factor out the common part:

```text
B'C(A' + A)
```

Since:

```text
A' + A = 1
```

then:

```text
B'C(1) = B'C
```

The term:

```text
ABC'
```

cannot be simplified with the other terms, so it stays the same.

## Final Answer for Question 1

```text
F = A'B' + A'C + B'C + ABC'
```

## Question 2: Motion-Sensing Light System

Inputs:

```text
m = motion sensed
t = test mode
```

Output:

```text
i = illuminate lamp
```

The lamp should turn on if:

1. Motion is sensed and test mode is off.
2. Test mode is on and no motion is sensed.
3. Test mode is on and motion is sensed.

## Original Boolean Expression

Motion is sensed and test mode is off:

```text
mt'
```

Test mode is on and no motion is sensed:

```text
m't
```

Test mode is on and motion is sensed:

```text
mt
```

So the original Boolean expression is:

```text
i = mt' + m't + mt
```

## Step-by-Step Simplification

Original expression:

```text
i = mt' + m't + mt
```

Group `mt'` and `mt`:

```text
i = m(t' + t) + m't
```

Since:

```text
t' + t = 1
```

then:

```text
i = m(1) + m't
```

So:

```text
i = m + m't
```

Now simplify:

```text
i = m + m't
```

Use the Boolean algebra rule:

```text
x + x'y = x + y
```

In this problem:

```text
x = m
y = t
```

Therefore:

```text
i = m + t
```

## Final Answer for Question 2

```text
i = m + t
```

This means the lamp turns on if motion is sensed or if test mode is on.

## Challenges

The main challenge was carefully grouping the Boolean terms without changing the meaning of the expression. Another challenge was remembering which Boolean identity to use, especially rules like `A + A' = 1`. For the motion-sensing light system, the challenge was translating the English conditions into a Boolean expression before simplifying it.

## Final Answers

Question 1:

```text
F = A'B' + A'C + B'C + ABC'
```

Question 2:

```text
i = m + t
```
