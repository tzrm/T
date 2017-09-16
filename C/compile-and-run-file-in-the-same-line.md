If you want to compile a file and then run it in the same file in linux, you can do this:

> gcc myprog.c -o myprog && ./myprog

Where && means that the new program will run only if it compiles successfully.
If there is a problem with the compile, it will skip running the program and simply display the errors on the screen.
