---
layout: post
title:  "Bedingte Ausdrücke"
date:   2023-10-28 10:28:36 +0530
categories: EPR
---

1. Practice

If n is an even number, it will be the half, and if n is an odd number, it will be 3 * n + 1.

```java

n % 2 == 0
  ? n / 2
  : 3 * n + 1

```

Let c be a variable of type char. Implement an expression using c that has the following properties:
    • If c contains a letter between a and z, the value of the expression should be the corresponding
    uppercase letter.
    • If c contains a letter between A and Z, the value of the expression should be the corresponding
    lowercase letter.
    • If neither of these cases is true, the value of the expression should be the value of c.
The char data type represents characters that are internally encoded as integers between 0 and 65535.
You can perform arithmetic operations on the codes (and thus indirectly on the characters) and
you can compare them, for example, using <= or >=. The codes of the characters a to z are consecutive
(similarly for the uppercase letters).

```java

c >= 'a' && c <= 'z'
   ? (char) (c - 'a' + 'A')
   : c >= 'A' && c <= 'Z'
      ? (char) (c - 'A' + 'a')
      : c

```

Keep in mind

    a && b
    a ? b : false
    
Both are the same experessions.


2. Write a code for an electricity bill.

```java

package electricitybill;

/**
 * let us calculate the electricity bill.
 */
public class ElectricityBill {

  /**
   * let us calculate the electricity bill.
   */
  public static void main(String []args) {
    /*
     * based on the provided 5 variables in the task.
     */
    int annualConsumption = 3535;
    float basePrice1 = 17.07f;
    float basePrice2 = 19.53f;
    float consumptionPrice1 = 33.26f;
    float consumptionPrice2 = 30.17f;

    /*
     * calculate the total cost for each tariff without rounding and multiply by 100.
     */
    float total1 = annualConsumption * consumptionPrice1 + (basePrice1 * 100 * 12);
    float total2 = annualConsumption * consumptionPrice2 + (basePrice2 * 100 * 12);

    /*
     * round off.
     */
    total1 = 0.01f * (int) total1;
    total2 = 0.01f * (int) (total2 + 0.5);

    /*
     * The energy service provider selects the cheaper tariff.
     */
    System.out.println((total1 < total2)
            ? total1
            : total2);
  }
}

```