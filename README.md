# compiladores
This contains my codes for the ç compiler, ç being the made-up language for this university course.
The basis for the lexical analysis is a automata with 5 states, each state dealing with a different kind of base tokens.
0 - operators/special characters.
1 - identifiers.
2 - numerical constants.
3 - char constant.
4 - string constant.

The syntax analysis was made using a slr1 parser that generates a map<int,map<string,vector<string>>>, where the int represents the automata state, the string represents the variables(terminal and non-terminal) and the vector contains information about each transition.
