# bob-board

Tracks reverse engineering the Bob dishwasher ESP32 control board for repurposing.

## Stuuuuf.

esp32-wroom-32d

18 pin 4-wire spi
display model no JWS024N1DS04.V0

```
spi.     esp
1        nc
2        28 (IO17)
3        27 (IO16)
4        23 (IO15)
5        16 (IO13)
6        30 (IO18)
7        31 (IO19)
8        nc
9        nc
10       nc
11       nc
12       nc
13       nc
14       nc
15       ?
16       ?
17       ?
18       ?
```

header
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

rj45

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

touch pin

J1

```
[1 2]
  v
```

1 12 (IO27) (???)
2 12 (IO27)

idk both pins are connected to the same pin on the board? something something witchcraft idk ¯\_(ツ)\_/¯
