---
layout: post
title:  "Typ-Konvertierung"
date:   2023-10-28 10:28:33 +0530
categories: EPR
---

Practice

Check if the experessions below are valid and how they can be converted.

    1.25 + 2.25

⇛ valid, and it will be converted into double.

    1.5 + 3.5F
    
⇛ valid, and it will be converted into double.

    3 >= (7 / 2)
    
⇛ valid, and it will be converted into boolean.

    23 * (9.87 > 10)
    
⇛ not valid.

    (char) ('b' - 1)
    
⇛ valid, and it will be converted into char.

    2 < 5 ? 14 : 1.4F
    
⇛ valid, and it will be converted into float.

    27 / (6 - (2 * 3))

⇛ valid, and it will be converted into int.

    314 / (float) 100
    
⇛ valid, and it will be converted into float.