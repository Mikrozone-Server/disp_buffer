# print_to_buffer

Script for creating a RAM buffer of the small dots matrix display

Display parameters are defined inside the script:

WIDTH - absolute X size of the destination screen buffer in pixels (eg. 128)

HEIGHT - absolute Y size of the destination screen buffer in pixels (eg. 64)

ORIENTATION - Portrait/Landscape


*Filesize of the outfile, is calclated as (WIDTH * HEIGHT) / 8*


## Usage

`print_to_buffer "text" Xpos Ypos [-e fontfile] -f filename`


### Options

  Xpos Ypos      ... X and Y position for start printing
  
  [-e | --fontfile <filename>]      ... file contains font
  
   -f | --outfile <filename>        ... output binary file as video RAM buffer
  
    
## Example
 `print_to_buffer "Hello wrold!" 0 10 [-e somefont.c] -f outbuffer.bin`
 
 .. will clear whole out buffer and printrendered text using somefont at position 0,10
 
