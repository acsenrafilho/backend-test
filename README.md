# Backend Test

Develop the workflow's REST API following the specification bellow and document it.

## Delivery instructions

Clone this project and push a private repository in the [GitHub](https://github.com/). When you feel confortable to share your code, please share the repo with the following emails: 
   - antonio.filho@nuveo.ai
   - cesar.gimenes
   - 

Recall to add as much information and details as possible, which will be useful to our evaluation. A tip is using a README.md file to create an easy documentation to explain your thoughts and decisions. We accept documentation written in Portuguese or English. Feel free to choose any of those languages. 

Remember to explain the right way to execute your code!

## Defining a workflow

|Name|Type|Description|
|-|-|-|
|UUID|UUID|workflow unique identifier|
|status|Enum(inserted, consumed)|workflow status|
|data|JSONB|workflow input|
|steps|Array|name of workflow steps

## Endpoints

|Verb|URL|Description|
|-|-|-|
|POST|/workflow|insert a workflow on database and on queue and respond request with the inserted workflow|
|PATCH|/workflow/{UUID}|update status from specific workflow|
|GET|/workflow|list all workflows|
|GET|/workflow/consume|consume a workflow from queue and generate a CSV file with workflow.Data|

## Technologies

- Go, C, C++, Python, Java or any other that you know
- PostgreSQL
- A message queue that you choose, but describe why you choose
- Usage of TDD for the code development process

In case of any doubts, please enter in contact with us using the emails cited above.
