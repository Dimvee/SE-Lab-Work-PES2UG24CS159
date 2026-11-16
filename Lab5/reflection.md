# Lab 5 – Static Code Analysis: Reflection

**1. What did you learn from this lab?**

I learned how to use Pylint, Bandit, and Flake8 to identify code quality issues, security vulnerabilities, and formatting errors in Python programs.

**2. What is the importance of static code analysis?**

Static code analysis helps identify errors and potential security problems without executing the program. It improves code quality, security, readability, and maintainability.

**3. What problems did you identify in your Python program?**

I identified unsafe XML parsing, a hardcoded password, unsafe shell command execution, mutable default arguments, naming convention problems, missing docstrings, and formatting errors.

**4. How did you fix the identified problems?**

I replaced the unsafe XML parser with defusedxml, removed the hardcoded password, replaced os.system() with a safer HTTP connection, changed mutable default arguments to None, improved naming conventions, added docstrings, and corrected formatting issues.

**5. What were the final results after using the tools?**

After fixing the issues, Pylint achieved a score of 10/10, Bandit reported zero security issues, and Flake8 reported zero formatting errors.

**6. What did you understand about the three tools?**

Pylint checks code quality and logical issues, Bandit identifies security vulnerabilities, and Flake8 checks Python coding style and formatting.

**7. How does static analysis help developers?**

It helps developers find problems early, write secure and clean code, reduce errors, and make programs easier to maintain.