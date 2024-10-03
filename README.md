# Arithmetic-Formatter-Project
Immediately after the declaration of the function arithmetic arranger, there are five new empty lists.
Let's all one by one.
## 1. all_elements
The input problem is a list of atmost five string elements. By applying the split command with in the first for loop, the input(problem) gets segmented and all the new ists are added to the empty list called all_elements. By removing the '#' sign you can see what the list all_elements consists of; just as follows.
[['44', '+', '815'], ['909', '-', '2'], ['45', '+', '43'], ['123', '+', '49'], ['888', '+', '40'], ['653', '+', '87']]
## 2. operand1_list
Operands in this sense are, the two numbers upon which a certain mathematical operation (addition or subtraction) is to be made Accordingly, operand1 is the first number that is found in the left had side of the '+' or '-' sign. Thus the list operand1_list looks like  as follows. By removing the '#' sign you can see what the list operand1_list consists of; just as follows.
[44, 909, 45, 123, 888, 653]
## 3. operand2_list
This list is the same as operand1_list except it consists of the right hand side elements. The list becomes as follows.
[815, 2, 43, 49, 40, 87]
## 4. operator_list
Again in the same way to the operands' list, it consists of the math operation sign in order.
['+', '-', '+', '+', '+', '+']
NB. The lists explained here from number 2 through 4 are made inside the second for loop.
## 5. result_list
Inside the third for loop, the mathematical operation is done based on the order of the operands and the operator sign.  In this stage, we order Python to add or subtract the elements in operand2_list to operand1_list in their occurance order and based on the type of math. operation in operand_list. By removing the '#' sign you can see what the list result_list consists of; just as follows.
[859, 907, 88, 172, 928, 740]
By comleting this, we obtained the operands, the operators and the result of all the inputs.  What is next is how we arrange all these into a vertically formatted math problems.
## 6. line1, line2, line3, line4
The base idea to arrange into vertical format is to keep the number of all charactors in one block of math operation six including  white space. In order to keep all blocks to have six characters, we count the number of characters an element have, then we fill its difference with six by adding whitespaces equal to the differnce. For instance, the first element in the operand1_list is 44. 44 is just two characters, thus, to have a total of 6 characters, 4 whitespaces are added to it. Just like this we complete the line. 

The forth line follows the same procedure as the first line. In the second line, the difference is calculated between 6 and the '+' or '-' sign sollowed by one white space and followed by the operand2 character. For instance, the operands_list first element is 815 and the math sign is '+'. In this case we have three operand2  character, a plus sign and a white space that separates the plus sign and the operand. Thus, we have 5 characters. The difference between 6 and 5 is one. we just add  a single whitespace.

The third line is the dash line. The number of dashes is determined by the longer between line1 nd line2. For example, in the firt elements case, the second line has 5 characters while the firt has only 2. Similarly we find the difference between 6 and the length of longer character, 5, which is 1. So we just add a single white space and fill the remaining 5 characters by dashes.
