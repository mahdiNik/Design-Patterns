# Design Patterns On C#

Design Patterns | Purpose | Sample in real life
--- | --- | ---
*Singleton* | Singleton Design Pattern aims to generate the object instance once and use it all the time and object instance is used the same everywhere. | An instance of the manager class related to the customers is created once and it used is everywhere on be require
*Factory Method* | Purpose is keep change under control. Creating an instance with a factory for similar classes that have implemented abstract classes (interface, abstract). Factories have separate conditions within themselves and according to the condition, it produces the class that has implemented the interface that the factory will return to. | For example, the project using MSSQL Server. If Oracle SQL Developer comes in the future, we can achieve this with small changes in our code thanks to the factory method design pattern.
*Abstract Factory* | While the factory method returns one instance, the abstract method has more than one factory method and can return more than one instance. | Let us be our car factory. And this factory will eventually produce cars, but the car model it produces may be different.
*Prototype* | We can use it when it is costly to create a new instance, and by cloning the existing object, we get an instance with a different reference from this object. | We can use it if we want to create the same from an object whose properties have values and use it in a slightly different way or for test objects
*Builder* | Creates the complex object step by step and returns this instance at the end. Just like the product produced on the factory production line. | Let's say we have a very complex model. Suppose that values from different databases or different sources are set to this model. We can create the values of this model step by step and return it.
*Facade* | Combining multiple objects in a single interface and consuming through this interface. Presenting the classes of a complex system in one place. | We can use it for dependency injections in the constructor in layers.
*Adapter* | Allows two incompatible systems work in compatible. | When using another service that is incompatible with our web service in our system.
*Composite* | Grouping objects in a tree structure. | We can establish hierarchical structure according to ranks of officers in police department.
*Proxy* | If always returned result of an operation is same value and this result usually does not change, we store value that will return in proxy. Return the stored value without any new operation. | If there is no change data in a table, we can write a proxy that returns the same value for select operations on the table.
*Decorator* | It provides new functionality in runtime by wrapping the object without changing the object. | Let's assume we have a structure that sends messages. message will be sent by mail, sms or any other way. We can create a decorator for each send path.
*Bridge* | Separates implementation and abstraction. | There are employee types and roles in a company. While designing this system, for example, there is abstract IPersonnel in abstraction part. Developer staff is refine abstraction which is child of the IPersonnel. In implementation part; abstract IRole implementor may have children, such as developer role and manager role. According to this structure, developer personnel who are IPersonnel class can use the developer role which is a IRole. In this way, a bridge between the abstract IPersonnel and the IRole is provided.
*Strategy* | Behavior of an object, its algorithm can change at runtime. | Let us have one Connection object and this object have a method called Connect. Let there be contexts that connect to A, B, C databases. Connect method keeps references of them in order to connect to any of them in different conditions.
*Observer* | Aims to notify subscribers about the incident with subscription system. | After following an account on the social media platform, receiving shared posts.
*Chain of Responsibility* | Each handler in chain either handles incoming request or transfers it to other. In this way, we regularly manage sequential complex steps in the code. | We can make user verification steps organized and manageable with help of this pattern.
*Memento* | Lets we save and restore previous state of an object. | We can define a memento list and use it for undo operations in text editor.
*Template Method* | Lets we have skeleton of algorithm in superclass. It aims to override required steps without breaking this skeleton in lower classes. | Lets we have a system that receives data from a source, sends data as a message and logs message. Used source, message sending method and logging methods in these stages may be different or some stages may be same. With this design pattern, we can prevent duplicate codes and proceed according to a certain layout.
*State* | Allows behavior to change according to the state of the object. | We can give an example of a video player.
*Mediator* | Aims to reduce dependency of tightly coupled objects. | In a form application, many components such as buttons, checkboxes, radio buttons, textboxes are dependent with each other. For example, when 1.checkbox is selected, it is bound by many conditions such as button will be hidden. Components interacting with others from one common place instead of each other will reduce dependency and increase developability.
*Visitor* | Aims to separate operations of objects from themselves. | Suppose we have a User class. The User class has many operations such as sending messages, updating. We can create a separate Visitor class, write accept method on our  User class, and send itself to the Visitor class received as a parameter in this method. Thus, when the existing operations of the User change or when new operations are added, we will only add it to the Visitor class without changing the User class.


