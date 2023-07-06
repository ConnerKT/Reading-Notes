# Exception Handling

This topic is important to me because I want to learn how to handle exceptions in my code.

## [Retrospective 1](https://connerkt.github.io/Reading-Notes/401/Class01/Retro01)

## References

<https://learn.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code?pivots=dotnet-7-0>.
<https://www.w3schools.com/cs/cs_user_input.php>.
<https://www.w3schools.com/cs/cs_methods.php>.
<https://learn.microsoft.com/en-us/dotnet/core/tutorials/debugging-with-visual-studio-code?pivots=dotnet-7-0>.
<https://learn.microsoft.com/en-us/visualstudio/get-started/csharp/tutorial-debugger?toc=%2Fvisualstudio%2Fdebugger%2Ftoc.json&view=vs-2019>.
<https://docs.microsoft.com/en-us/visualstudio/debugger/debugging-absolute-beginners?view=vs-2019>.
<https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-use-the-try-catch-block-to-catch-exceptions>.
<https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/exception-handling-statements>.

## Debugging in C#

Debugging is running our code in steps to fix the exact point where the mistake is made, its not perfect.

Make assumptions in order to try and solve it, try to dig for the answer before debugging.

Using the debug button, we insert a breakpoint.

Keep restarting and checking the debugger results, analyzing your code to determine where the mistake was made.

## Try and Catch in C#

**Try and Catch** are used to handle exceptions. You use the try block to try execute code and use the catches incase it catches a certain exception.

    try
    {
    // Code that might throw an exception
    int numerator = 10;
    int denominator = 0;
    int result = numerator / denominator; // This line will throw an        exception
    Console.WriteLine("The result is: " + result);
    }   
    catch (DivideByZeroException ex)
    {
    // Code to handle the exception
    Console.WriteLine("An exception occurred: " + ex.Message);
    }

## Things I want to know more about

I want to understand different features that are different about C# compared to JS

I want to know how to use the debugger better.

