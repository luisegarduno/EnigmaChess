<div align="center">
  <img src="https://user-images.githubusercontent.com/30121656/195773070-262469d6-dc1d-425a-bf6b-726606e19ee5.png" width="300" />
  <br></br>
  
  [![EnigmaChess](https://github.com/luisegarduno/EnigmaChess/actions/workflows/build.yml/badge.svg)](https://github.com/luisegarduno/EnigmaChess/actions/workflows/build.yml)
  [![wakatime](https://wakatime.com/badge/user/57c8e6ad-7ce9-4067-864a-424b89ee01da/project/a1dce114-f23c-4ca0-bca1-78cda03e057e.svg)](https://wakatime.com/badge/user/57c8e6ad-7ce9-4067-864a-424b89ee01da/project/a1dce114-f23c-4ca0-bca1-78cda03e057e)
  ![TotalViews](https://hitscounter.dev/api/hit?url=https%3A%2F%2Fgithub.com%2Fluisegarduno%2FEnigmaChess&label=Total-Views&icon=&color=%230969da)
  
</div>

# _Enigma Chess_

EnigmaChess is a chess engine with clean & efficient code. 

## Prerequisites:
- Recommended - __Shell__: Bash, __OS__: Ubuntu v20.04
- Have the following packages installed: C++
  - `$ sudo apt install build-essential`


## Instructions:
__Option 1 (fastest)__
  1. Run the included build (`$ ./EnigmaEngine`)     

<br>

__Option 2 (fresh build)__
  1. In line 14 of *__main.cpp__*, replace _true_ with _false_     
  2. Compile the program (`$ g++ *.cpp *.h -std=c++17 -o EnigmaEngine`)     
  3. Run the generated file (`$ ./EnigmaEngine`)


<br></br>

----------------

(_at the moment_): Program creates a board using a FEN string that is defined in `main.cpp`.

Each square is assigned a number between 0-63. Once the initial board is created, it prompts the user to enter _S_, and _E_ afterwards.
- S = Starting index location for the piece you would like to move.
- E = End index location for where you would like to move the piece.

Example: [1] To move the white pawn from c2 to c3, then S=10, E=18. [2] To move the white pawn from g2 to g3, then S=14, E=22.

** Making a user input moves in this type of notation is very confusing. I also believe that the only pieces that can be moved at the moment are the pawns in the 2nd. Please note that both of these issues are something that i'm working on fixing. Once fixed, the program will be using the current standard for chess notation: algebraic notation. 
