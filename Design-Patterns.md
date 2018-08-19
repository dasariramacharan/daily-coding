References : 
https://docs.microsoft.com/en-us/azure/architecture/patterns



Cloud Design Patterns
1. Compensating Transaction pattern 
    Undo the work performed by a series of steps, which together define an eventually consistent operation, if one or more of the steps fail.
    https://docs.microsoft.com/en-us/azure/architecture/patterns/compensating-transaction
    

4.  Circuit Breaker pattern
    Handle faults that might take a variable amount of time to recover from, when connecting to a remote service or resource. 
    This can improve the stability and resiliency of an application.

Availability patterns

1. Health Endpoint Monitoring pattern
       Implement functional checks in an application that external tools can access through exposed endpoints at regular intervals.
       
2. Queue-Based Load Leveling	
        Use a queue that acts as a buffer between a task and a service that it invokes in order to smooth intermittent heavy loads.

3. Throttling	
         Control the consumption of resources used by an instance of an application, an individual tenant, or an entire service.



Data Management patterns

1. Cache-Aside	Load data on demand into a cache from a data store 

2. CQRS -Command And Query Responsibility segregation Pattern
     Segregate operations that read data from operations that update data by using separate interfaces. 

3. Event Sourcing
     Use an append-only store to record the full series of events that describe actions taken on data in a domain.
     
4. Index Table
      Create indexes over the fields in data stores that are frequently referenced by queries.    

5. Materialized View	
       Generate prepopulated views over the data in one or more data stores when the data isn't ideally formatted for required query operations.

6. Sharding	 
        Divide a data store into a set of horizontal partitions or shards. 
        Strategies to do create select shard key and distribute it are a)The Lookup strategy b)The Range strategy c)The Hash strategy.  
       
7. Static Content Hosting pattern
        Deploy static content to a cloud-based storage service that can deliver them directly to the client.  

8. Valet Key pattern 
        Use a token or key that provides clients with restricted direct access to a specific resource or service (when using Static Content Hosting pattern).
        
 
 Messaging patterns
 
 1.Competing Consumers	
        Enable multiple concurrent consumers to process messages received on the same messaging channel.
 
2.  Pipes and Filters pattern
     Decompose a task that performs complex processing into a series of separate elements that can be reused. 
      
3.  Priority Queue	
     Prioritize requests sent to services so that requests with a higher priority are received and processed more quickly than those with a lower priority.

4. Queue-Based Load Leveling	
     Use a queue that acts as a buffer between a task and a service that it invokes in order to smooth intermittent heavy loads.
     
5. Scheduler Agent Supervisor	
     Coordinate a set of actions across a distributed set of services and other remote resources.     


Design and Implementation patterns
      Good design encompasses factors such as consistency and coherence in component design and deployment, maintainability to simplify
administration and development, and reusability to allow components and subsystems to be used in other applications and in other
scenarios.

1. Ambassador
     Create helper services that send network requests on behalf of a consumer service or application.

2.Anti-Corruption Layer	
      Implement a façade or adapter layer between a modern application and a legacy system.

3. Backends for Frontends	
      Create separate backend services to be consumed by specific frontend applications or interfaces.

4. Compute Resource Consolidation	
       Consolidate multiple tasks or operations into a single computational unit.

5. External Configuration Store	
       Move configuration information out of the application deployment package to a centralized location.

6. Gateway Aggregation	
       Use a gateway to aggregate multiple individual requests into a single request.
      
7.Gateway Offloading	
     Offload shared or specialized service functionality to a gateway proxy.       

8.Gateway Routing	
     Route requests to multiple services using a single endpoint.
        
7.Leader Election
       Coordinate the actions performed by a collection of collaborating task instances in a distributed application by electing one instance as the leader that assumes responsibility for managing the other instances.

8.Sidecar
        Deploy components of an application into a separate process or container to provide isolation and encapsulation.
     
        
        
