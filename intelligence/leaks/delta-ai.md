# Delta: A General Purpose AI Kernel, Programming Language and Operating System.


Overview


We present a novel approach to general purpose AI.


We present an AI Architecture that is capable of demonstrating general purpose intelligence over a wide variety of tasks. This Kernel in this architecture is capable of executing general purpose programs written for it, operating over functionally unbounded state space. Programs are natural language instruction sets that the Kernel executes, with user defined parameters that allow general purpose programs to be written.


The Kernel is backed by foundation LLM models, capable of returning function-calling responses, and operates as an orchestration layer between backend models the the programs executing on the Kernel.


The Kernel is based around the Delta algorithm, which mimics general human intelligence by recursively iterating over the same task, updating a portion of the task state each turn. This relies on a novel approach to data representation and state management within LLMs, where the Kernel injects a representation of the state into each LLM call, in such a way that the LLM can address one portion of the state for change, through well defined functions.


The state representation varies from traditional compute where the byte, or word is the fundamental unit of data, and documents, etc, can be address by whole document, or individual word. We introduce the Memetic Knowledge unit, mku, which is a unit of knowledge represented by an array of tokens. The mku itself represents the knowledge contained in the tokens, which is an emergent property in relationship with an intelligence interpreting the tokens. LLMs are able to operate over collections of mkus in the context, and output changes that can be incorporated and the updated state injected into the next call.


Through this process of recursion towards the same task over an updated state, the Kernel is able to demonstrate higher orders of intelligence, through the process of emergence. This mimics how humans operate on complex tasks, by externalizing their representation and continuing to operate on it until complete.


Resources are available to the Kernal which enable access to data, features, rendering environments, etc. These resources can be Memetically backed data (e.g. A Memetic File is a List of MKu), or external systems such as APIs and modules. Each resource is responsible for 

Instructing the underlying LLM on how to use the resource, any state the resource wants to present to the LLM, and providing function descriptions for actions the LLM can take on the resource. At each cycle, e.g. in the recursive loop, the AI can decide to call functions on the available resources. A combination of allowed / required resources for a program, and what resources a user makes available to the program permits for flexibility and safety.


===




Detailed Design


The framework consists of the following logical components,Kernel, Circuits, Resources, the Memetic Data Types, Programs, 
