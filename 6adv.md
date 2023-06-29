Q1. Three applications for exception processing are:

- Error handling: Exceptions provide a mechanism to handle and manage errors in a program. They allow you to detect and respond to unexpected conditions that may occur during the execution of your code. You can catch specific exceptions and handle them gracefully to prevent program crashes and provide meaningful error messages to users.

- Resource management: Exceptions can be used to ensure proper cleanup and release of resources. For example, if you're working with files, databases, or network connections, you can use exceptions to catch errors and ensure that resources are properly closed and released, even if an exception occurs.

- Program flow control: Exceptions can also be used to control the flow of your program. By raising exceptions in specific situations, you can alter the normal execution flow and handle exceptional cases differently. This allows you to handle specific conditions or trigger specific actions based on the occurrence of an exception.

Q2. If an exception is not properly handled or treated, it will propagate up the call stack until it reaches the top-level of the program. At that point, if the exception is still unhandled, it will terminate the program and display an error message, potentially leaving the program in an inconsistent or unrecoverable state.

Q3. The options for recovering from an exception in your script include:

- Handling the exception using a try-except block: You can catch and handle specific exceptions using a try-except block. Within the except block, you can provide code to handle the exception, perform necessary cleanup, and continue program execution.

- Raising a different exception: In some cases, you may want to catch an exception, perform some additional operations or checks, and then raise a different exception if needed. This allows you to modify the exception flow and provide more specific error information.

- Exiting the script: In certain situations, it may be appropriate to terminate the script gracefully if an exception occurs that cannot be recovered from. You can use the `sys.exit()` function to exit the script and provide an exit status indicating the reason for termination.

Q4. Two methods for triggering exceptions in your script are:

- Using the `raise` statement: You can explicitly raise an exception using the `raise` statement followed by the type of the exception. For example, `raise ValueError("Invalid input")` raises a `ValueError` exception with a custom error message.

- Invoking a method or function that raises an exception: You can call a method or function that is designed to raise specific exceptions based on certain conditions. For instance, calling the `open()` function to open a file that doesn't exist will raise a `FileNotFoundError` exception.

Q5. Two methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists, are:

- Using the `finally` block: The `finally` block is used in conjunction with a `try-except` block to specify code that should be executed regardless of whether an exception occurred or not. The code within the `finally` block will always be executed, ensuring cleanup or finalization actions are performed.

- Using the `atexit` module: The `atexit` module provides a way to register functions to be called when the Python interpreter is about to exit. You can use the `atexit.register()` function to register functions that should be executed at termination time. These functions will be called in the reverse order of registration.