#  Code Smells Analysis

| Code Smell | Where in the Code? | Principle Broken |
|---|---|---|
| Magic Numbers | 1200, 0.5, 2000, and 5000 | Maintainability |
| Long Conditional | Repeated if/elif statements checking the invoice kind | Open/Closed Principle (OCP) |
| Long Function | make_invoice() calculates fees, formats text, writes to a file, and prints the invoice | Single Responsibility Principle (SRP) |
| Manual Resource Management | The file is opened using open() and closed manually | Safe Resource Management |
| Tight Coupling | make_invoice() directly handles file writing and printing | Dependency Inversion Principle (DIP) |

