# React Review

 ## Component-Based Architecture

 Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides the problem into sub-problems, each associated with component partitions.

 The primary objective of component-based architecture is to ensure component reusability. A component encapsulates functionality and behaviors of a software element into a reusable and self-deployable binary unit.

 Component-oriented software design has many advantages over the traditional object-oriented approaches such as:

 - Reduced time in market and the development cost by reusing existing components.

 - Increased reliability with the reuse of the existing components.

 ## What is a Component?

 A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

 A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

## Principles of Component−Based Design

 A component-level design can be represented by using some intermediary representation (e.g. graphical, tabular, or text-based) that can be translated into source code. The design of data structures, interfaces, and algorithms should conform to well-established guidelines to help us avoid the introduction of errors.

 - The software system is decomposed into reusable, cohesive, and encapsulated component units.

 - Each component has its own interface that specifies required ports and provided ports; each component hides its detailed implementation.

 - A component should be extended without the need to make internal code or design modifications to the existing parts of the component.

 - Depend on abstractions component do not depend on other concrete components, which increase difficulty in expendability.

 - Connectors connected components, specifying and ruling the interaction among components. The interaction type is specified by the interfaces of the components.

 - Components interaction can take the form of method invocations, asynchronous invocations, broadcasting, message driven interactions, data stream communications, and other protocol specific interactions.

 - For a server class, specialized interfaces should be created to serve major categories of clients. Only those operations that are relevant to a particular category of clients should be specified in the interface.

 - A component can extend to other components and still offer its own extension points. It is the concept of plug-in based architecture. This allows a plugin to offer another plugin API.

# References

 [1] <https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm>

 [2] <https://www.youtube.com/watch?v=Tn6-PIqc4UM&ab_channel=Fireship>

 [3] <https://www.youtube.com/watch?v=TNhaISOUy6Q&ab_channel=Fireship>




