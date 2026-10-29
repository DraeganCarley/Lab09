# Lab09
# Sequential Circuits: Latches


In this lab, you learned about the basic building block of sequential circuits: the latch.


## Rubric


| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |


## Names
Group #7 - Aaron Ray and Draegan Carley
## Summary
In this week's lab, we learned about sequential logic and how to create circuits that can store information. We started by learning about SR-Latches and how they can hold a value even after the inputs change. We then learned about D-Latches and how they use an enable signal to control when data is stored. We used behavioral Verilog to create a D-Latch and expanded on this to create a four-byte memory system. This helped me better understand how memory works in digital circuits and how we can combine latches with multiplexers and demultiplexers to store and retrieve data.
## Lab Questions


###  Why can we not just use structural Verilog to implement latches?
We cannot just use structural Verilog because latches require feedback loops to hold their values. While we can create these loops using structural Verilog, Vivado recognizes them as combinational loops and will not allow them to synthesize normally. By using behavioral Verilog, we can describe how the latch should work and allow Vivado to implement it correctly.
### What is the meaning of always @(*) in a sensitivity block?
The always @(*) statement tells Verilog to run the block whenever any of the signals being used inside it change. This makes it easier because we do not have to manually list every input in the sensitivity list. It is commonly used for combinational logic, but it can also describe a D-Latch when the code allows the output to hold its previous value.
### What importance is memory to digital circuits?
Memory is important because it allows digital circuits to store information instead of only reacting to their current inputs. Without memory, a circuit would lose its previous values whenever the inputs changed. By using memory, we can save data and use it later, which is important for more complicated systems like computers and processors. It also allows circuits to hold values until they are ready to be changed or used again.
