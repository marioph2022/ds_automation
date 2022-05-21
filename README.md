# Data Science Automation Tools

The idea of this repository is to create a list of data science tools that can help during development of AI or ML projects and contain automation features. There are examples of the usage for a few of the tools listed but this can be use as a starting point to try to include third-party products for automated projects.  It is expected that the number as well as the precision of them will increase to make them more powerful and to apply them in even more scenarios; however, the suggestion is to use a combination of both automation features and custom development where possible.

### List of tools

1. GPT3
2. AWS SageMaker Studio
3. AWS SageMaker Studio Lab
4. AWS Autopilot
5. DataRobot
6. GitHub Copilot
7. OpenAI Codex

## GPT3
Homepage - https://beta.openai.com/

GPT3 is Generative Pre-trained Transformer 3 performs a wide variety of natural language tasks.

This is a tool that can be used to create an application by adding features developed by this project.  This works with text in many different scenarios and it comprises 49 different categories at the time of this writing and a few examples were executed to see the result.

Some categories are:

- Q&A
- Grammar correction
- Summarize for a 2nd grader
- Text to command ...

Three categories were selected to describe the GPT3 tool capabilities: a translation from table and column names plus some text to a select statement, a simplification of complex text, and explanation of python code.  

By looking at the three examples i), ii) and iii) below, it can be seen that some training is needed or more experiments should run, for example, in the case of the select statement the created query does not include a group or a count to be closer to the correct statement.  Regarding the text in the quantum field, the simplification is identical to part of the original text but might be the text can not be translated unless important meaning is lost. The results were obtained by using the engine (or model) named "text-curie-001" so it might be worth trying a different one.

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

One more example with a slightly more complex code but adding a screenshot to show how the environment of the tools looks like.  There is an area where the text can be added (in this case Python code), text which is like a command and a submit button to execute the experiment.

![image](https://user-images.githubusercontent.com/98497219/169658105-65e94ddc-69c6-4e7a-8714-f9b24a26931e.png)


## Amazon SageMaker Studio
Homepage - https://aws.amazon.com/sagemaker/data-scientist/

Amazon SageMaker is a service with various components and the page added as a reference is one that can help in the data scientist role. This section is announced as Amazon SageMaker for Data Scientists with Integrated development environment (IDE) for the ML lifecycle.

Part of SageMaker is the Amazon SageMaker Studio that is an IDE where Jupyter Notebooks can be created but the studio has some other features which some are listed as follows:

- GitHub integration
- Terminals
- Settings
- Experiment

The automation part that should be mentioned here is known as Autopilot which can be started from file --> new --> experiment.  An experiment is a way of creating a machine learning model automatically and in this case the types of problems that are solved by this technique are: binary and multiclass classification, and linear regression las of 05/2022.  

By creating an experiment, it should be noted that there almost no requirement to execute the experiment since basically what is required is

- Input text file (path and file in S3, S3 is a AWS storage service)
- Output path (bucket and path in S3)

Once the file is loaded, the target column must be selected so the model can predict and determine the type of problem to solve. It is good to mention that the output location in S3 is needed because during the model creating multiple models are created to select the best one and this allows a user to work on the notebooks that were created automatically and store in S3.

![image](https://user-images.githubusercontent.com/98497219/169663072-11f90641-8d94-4c14-9180-62f440f95d3c.png)


## Amazon SageMaker Studio Lab
Homepage - https://studiolab.sagemaker.aws

There is faq section in their homepage that describes this tool as a free online web application for learning and experimenting with data science and machine learning using Jupyter notebooks.  This is based on the same technology as SageMaker Studio, but with limited computed, storage and a subset of the capabilities from the original one.

At the time of this writting the sign up process is in waitlist though the approval should be in at most five business days.

## AWS Autopilot
Homepage - https://aws.amazon.com/sagemaker/data-scientist/

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






