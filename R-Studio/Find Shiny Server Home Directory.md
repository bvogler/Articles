#Find Home directory in Shiny Server

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





