Defined the packages in which software are defined. Concerned with large scale organisation of software and its packages, subsystems and layers.
Layers are coarse-grained grouping of classes, packages etc that has cohesive responsibility for major aspects of systems.
- UI, application logic and domain objects all important
There exists strict layered architecture, only calls upon services directly below it, relaxed layered architecture is higher calls upon several lower layers.
Used to address changes in system affecting other areas due to coupling, intertwine logic and UI, high coupling across areas of concern, and leads to impacts on division of development work.

![[Pasted image 20241025210312.png]]
![[Pasted image 20241025210322.png]]
Common layers:
![[Pasted image 20241025210352.png]]
