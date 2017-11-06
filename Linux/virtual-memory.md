What is virtual memory? (in linux)
----------------------------------


- using a disk as an extension of RAM
- the kernel will write the contents of a currently unused block of memory to the hard disk so that the memory can be used for another purpose
- where the original contents are needed again, they are read back into memory
- part of the hard disk used as the virtual memory is named __swap space__

|swapping| paging|
|--------|-------|
|writing the wholw peocess out to swap|writing only fixed size parts, usually a few kilobytes, at a time|
