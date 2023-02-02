# Demonstration of Tasks, Gpio, InputButton and Led libraries

C++ project for PlatformIO, that demonstrate some libraries that I wrote.

This sample project consists of a blinking led and a push button. When the button is pushed, the led blinks three times per second, when the button is released, the led blinks once per second.

## How to use

Clone this repository with its submodules, open it in VSCode with PlatformIO plugin installed, configure, upload.

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

The repository of each library :

* AnimatedValues : https://github.com/sporniket/AnimatedValues
* FeedbackLed : https://github.com/sporniket/FeedbackLed
* GpioAbstractionLayer : https://github.com/sporniket/GpioAbstractionLayer
* GpioAbstractionLayer-espressif32-espidf : https://github.com/sporniket/GpioAbstractionLayer-espressif32-espidf
* InputButton : https://github.com/sporniket/InputButton
* Task-espressif32-espidf : https://github.com/sporniket/Task-espressif32-espidf

