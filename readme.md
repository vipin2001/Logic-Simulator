# Logic Optimizer

Input a circuit in the Netlist format given below followed by the input values. The logic optimizer will implement the circuit layer by layer and process the input.

## NetList Format 
### Text File
Primary Output<br />
Circuit Name
Primary Input
OUT_NODE GATE_TYPE IN_NODE
....
END
Gate type can be:
AND
OR
NOT
XOR

### In Code 
You can edit the netlist give below in the format
["Primary Input", "Circuit Name","Primary Output","OUT_NODE GATE_TYPE IN_NODE", .... ,"END"]

## Using the Code
Circuit is a class initialized by a netlist input.
### Output Function
Takes in a a list of primary input in the format given below:
["Primary_Input_Variable_1 Primary_Input_Value_1", "Primary_Input_Variable_2 Primary_Input_Value_2",...]
and returns the value at output nodes.
### Netlist Loader
Takes the file address of .txt file consissting of multiple inputs with input order same as the alphabetic order of primary input and outputs a list of inputs.
.txt file format:
P1_Value P2_Value P3_Value...
.
.
.

### Ouputs Function
Takes in a list of inputs and outputs a list of output corresponding to the input.
