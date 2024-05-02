# USBD Middleware Example - User View

This is the directory structure that a user should get when working with a MDK-Middleware example.

The Board layer is copied into a directory with the name `.\Board\B-U585I-IOT02A`.

## Workflow Issues

1. Initially the project does not have any target-types.  The message should hint the user towards it.

```txt
  target-types:
#    - type: B-U585I-IOT02A          # type name identical with board name?
#      board: B-U585I-IOT02A
#      variables:
#       - Board-Layer: $SolutionDir$\Board\B-U585I-IOT02A\Board.clayer.yml
#        - Board-Layer: C:\Test\USBD\Board\B-U585I-IOT02A\Board.clayer.yml

C:\Test\USBD>cbuild USB_Device.csolution.yml   
C:/Test/USBD/USB_Device.csolution.yml:6:3 - error csolution: node 'target-types' shall contain sequence elements
```

2. With Targets added, tool should detect the missing variable `Board-Layer` and search for compatible layers

```txt
  target-types:
   - type: B-U585I-IOT02A          # type name identical with board name?
     board: B-U585I-IOT02A
#      variables:
#       - Board-Layer: $SolutionDir$\Board\B-U585I-IOT02A\Board.clayer.yml
#        - Board-Layer: C:\Test\USBD\Board\B-U585I-IOT02A\Board.clayer.yml
```

## Workaround to allow build

- Board\B-U585I-IOT02A\CubeMX\HID.cgen.yml added to make this command working

```bash
cbuild USB_Device.csolution.yml -S
```

## Problems

- CMSIS-RTX pack: 
MISSING ARM::CMSIS:RTOS2:Keil RTX5&Source@5.8.0
  require Device:Startup

