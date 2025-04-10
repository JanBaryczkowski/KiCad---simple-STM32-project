Project based on course made by Philip Salomony
Overview

A hands-on PCB design project using KiCad V6 to create a fully custom STM32-based development board, transitioning from Arduino-style prototyping to professional-grade hardware. The board integrates critical STM32 peripherals (USB, SWD, GPIOs) and follows industry best practices for schematic design, layout, and manufacturing.
Key Features

  Microcontroller: STM32F103C8T6 

    Power Supply:

        5V USB input → 3.3V LDO regulator (e.g., LD1117).

        Decoupling capacitors for noise reduction.

    Connectivity:

        USB 2.0 Full Speed (for programming/debugging).

        SWD Interface (ST-Link compatible).

        GPIO headers (breakout for sensors/actuators).

    Clock: 8MHz crystal + optional 32.768kHz RTC crystal.

    PCB Design:

        2-layer board (optimized for cost).

        Custom silkscreen (logo, pin labels).

        Mounting holes for mechanical stability.

Design Workflow (Following Course Modules)

    Schematic (KiCad V6):

        STM32 symbol creation + pinout planning (STM32CubeIDE).

        Critical circuitry: USB pull-up resistors, boot mode selection, reset circuit.

        ERC (Electrical Rules Check) and footprint assignment.

    PCB Layout:

        Component placement: Prioritize MCU, decoupling caps, and crystal.

        Route high-speed traces (USB, clock) first, followed by power planes.

        Ground pours and via stitching for EMI reduction.

    Routing & Validation:

        Signal integrity: Avoid 90° traces, minimize loops.

        Design Rule Check (DRC) against manufacturer specs (e.g., JLCPCB).

    Manufacturing Prep:

        Generate Gerber files, drill files, and BOM.

        Optional: Order assembled PCBs using KiCad’s fabrication outputs.

Software Tools

    KiCad V6 (Schematic + PCB).

    STM32CubeIDE (Pinout configuration, firmware development).

Learning Outcomes

    Transition from Arduino to custom STM32 hardware.

    Master KiCad workflow (schematic → manufacturing).

    Apply PCB best practices: decoupling, grounding, signal routing.

    Understand STM32 hardware requirements (clocking, USB, SWD).
