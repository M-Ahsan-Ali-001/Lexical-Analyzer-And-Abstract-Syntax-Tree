# Lexical Analyzer:

<br>•	First, take the  expression from the user  and store that in string.
<br>•	(**splitFunction()**) , in this function we store the characters one by one in a list and remove the white spaces.
<br>•	Print_Before_Tokenization() ,in this function we print the entered equation.
<br>•	tokenFinder(), in this function  we check the elements of split list one by using regular Expression to check form which category the current element belongs to.
<br>•	We get a match, we put that element in a dictionary along with is category type. 


### Regex used: 
 
            o	Re.search(‘[a-zA-Z]’ , element) :  it returns the if string contains alphabets.
            o	Re.search(‘[0-9]’, element) :  it returns the if string contains constants.
            o	Re.search(‘[+ , / , * ]’ , element) it returns the if string contains operators.
            o	Re.search(‘[{ , }  , ( , ) ]’ , element) it returns the if string contains punctuators.
            o	Re.search(‘[& , %  , $ ]’ , element) it returns the if string contains Speical Characters.



# Abstract Syntax Tree:
<br>•	First, take the  expression from the user  using Input_Equation() and store that in a string self.Expression.
<br>•	Tree_Parser() , in this function we use ast.parse() to tokenize the input expression , mode = ‘eval’ is used for evaluating the expression.
<br>•	Inter_nodes() , in this function we first use ast.walk() it is a built-in function used to visit the specified node , and recursively all its descendant , but in a non-specified order, ast.iter_fields() it is used overview the dictionary and ast.iter_child-nodes()  is use to print the keys of nodes.
<br>•	Dump_ast() , is use to  print the code in different components before actual execution.
<br>•	Evale_ASTree() , is a function used to evaluate the expression using output of ast.dump().
