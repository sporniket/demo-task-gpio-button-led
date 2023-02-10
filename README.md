# Demonstration of Tasks, Gpio, InputButton and Led libraries

C++ project made with PlatformIO, running on Espressif ESP32 based boards, that showcases some libraries that I wrote and serves as a maintenance workspace for those libraries.

The showcased libraries are :

* AnimatedValues : https://github.com/sporniket/AnimatedValues
* FeedbackLed : https://github.com/sporniket/FeedbackLed
* GpioAbstractionLayer : https://github.com/sporniket/GpioAbstractionLayer
* GpioAbstractionLayer-espressif32-espidf : https://github.com/sporniket/GpioAbstractionLayer-espressif32-espidf
* InputButton : https://github.com/sporniket/InputButton
* Task-espressif32-espidf : https://github.com/sporniket/Task-espressif32-espidf

This showcase consists of a blinking led and a push button. When the button is pushed, the led blinks three times per second, when the button is released, the led blinks once per second.

## How to use

* Clone this repository with its submodules : `git clone --recurse-submodules https://github.com/sporniket/demo-task-gpio-button-led.git 
&& cd demo-task-gpio-button-led`
* Open it in VSCode with PlatformIO plugin installed, 
* Open a PlatformIO terminal, and configure the project using esp-idf menuconfig tool : `pio run -t menuconfig` ; especially, select the target pins according to your own wiring.
* upload to your board, and push the button while observing the led.

## Dependency graph

```
|-- GpioAbstractionLayer-espressif32-espidf 
|   |-- GpioAbstractionLayer 
|-- FeedbackLed 
|   |-- AnimatedValues 
|-- GpioAbstractionLayer 
|-- InputButton 
|-- Task-espressif32-espidf 
```
