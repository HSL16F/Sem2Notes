Domain models involves the identification of concepts, attributes and associations that are notable for the model.
A domain model represents *real world* situations via conceptual classes.
It is not software object, only noteworthy domain concepts or objects.
A type of domain model is a unified process (UP) business object model. It focuses on explaining things and products important to a business model.
[[UML]] is used to illustrate the model and design.
No operations (Method signatures) are defined in the class diagram
Domain model is essentially communicating the ideas and conceptual overview using domain vocabulary and information contextually supported by the given domain
Formally a conceptual class has:
Symbol: Words or images representing a conceptual class
Intension: Definition of of conceptual class
Extension: Set of examples of which conceptual class applies
![[Pasted image 20241010151501.png|400]]
Noun phrases common way to identify conceptual classes, though anything that allows us to identify the classes is valid, including common knowledge and category list
![[Pasted image 20241010151823.png|600]]
Associations is the relationship of the conceptual classes, significant in the domain context, knowledge of relationships is preserved.
![[Pasted image 20241010151953.png|400]]
Example of use case in lectures [[Week 2]] pg15-18
There can exists generalised super classes and subclasses, with some acting as general identifying and common elements, such as payment, with subclasses of cash, credit, check.
Subclasses are typically more specialised

Conceptual classes posses attributes which are logical values within the object. Attributes are includes in true conceptual class when use cases suggest of imply there is a need to store/remember information, example:
![[Pasted image 20241010152417.png]]
There are some considerations for creating **subclasses**
Subclass has additional attributes and associations of interest, and a subclasses are operated on, reacted to and/or manipulate different to other classes in noteworthy ways.
Both super and subclasses have attributes.
Design and [[System Sequence Diagrams]] share some aspects of the design.
![[Pasted image 20241010155217.png]]

#### Examples
![[Pasted image 20241010150856.png]]
![[Pasted image 20241010150934.png]]
![[Pasted image 20241010152435.png]]