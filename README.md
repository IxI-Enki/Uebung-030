# Uebung-03  --  Fakultät
<!--
## Lernziele:

## Aufgabenstellung:

### Beispiel:
### Beispielausgabe:

#### Hinweis:

-------------------------------
## *Zusatzaufgabe:*



-->
-------------------------------
# **SPOILER**

```c#
using System;

namespace Fakultät
{
  internal class Program
  {
    static void Main()
    {
      string userInput;
      int userInteger,
          output = 1;
      Console.Write("\n         Fakultätrechner " +
                    "\n================================" +
                    "\n Geben Sie eine ganze Zahl ein." +
                    "\n ");
      userInput = Console.ReadLine();
      int.TryParse(userInput, out userInteger);

      Console.Write($"{userInteger}! ergibt: ");
      if (userInteger == 0)
      {
        output = 1;
      }
      else
      {
        for (userInteger = userInteger; userInteger > 0; userInteger--)
        {
          output = userInteger * output;
        }
      }
      Console.Write($" {output} ");

      Console.Write("\nZum Beenden bitte Eingabetaste drücken ...");
      Console.ReadLine();
      Console.Clear();
    }
  }
}
```
