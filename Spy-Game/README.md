### Project Overview

 I, the lieutenant decipher a message that was received from his intel. He has multiple text files that need to be read and have certain operations performed to get final message. He uses the intermidiate Python language i.e. String operations, Conditional statement and loops, File I/O, Functions to get final message.


### Learnings from the project

 After completing this project, I have a better understanding of solving logical problems using python. In this project, I have applied the following concepts:

**String operations
Conditional statement and loops
File I/O
Functions**


### Approach taken to solve the problem

 
 **## Step 1**: The first thing I did is to write a function that reads the contents of the files that we have.

The path for file has been stored in a variable 'file_path'

Write a function "read_file()" that :

    Takes 'path' as a parameter.

    Opens the file associated with the 'path' in the read-only mode ('r') and store it in a variable file.

    Reads the content(first line) of the file and stores it in a variable called 'sentence'

    Closes the file

    Returns 'sentence'

Call the function "read_file()" with 'file_path' as input parameter and store the result in a variable called 'sample_message'

**## Step 2**: In this task, I have used messages of two different files. In the two files, I have one number each. I have to apply a certain operation to extract message.

Path for the two files that you will require for this task has been stored in variables file_path_1 and file_path_2

Call the function read_file() written in the previous task for file_path_1 & file_path_2 and store their message sentences in variables message_1 and message_2 respectively.

Print message_1 and message_2 to see what they contain.

Write a function fuse_msg() that :

    Takes message_a and message_b as parameters

     Implements integer(floor) division of message_b over message_a and stores the quotient in a variable called quotient

    Returns quotient in string format.

Call the function fuse_msg() with message_1 & message_2 and store the result of it in a variable called secret_msg_1

**## Step 3**: In this task, I have substituted the message of the file for a secret message.

Path for the file that you will require for this task has been stored in variables file_path_3

Call the function read_file() for file_path_3 and store its message sentences in variables message_3

Print message_3 to see what it contains.

Write a function substitute_msg() that :

   Takes message_c as a parameter

   Creates a new variable 'sub' and in it stores

      'Army General' if message_c is 'Red'
      'Data Scientist' if message_c is 'Green'
      'Marine Biologist' if message_c is 'Blue'

   Returns 'sub'

Call the function "substitute_msg()" with 'message_3' and store the result of it in a variable called 'secret_msg_2'

**## Step 4**: In this task, I have used messages from two different files. I have to compare the two messages and take only those words that appear in first message but not in second message.

Path for the two files that I will require for this task has been stored in variables file_path_4 and file_path_5

Call the function read_file() for file_path_4 & file_path_5 and store their message sentences in variables message_4 and message_5 respectively

Print message_4 and message_5 to see what they contain.

Write a function compare_msg() that :

    Takes message_d and message_e as parameters
    Breaks down the sentences in message_d & message_e into words using split() function and stores them in a_list & b_list respectively

    Stores all the words that are there in a_list but not in b_list in a new list called c_list

    Combines the words of c_list back to a sentence using join() and stores it in a variable called final_msg and returns it

Call the function "compare_msg()" with 'message_4' & 'message_5' and store the result of it in a variable called 'secret_msg_3'

**## Step 5**: In this task, I have to extract only those words from the message in the file that are of even length.

Path for the file that I will require for this task has been stored in variables file_path_6

Call the function read_file() for file_path_6 and store its message sentence in variables message_6

Print message_6 to see what it contains.

Write a function extract_msg() that :

    Takes message_f as a parameter

    Breaks down the sentence in message_f into words and stores them in a_list

    Creates a lambda function called even_word with the condition that will return true if length of x (lambda function variable) is even

    Implements filter() function with function parameter as even_word and sequence parameter as a_list and stores the result of it in a variable called b_list

    Combines the words of b_list back to a sentence and stores it in a variable called final_msg and returns it

Call the function "extract_msg()" with 'message_6' and store the result of it in a variable called 'secret_msg_4'

**## Step 6**: I have successfully deciphered all the message bits that I received. In this final task, I will combine all the message bits into a single message and write it in a file.

The message parts that I deciphered have been provided to me in the order that they have to be read, in a list called message_parts.

Combine the contents of message_parts into a single sentence and store it in a variable called secret_msg

Write a function write_file() that :

    Takes secret_msg and pathas parameters

    Opens the file mentioned in the path in a+ mode

    Writes the content of the secret_msg in the above opened file

    Closes the file

The function has no return parameters

Call the function "write_file()" with 'secret_msg' and 'final_path'
(final_path= user_data_dir + '/secret_message.txt')
Printed the content of the 'secret_msg' so I can also see the message




