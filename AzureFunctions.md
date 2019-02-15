# Notes of Azure Function Fundamentals
## Azure Function:
Azure function is the idea of events and code. When a function is written in any programming language and the azure function knows the event to trigger it trigger it. <br>
Azure Function = Events + Code.<br><br>
Benifits: 
- Simplified Programming Model: Only need to write a code that respond to a event of interest.
    - No boilerpoate.
    - Focus on Business requirement.
- New Pricing Model: Pay As you go. Examlple: Listening for the queue but no new messages then no need to pay for this.(consumption/Dynamic plan)<br>
    - Billing Model:
        - Number of Execution
        - CPU time(s) * RAM(GB)
    - Free Monthly grant
        - 1M executions
        - 400000GB-s
    - Consumption Plan
        - Limited to five minutes per execution.
        - Optional Daily Quota in GBs

- Rapid and Simple Development:
    - Code within the portal.
    - Eliminate Boilerplate.
- No server to maintain
    - Automatic Scaling.

## Serverless Computing
There are servers but no need to worry because one can delegate the management of maintaining them to a third party(PaaS). 