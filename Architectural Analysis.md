Core idea is identifying the factors that influence the architecture and the variability and priority of them. Goal is to reduce critical factors of the design of a system.
Used to address concerns related to non-functional requirements with awareness of business context and functional requirements and their variability, alongside concerns to system-level and other broad problems, resolution involving large scale or fundamental design decisions.
Address interdependencies and trade-offs (Security/performance or anything/cost)
Involves generation/evaluation of alternatives.

**Architecturally significant functional requirements:**
![[Pasted image 20241025202456.png]]
**Architecturally significant functional requirements:**
Usability (UI/UX), reliability, performance, supportability

Though this can differ depending on the context
General steps in architectural analysis:
1. Identify/analyse factors and impact on the architecture (What's requirement and non-requirement)
2. What architectural decisions should be made (Remove requirement, custom solution, stop project, need expert etc)
Priorities:
1. Inflexible constraints like safety, security, legal compliance
2. Business goals like demo for client tradeshow in ~18 months, competitor driven window of opportunity
3. Other goals such as higher level goals and later business goals, extendable
There exists a factor table to describe notable factors, their priorities and variability
1. actor
2. Measures and quality scenarios
3. Variability (Current flexibility and future evolution)
4. Impact of factor (and variability) on stakeholders, architecture and other factors
5. Priority for success
6. Difficulty or risk
![[Pasted image 20241025203934.png]]

Technical memos often used to record alternative solutions, decisions, notable factors and motivations for noteworthy issues and decisions, consists of
- Issue 
- Solution summary
- Factors
- Solution
- Motivation
- Unresolves issues
- Alternatives considered

**Technical Memo: Issue: Reliability—Recovery from Remote Service Failure**
**Factors**
Robust recovery from remote service failure, e.g., tax calculator, inventory
**Solution**
To satisfy the quality scenarios of reconnection with the remote services ASAP,   use smart Proxy objects for the services, that on each service call test for remote service reactivation, and redirect to them when possible. 
Where possible, offer local implementations of remote services. For example, implementing a small cache to store data (e.g., tax rates)
Achieve protected variation with respect to location of services using an Adapter created in a ServicesFactory.
**Motivation**
	Retailers really don't want to stop making sales! Therefore, if the NextGen POS offers this level of reliability and recovery, it will be a very attractive product, as none of our competitors provide this capability. The small product cache is motivated by very limited clientside resources. The real thirdparty tax calculator is not replicated on the client primarily because of the higher licensing costs, and configuration efforts (as each calculator installation requires almost weekly adjustments). 
	This design (Adapter and ServiceFactory) also supports the evolution point of future customers willing and able to permanently replicate services such as the tax calculator to each client terminal. 
**Unresolved Issues**
none  
**Alternatives Considered**
A “gold level” quality of service agreement with remote credit authorization  
services to improve reliability. It was available, but much too expensive.

