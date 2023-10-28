
# pre-EXAM

## Q01

The following code is intended to replace all occurrence of substring **sub1** by a new string **nst** in the original string **str**:

```C++
void replacestr(char * str, char * sub1, char * nst)
{
  int lsub1= strlen(sub1);
  int lstr=strlen(nst);
  int location = findfirst(str, sub1);
  if (location!=-1) {
    movestr(&str[location+lsub1],&str[location+lnstr]);
    replacestr(&str[location+lsub1],sub1, nst);
  }
}
```

here:  
- the **strlen** return the length of the char string,   
- **findfirst** return the location of first occurrent of sub1 in str.   
- **findfirst** return -1 if sub1 is not found in str.   
- **movestr (char * src, char * dest)** move the substring at src to dst.  

Will the above implementation generates the desired result? if not, what is the problem and how to fix it?

## Q02

Subject of study is the (valid) C++ code below.

```C++

# i n cl u d e <i o st r e a m >
class A {
  publi c :
    int i ;

    A ( ) {
      i = 0 ;
    }
} ;

void fun (A a )
{
  a.i += 1 ;
  std::cout << a.i << std : : endl ;
}

int main ( int argc , char ∗ argv [ ] )
{
  A a ;
  fun ( a ) ; / / f u n c t i o n c a l l
  std::cout << a.i << std::endl ;
  return 0 ;
}
```

- Write down the terminal output of the program
- Rewrite function **fun** and the code in its scope to use **call-by-reference** instead of **call-by-value**. The output has to remain the same, and the application’s overall semantics (states) have to be preserved as well.




  
