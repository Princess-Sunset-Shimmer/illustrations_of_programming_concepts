# illustrations_of_programming_concepts
## compile from a source file to an executable file
[conceptional steps of translation from a source file to a executable file](https://odysee.com/@PrincessSunsetShimmer:5/convert:3?r=C1aSMbuRnkFY1YeXhdBUotkHNrBjgqCD)
![pic_0](https://player.odycdn.com/api/v4/streams/free/convert/3f9504767713e53b0df03edfe2eab43a7f061e47/5d71f1)
the real compiling steps are combined for translation acceleration

## layout of memoty allocation for an executable program file
[conceptional memory segmentation for an executable file](https://odysee.com/@PrincessSunsetShimmer:5/mem:c?r=C1aSMbuRnkFY1YeXhdBUotkHNrBjgqCD)
![pic_1](https://player.odycdn.com/api/v4/streams/free/mem/c17e7711f5d87bf2d48c6a141a7b5d653cb90ec6/205211)
- .text relates to function codes
- .data relates to global variable and static local variable both initialized with non-zero value
- .bss relates to global variable and static local variable both initialized with zero
- heap relates to calloc(), nalloc(), realloc(), and free();
- stack relates to function stack frame; showed as figure as below

[Stack Frame](https://odysee.com/@PrincessSunsetShimmer:5/sf:36?r=C1aSMbuRnkFY1YeXhdBUotkHNrBjgqCD)
![pic_2](https://player.odycdn.com/api/v4/streams/free/sf/36b65c3d66001d9521fb53dc9abcaa4787eb84d3/c2d869)
btw, the typical function has three main part
1. entry part:
    - allocate stack frame
    - store return address
    - store register if have to
3. main body part:
    - initialize local variable if have to
    - process local-variable, global-variable, and arguments if have to
    - passing self's callee's arguments and call self's callee if have to
    - continuously process self's callee's return-value, local-variable, global-variable, arguments, and return-value needs to be returned to self's caller if have to
5. leave part:
    - restore register if have to
    - restore return address
    - decallocate stack frame
    - return to origional point

## store bytes on memory
[little endian](https://odysee.com/@PrincessSunsetShimmer:5/l-e:0?r=C1aSMbuRnkFY1YeXhdBUotkHNrBjgqCD)
![pic_3](https://player.odycdn.com/api/v4/streams/free/l-e/06ca63d2b588d8e142095ca8b1807b902f58540c/894eba)
