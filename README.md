# led_display
program that display a number with LCD like ascii characters

# compilation

compile with the following:   

gcc -o led main.c 

# Information (font)

The font consists of a 8x8 binary data. Each digit is 8x8 bits. So for a single digit, it consumes 8 bytes of memory, so 80 bytes in total for the whole font.

# Information (rendering)

Instead of doing any memory allocation, the digits are rendered from left to right one row at a time. The number of digits doesn't matter. The only memory allocation in the whole program is done when you call the function with the string. Some integers are used for the iteration through characters and pixels.

The program should be fast for the little thing it does but it was optimized for size and not speed.


