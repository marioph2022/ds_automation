# Data Science Automation Tools

The idea of this repository is to create a list of data science tools that can help during development of AI or ML projects and contain automation features. At the time of writing the sign up process is in progress and sample usage is pending.

### List of tools

1. GPT3
2. AWS SageMaker Studio Lab
3. AWS SageMaker Studio
4. AWS Autopilot
5. DataRobot
6. GitHub Copilot
7. OpenAI Codex

## GPT3
Homepage - https://beta.openai.com/

GPT3 is Generative Pre-trained Transformer 3 performs a wide variety of natural language tasks.

This is a tool that can be used to create an appliction by adding features developed by this project.  This works with text in many different scenarios and it comprises 49 different categories at the time of this writing and a few examples were executed to see the result.

Some categories are:

- Q&A
- Grammar correction
- Summarize for a 2nd grader
- Text to command ...

Three categories were selected to describe the tool capabilities: a translation from table and column names plus some text to a select statement, a simplification of complex code, and explanation of python code.  

By looking at the three examples i), ii) and iii) below, it can be seen that some training is needed or more experiments should run, for example, in the case of the select statement the created query does not include a group or a count to be a closer correct statement.  The results were obtained by using the engine (or model) named "text-curie-001" so it might be worth trying a different one.

Examples
### i) Create an SQL statement based on text
Text

Postgres SQL tables, with their properties: 

Employee(id, name, department_id) 
Department(id, name, address) 
Salary_Payments(id, employee_id, amount, date) 

### A query to list the names of the departments which employed more than 10 employees in the last 3 months 

Result

SELECT name FROM Salary_Payments WHERE employee_id > 10 AND date > 3 months

### ii) Summarize for a 2nd grader

Text

Quantum computing is a type of computation that harnesses the collective properties of quantum states, such as superposition, interference, and entanglement, to perform calculations. The devices that perform quantum computations are known as quantum computers.[1]: I-5  Though current quantum computers are too small to outperform usual (classical) computers for practical applications, they are believed to be capable of solving certain computational problems, such as integer factorization (which underlies RSA encryption), substantially faster than classical computers.[2] The study of quantum computing is a subfield of quantum information science. 

Result

Quantum computing is a type of computation that harnesses the collective properties of quantum states, such as superposition, interference, and entanglement, to perform calculations. The devices that perform quantum computations are known as quantum computers. Though current quantum computers are too small to outperform usual (classical)

### iii) Explain Python code

Python 3 Code

for idx in range(0, idx):
    print(2*idx)

Explanation of what the code does:

Result:

The code prints the value of 2 multiplied by the value of the variable idx.






## DataRobot
Homepage - https://www.datarobot.com/

Text taken from the home page - "From data preparation through value tracking, DataRobot equips you with enterprise-grade stability and scalabitlity you can count on."

There might be geo limits to access and sign up for an account.

## GitHub Copilot
Homepage - https://copilot.github.com/

Text taken from the home page - "Your AI pair programmer – With GitHub Copilot, get suggestions for whole lines or entire functions right inside your editor."

Sign up - in progress/waitlist

## OpenAI Codex

Homepage - https://openai.com/blog/openai-codex/

Text from their homepage: "We’ve created an improved version of OpenAI Codex, our AI system that translates natural language to code, and we are releasing it through our API in private beta starting today"






