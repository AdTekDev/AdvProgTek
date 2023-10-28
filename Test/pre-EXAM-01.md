
# pre-EXAM

## Q01

The following code is intended to replace all occurrence of substring sub1 by a new string nst in the original string str:

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

here the **strlen** return the length of the char string,   
and **findfirst** return the location of first occurrent of sub1 in str.   
**findfirst** return -1 if sub1 is not found in str.   
**movestr (char * src, char * dest)** move the substring at src to dst.  

Will the above implementation generates the desired result? if not, what is the problem and how to fix it?
