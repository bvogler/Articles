#Find Home directory in Shiny Server

<<<<<<< HEAD:R-Studio/Find Shiny Server Home Directory.md
Use Sys.getenv to get the environment variables.  Normal the environment variable “HOME” is set toto the home directory.

###Example
Sys.getenv(“HOME”)

###Usage
Sys.getenv(x = NULL, unset = "", names = NA)

###Arguments
xa character vector, or NULL.unseta character string.nameslogical: should the result be named? If NA (the default) single-element results are not named whereas multi-element results are.Details
Both arguments will be coerced to character if necessary.
Setting unset = NA will enable unset variables and those set to the value "" to be distinguished, if the OS does. POSIX requires the OS to distinguish, and all known current R platforms do.

###Value
A vector of the same length as x, with (if names == TRUE) the variable names as its names attribute. Each element holds the value of the environment variable named by the corresponding component of x (or the value of unset if no environment variable with that name was found).
On most platforms Sys.getenv() will return a named vector giving the values of all the environment variables, sorted in the current locale. It may be confused by names containing = which some platforms allow but POSIX does not. (Windows is such a platform: there names including = are truncated just before the first =.)
When x is missing and names is not false, the result is of class "DList" in order to get a nice print method.
=======
Use Sys.getenv to get the environment variables.  Normal the environment variable ï¿½HOMEï¿½ is set toto the home directory.
###Example
Sys.getenv(ï¿½HOMEï¿½)

###Usage
Sys.getenv(x = NULL, unset = "", names = NA)
###Arguments


x a character vector, orï¿½NULL.
unset a character string.
names logical: should the result be named? Ifï¿½NAï¿½(the default) single-element results are not named whereas multi-element results are.
Details
Both arguments will be coerced to character if necessary.
Settingï¿½unset = NAï¿½will enable unset variables and those set to the valueï¿½""ï¿½to be distinguished,ï¿½if the OS does. POSIX requires the OS to distinguish, and all known currentï¿½Rï¿½platforms do.
Value
A vector of the same length asï¿½x, with (ifï¿½names == TRUE) the variable names as itsï¿½namesï¿½attribute. Each element holds the value of the environment variable named by the corresponding component ofï¿½xï¿½(or the value ofï¿½unsetï¿½if no environment variable with that name was found).
On most platformsï¿½Sys.getenv()ï¿½will return a named vector giving the values of all the environment variables, sorted in the current locale. It may be confused by names containingï¿½=ï¿½which some platforms allow but POSIX does not. (Windows is such a platform: there names includingï¿½=ï¿½are truncated just before the firstï¿½=.)
Whenï¿½xï¿½is missing andï¿½namesï¿½is not false, the result is of classï¿½"DList"ï¿½in order to get a niceï¿½printï¿½method.
>>>>>>> cdf82ecdb4f9691159b07957d8d6f4a0eb84d756:R-Studio/Find Shiny Server Home Directory.txt





