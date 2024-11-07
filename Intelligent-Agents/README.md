# Intelligent Agents

- **Simple Reactive Agent**: Implementation of an agent that responds to stimuli from the environment without using memory or learning.
- **Model-Based Agent**: Agent that maintains an internal model of the world to make more informed decisions.

---

## Simple Reactive Agent

A **simple reactive agent** is a type of agent that selects actions based solely on the current perception of the environment, without considering the history of perceptions or maintaining an internal state. This type of agent follows predefined condition-action rules, where each perception is associated with a specific action.

**Main characteristics:**

- **Simplicity**: Its design is simple, since it does not require storage of past information or complex processing.
- **Speed ​​of response**: By not processing historical information, it can react quickly to changes in the environment.
- **Limitations**: It cannot handle situations where the appropriate action depends on past events or requires future planning.

## Model-Based Agent

A **model-based agent** is an agent that, in addition to current perceptions, maintains an internal state that represents an understanding of the world. This internal state is continually updated and allows the agent to make more informed decisions, even in partially observable environments.

**Main characteristics:**

- **Internal State**: Stores information about the history of perceptions and the state of the environment.
- **Model of the World**: Possesses knowledge about how the environment works and how its actions affect it.
- **Predictive Ability**: Can anticipate the consequences of its actions and plan accordingly.

--- 

## Implementations

This repository includes practical implementations of the mentioned agents: 

**SimpleReactiveAgent:** 
- `garbage collector` 
- ``smart light`` 
- ``vacuum cleaner`` 
- ``vending machine ``

**ModelBasedAgent**: 
- ``traffic managment`` 
- ``vending machine ``

--- 

For any issues, suggestions, or contributions, please open an *Issue* or submit a *Pull Request*. Your input helps enhance the functionality and accuracy of this fuzzy logic risk assessment system.