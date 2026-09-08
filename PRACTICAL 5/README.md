# Practical 5: Rule-Based Expert System / Logic Inference Engine

## README Summary

### Aim

To build a small **rule-based expert system or logic inference engine** for solving a diagnosis or advisory problem using predefined rules and facts.

### Description

A rule-based expert system is an artificial intelligence system that uses a collection of **facts, rules, and an inference mechanism** to make decisions or provide recommendations. In this practical, the system takes user-provided information as input, compares it with predefined rules, and generates an appropriate diagnosis or advice.

The system generally consists of:

* **Facts:** Information provided by the user.
* **Rules:** IF–THEN statements that represent expert knowledge.
* **Inference Engine:** Matches the available facts with the rules.
* **Output:** Provides the diagnosis, recommendation, or conclusion based on the matched rules.

### Example

For a simple health-diagnosis system:

* **Rule 1:** IF fever AND cough THEN possible flu.
* **Rule 2:** IF fever AND sore throat THEN possible throat infection.
* **Rule 3:** IF headache AND fever THEN possible viral infection.

If the user provides the facts **fever** and **cough**, the inference engine matches Rule 1 and produces **possible flu** as the result.

### Working

1. Define the problem and possible outcomes.
2. Create a set of facts and IF–THEN rules.
3. Accept relevant facts from the user.
4. Compare the input facts with the conditions in the rules.
5. Apply the matching rules using the inference engine.
6. Display the resulting diagnosis or recommendation.

### Technologies

The system can be implemented using a programming language such as **Python**, using basic conditional statements, lists, dictionaries, or a simple inference mechanism.

### Learning Outcome

This practical demonstrates how expert knowledge can be represented using rules and how a computer can perform logical reasoning to reach a conclusion. It also provides an understanding of the basic working of **expert systems, knowledge bases, and inference engines**.

---

## Conclusion

The rule-based expert system was successfully designed to solve a simple diagnosis or advisory problem using predefined facts and IF–THEN rules. The inference engine analyzed the available information, matched it with the appropriate rules, and generated a suitable conclusion.

This practical helped in understanding the fundamental concepts of **Artificial Intelligence, knowledge representation, rule-based reasoning, and logical inference**. Although the system is small and depends on predefined rules, it demonstrates the basic principles used in larger expert systems and decision-support applications.
