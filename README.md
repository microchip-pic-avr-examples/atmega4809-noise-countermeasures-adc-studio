<a href="https://www.microchip.com" rel="nofollow"><img src="images/microchip.png" alt="MCHP" width="300"/></a>

# ATMEGA4809 Noise Countermeasures for ADC Applications

This is an example for noise countermeasures for ADC applications on the ATMEGA4809, this is a general example which is applicable to the whole megaAVR 0-series.

## Related Documentation

- [AN2551 -  Noise Countermeasures for ADC Applications ](https://www.microchip.com/wwwAppNotes/AppNotes.aspx?appnote=en600674)
- [ATmega4809 Family Product Page](https://www.microchip.com/design-centers/8-bit/avr-mcus/device-selection/atmega4809)

## Software Used

- [Atmel Studio 7.0 or newer](https://www.microchip.com/mplab/avr-support/atmel-studio-7)
- ATmega_DFP 1.4.351 or newer

## Hardware Used

- ATmega4809 Xplained Pro [(ATMEGA4809-XPRO)](https://www.microchip.com/developmenttools/ProductDetails/ATMEGA4809-XPRO)

## Setup

1. Open `NoiseCountermeasuresforADCApplicationswithmegaAVR0-series.atsln` in Atmel Studio
2. Connect the ATmega4809 Xplained Pro to your computer with a micro usb cable.
3. In your menu bar in Atmel Studio go to `Debug->Start Without Debugging` or press `CTRL + ALT + F5`
4. Open data visualizer under `Tools->Data Visualizer` to view the messages which is transmitted through UART. The baud rate is `19200`
5. Follow Appendix A in [AN2551](#Related-Documentation) for step by step instructions on how to graph the samples

## Operation

Filtered ADC values will be passed over the UART port, these can be parsed or graphed for a visual understanding of ADC value.
The ADC input is mapped to `PD5` and will change the ADC values being sent over UART depending on the voltage applied.

## Summary

We have here shown how to get started with the [AN2551 -  Noise Countermeasures for ADC Applications](#Related-Documentation) appnote. For more details about the code and theory of operation please inspect the appnote itself.