---
layout: post
title: Code Examples
description: Example of code highlighting
tags: fortran c++ c python
---
FORTRAN

```fortran
PROGRAM fdate
!
! "@(#) fdate(1) writes timestamp using specified syntax"
!
   USE m_kracken                     ! command line parameter cracking module
   IMPLICIT NONE

   INTEGER , PARAMETER  :: clen=255  ! length of format
   CHARACTER(len=clen)  :: format    ! input format string

   INTEGER              :: ilen
   INTEGER              :: ier
   INTEGER              :: i10

   CHARACTER(LEN=8)     :: date      ! returned values from DATE_AND_TIME()
   CHARACTER(LEN=10)    :: time
   CHARACTER(LEN=5)     :: zone
   INTEGER,DIMENSION(8) :: values    

   LOGICAL              :: keyword   ! flag that previous character was a % character
   CHARACTER(LEN=1)     :: char      ! character being looked at in format string
```

Python
```python
# Import the modules
import sys
import random

ans = True

while ans:
    question = raw_input("Ask the magic 8 ball a question: (press enter to quit) ")
    
    answers = random.randint(1,8)
    
    if question == "":
        sys.exit()
    
    elif answers == 1:
        print "It is certain"
    
    elif answers == 2:
        print "Outlook good"
    
    elif answers == 3:
        print "You may rely on it"
    
    elif answers == 4:
        print "Ask again later"
    
    elif answers == 5:
        print "Concentrate and ask again"
    
    elif answers == 6:
        print "Reply hazy, try again"
    
    elif answers == 7:
        print "My reply is no"
    
    elif answers == 8:
        print "My sources say no"
```

C
```c
/*   
   A palindrome is a word, phrase, number, or other sequence of symbols or elements, 
  whose meaning may be interpreted the same way in either forward or reverse direction.
  This program will prompt the user to enter a word or a sentence and then confirms if 
  the user's entry is an palindrome or not.   
*/
#include <iostream>
#include <cstdlib>
 
bool isPalindrome( char [] );
 
int main( int argc, char *argv[] )
{
    char userString[300];
    std::cout << \"Type a word or phrase to see if it's a Palindrome.\" << \"\n\n\";
    std::cin.getline(userString, 300);      
    std::cout << \"\n\";
    if ( isPalindrome( userString ) )
            std::cout << \"\\"\" << userString << \"\\" is a Palindrome.\";
    else
            std::cout << \"\\"\" << userString << \"\\" is not a Palindrome.\";   
    std::cout << \"\n\n\";
    system( \"PAUSE\" );        
    return 0;
}
```

C++
```c++
#include <iostream>
using namespace std;

int main() {
  // Good name
  int minutesPerHour = 60;
  
  // OK, but not so easy to understand what m actually is
  int m = 60;
  
  cout << minutesPerHour << "\n";
  cout << m;
  return 0;
}

```