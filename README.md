# 2018_LEDTetris

# 1. Overview 📖

Our goal was to create tetris game controlled by four buttons. The whole output is presented on two 8x8 LED matrices connected to each other.

# 2. Description 📌

Two merged matrices give us 128 diodes. We are using MAX7219 Driver which allows SPI communication. To control slowly dropping blocks during the game, we operate on 4 buttons. First is responsible for moving target one position right, second one position left, third increases speed of falling and the last one changes a shape of block.

# 3. Specification 📃

- 8x8 LED Matrix Specification



# 4. Tools 🔧

- STM32F4DISCOVERY,
- 8x8 LED Matrix + MAX7219 Driver (2x),
- Waveshare board 8 push buttons,
- Wires to connect the items.

# 5. How to run 🔥

Run program in System Workbench C/C++ Developers for STM32 and connect wires as follows





# 6. How to compile ⚡️

# 7. Future improvements 🔨

# 8. Attributions 💾

HAL library https://github.com/petoknm/MAX7219/

# 9. License 📑

MIT license. Read license.txt for more.

# 10. Cre
