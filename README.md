# bob-board

Tracks reverse engineering the Bob dishwasher ESP32 control board for repurposing.

## Stuuuuf.

esp32-wroom-32d

### 18 pin 4-wire spi

display model no JWS024N1DS04.V0 or QY24057A0-00

https://offer-product.oss-cn-beijing.aliyuncs.com/product/offer/attachment/null/file/subPdf_820578_362261_20240514-150813443.pdf

the one listed there uses ST7789V

```
spi.     esp
1        GND
2        28 (IO17)
3        27 (IO16)
4        23 (IO15)
5        16 (IO13)
6        30 (IO18)
7        31 (IO19)
8        ?
9        ?
10       ?
11       ?
12       ?
13       ?
14       ?
15       ?
16       ?
17       ?
18       ?
```

### unpopulated header

This will have to be populated to do the re-flashing.

(pin 1 nearest ESP when viewed from ESP Top Side)

```
 X
1       34 (RXD0)
 2      GND
3       35 (TXD0)
 4      GND
5       3  (EN)
 6      GND
7       35 (IO0)
 8      2 (3v3)
X
```

### rj45

This carries power, ground and probably a bunch of signals to trigger relays and sensors.

All I really want from that is the power and ground connections.

socket hole facing you

```
+--------+
|12345678|
+--| |--+
    -
1
2
3
4
5
6 GND
7
8

```

### touch pin

The touch sensor is attached to the door, and seems to be connected to two wires.

idk both pins are connected to the same pin on the board? something something witchcraft idk ¯\_(ツ)\_/¯

J1

```
[1 2]
  v
```

1 12 (IO27) (???)
2 12 (IO27)
