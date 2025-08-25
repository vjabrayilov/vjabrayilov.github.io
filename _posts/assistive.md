---
layout: distill
title: "Assistive System for Visually Impaired People"
description: A blog post about our group project submitted to national conference during my bachelor's degree
tags: arduino opencv tensorflow robotics raspberry-pi
# categories: blog
date: 2021-03-01
featured: false

authors:
  - name: Mujgan Huseynli
    url: "https://mujganhuseynli.github.io"
    # affiliations:
    #   name: EE, George Washington University
toc:
  - name: Introduction
  - name: Harnessing the Power of Technology
  - name: Seamless Integration and User-Friendly Interface
  - name: Energy Efficiency and Sustainability
  - name: Real-World Impact and Future Prospects
---

[Click here to download the PDF for submission.](/assets/pdf/assistive.pdf)

# Revolutionizing Mobility for the Visually Impaired: A Deep Dive into Advanced Assistive Systems

In a world where mobility is often taken for granted, visually impaired individuals face unique challenges that can hinder their ability to navigate environments safely and independently. However, groundbreaking technological advancements are setting the stage for a new era of accessibility. We developed this project as a team during my bachelor's degree at Baku Higher Oil School, Azerbaijan, using a combination of IoT hardware and software technologies to create a safer, more navigable world for those with visual impairments.

<div style="text-align: center;">
<img style="width: 80%;" src="/assets/img/assistive/gen.png"/>
</div>

### Harnessing the Power of Technology

The core of this innovative system is built on two key modules: the shoe module and the box module, each equipped with cutting-edge technology tailored to meet the needs of visually impaired users.

#### The Shoe Module

The shoe module is a marvel of engineering, incorporating a variety of sensors and devices to ensure user safety. Key components include:

- **Arduino Nano**: Serves as the microcontroller, managing all the module's operations.
- **Ultrasonic Sensors**: These are crucial for detecting obstacles, whether on the side or directly in front of the user, providing real-time feedback to avoid collisions.
- **Vibrating Motors**: Positioned to correspond with the location of detected obstacles, these motors provide tactile alerts to the user, guiding their movement.
- **Water Level Sensor**: Enhances navigation during adverse weather conditions by detecting puddles and alerting the user to potential slip hazards.
<div style="text-align: center;">
<img style="width: 80%;" src="/assets/img/assistive/shoe.png"/>
</div>

#### The Box Module

The box module works in tandem with the shoe module to refine the system's responsiveness and accuracy. It includes:

- **Raspberry Pi 4 Model B**: This powerful single-board computer handles complex image processing tasks, ensuring the system can identify and classify various obstacles.
- **Camera and Bluetooth USB Dongle**: These components are vital for object detection and data transmission, respectively, allowing the system to adapt and respond to dynamic environments.
<div style="text-align: center;">
<img style="width: 80%;" src="/assets/img/assistive/hand.png"/>
</div>

### Seamless Integration and User-Friendly Interface

To make the system as user-friendly as possible, it includes voice command capabilities through the Google Speech-to-Text API, allowing users to operate the system hands-free. This feature is crucial for enhancing the accessibility and ease of use of the technology.

### Energy Efficiency and Sustainability

A standout feature of this system is its energy efficiency. The shoe is designed to harvest energy from walking via a piezoelectric transducer, which converts mechanical energy into electrical energy, providing a sustainable power source for the system.

### Real-World Impact and Future Prospects

This assistive system represents a significant advancement in assistive technology for the visually impaired. It not only increases the independence and safety of its users but also integrates seamlessly into their daily lives, providing a level of intuitiveness and ease that was previously unattainable.

As technology continues to evolve, future enhancements could include more precise image processing capabilities and the integration of AI to detect undefined potential obstacles, further enhancing the effectiveness of the system.

This assistive system is more than just a technological innovation; it is a beacon of hope, opening up new pathways for independence and safety for visually impaired individuals around the world.
