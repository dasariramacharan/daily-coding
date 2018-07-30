References : 
https://docs.microsoft.com/en-us/azure/architecture/patterns



Cloud Design Patterns
1. Compensating Transaction pattern 
    Undo the work performed by a series of steps, which together define an eventually consistent operation, if one or more of the steps fail.
    https://docs.microsoft.com/en-us/azure/architecture/patterns/compensating-transaction
    
2.  Pipes and Filters pattern
     Decompose a task that performs complex processing into a series of separate elements that can be reused. 
     This can improve performance, scalability, and reusability by allowing task elements that perform the processing to be
     deployed and scaled independently.The filters in a pipeline can be implemented as separate hosted tasks 
     running close to the data that they maintain.
     
3.  CQRS -Command And Query Responsibility segregation Pattern
     Segregate operations that read data from operations that update data by using separate interfaces. 

4.  Circuit Breaker pattern
    Handle faults that might take a variable amount of time to recover from, when connecting to a remote service or resource. 
    This can improve the stability and resiliency of an application.



Availability patterns

1. Health Endpoint Monitoring pattern
       Implement functional checks in an application that external tools can access through exposed endpoints at regular intervals.
       
2.
