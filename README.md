# print-to-buffer

Script for creating a RAM buffer of the small dots matrix display

Display parameters are defined inside the script:
- `LCD_WIDTH` - absolute X size of the destination screen buffer in pixels (eg. 128)
- `LCD_HEIGHT` - absolute Y size of the destination screen buffer in pixels (eg. 64)
- ~~`ORIENTATION` - Portrait/Landscape~~

## Usage

`print-to-buffer Xpos Ypos "text" [ "filename"]`

### Options
- Xpos Ypos      ... X and Y position for start printing
- "text"         ... text to be written
- [ "filename" ] ... output binary file as video RAM buffer  
    
## Example
`print-to-buffer 0 10 "Hello world!" outbuffer.bin`
.. will clear whole out buffer and print rendered text using somefont at position 0,10
