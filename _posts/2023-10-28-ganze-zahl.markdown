---
layout: post
title:  "Ganze Zahlen"
date:   2023-10-28 10:28:36 +0530
categories: EPR
---

1. Write a code with integer numbers.

```java

package calculation;

/**
 * Prints values of Fahrenheit and time expressions.
 */
public class Calculations {
  /**
   * Prints both values.
   */

  public static void main(String[] args) {
    /*
     * Prints Fahrenheit.
     */

    System.out.println((5 * (40 - 32)) / 9);
    System.out.println((5 * (41 - 32)) / 9);

    /*
     * Prints time expressions.
     */
    System.out.println((5 / 60 * 100) + 5 % 60);
    System.out.println((59 / 60 * 100) + 59 % 60);
    System.out.println((60 / 60 * 100) + 60 % 60);
    System.out.println((61 / 60 * 100) + 61 % 60);
    System.out.println((825 / 60 * 100) + 825 % 60);
  }
}

```

2. Integer expressions in Java

How can you describe the last two numbers of 12498?
    
    12498 % 100
    
How can you describe the first two numbers of 12498?

    12498 / 1000
