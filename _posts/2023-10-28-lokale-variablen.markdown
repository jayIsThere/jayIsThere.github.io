---
layout: post
title:  "Lokale Variablen"
date:   2023-10-28 10:28:32 +0530
categories: EPR
---

1. Write a code for charging.

```java

package charging;

/**
 * Print charging.
 */
public class Charging {

  /**
   * Print charging.
   */
  public static void main(String[] args) {
    int kostenProKwh = 50;
    int kostenProMinute = 30;
    int currentKosten;
    int total = 0;

    currentKosten = 50 * kostenProKwh + 60 * kostenProMinute;
    total += currentKosten;
    System.out.println(currentKosten);

    currentKosten = 70 * kostenProKwh + 90 * kostenProMinute;
    total += currentKosten;
    System.out.println(currentKosten);

    currentKosten = 55 * kostenProKwh + 70 * kostenProMinute;
    total += currentKosten;
    System.out.println(currentKosten);
    System.out.println(total);
  }
}

```

2. write a code to count the number of rice.

```java

package rice;

/**
 * Print rice.
 */
public class Rice {

  /**
   * Print rice.
   */
  public static void main(String[] args) {

    int koerner = 3;
    int prozent = 50;
    int currentNumber = koerner;
    int total;

    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    total = currentNumber;
    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    total += currentNumber;
    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    total += currentNumber;
    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    total += currentNumber;
    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    total += currentNumber;
    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    total += currentNumber;
    System.out.println(currentNumber);
    currentNumber = currentNumber + currentNumber * prozent / 100;
    System.out.println(currentNumber);
    total += currentNumber + koerner;
    System.out.println(total);
  }
}

```

3. Practice

How can you describe this expression in Java?

       num∈[min,max]

⇛ num >= min && num <= max

