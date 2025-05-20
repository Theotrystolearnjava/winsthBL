Bootlaoder:
    first stage:
        [ ] | start at 0x000:7c00 / 0x7c0:0x0000
        [ ] | Enforce CS:IP | CS = Code Segment; IP = Instruction Pointer | Example above (0x000:7c00 ~ CS:IP)
        [ ] | Change mode into the preferred one, if not already in it
        [ ] | Load second stage into memory | BIOS INT 13h (BIOS Interrupt 13h)
        [ ] | Pass Control to second stage | jump to memory address where it's loaded into
    second stage:
        [ ] | Seome stuff here probably..
        [ ] | Load kernel into memory and pass control to it
