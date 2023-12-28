# OperaFace: Digitized Opera Face Changing Toys Based on Emotion Recognition

## Background:
Sichuan Opera Face Changing is one of the stunts used in Sichuan Opera performances, which is used to reveal the inner feelings and thoughts of the characters in the play, i.e., to turn the invisible and imperceptible abstract emotions and psychological states into visible and perceptible concrete images - face paintings. Face painting is a kind of stunt used in the art of Sichuan Opera to portray characters and reveal the inner thoughts and feelings of the characters in the play as a kind of romanticism technique.

We proposed to use facial expression recognition methods to simulate the corresponding Sichuan opera face expressions on digital led masks, to help users better understand the cultural connotations of Sichuan opera face changing and the emotional knowledge it contains; to help users better understand the emotional expression, which can be applied to children's emotional education sessions.

## Open-source Projects
open-source hardware is a hardware whose design is made publicly available so that anyone can study, modify, distribute, make, and sell the design or hardware based on that design. The hardware's source, the design from which it is made, is available in the preferred format for making modifications to it. Ideally, open-source hardware uses readily-available components and materials, standard processes, open infrastructure, unrestricted content, and open-source design tools to maximize the ability of individuals to make and use hardware. Open-source hardware gives people the freedom to control their technology while sharing knowledge and encouraging commerce through the open exchange of designs.

### Project 1: Zoning Projections
Matrials: 3D printed masks, PCBs, Pi, Raspberry Pi...
Limitations: large size, fixed, light blocking, limited resolution

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" style="width:75%;" >
</div>

### Project 2: TouchDesigner+FaceTrack
Usage: Real-time face changing through TouchDesigner's FaceTrack...
Limitations: completely dependent on computer software, less variation in the face changing effect.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" style="width:75%;" >
</div>

### Project 3: LED-integrated Board
Usage: Arduino board, RGB matrix, matrix power supply...
Limitations: rely entirely on the computer's software implementation, face changing effect is less variable

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" style="width:75%;" >
</div>

## Our Project - OperaFace
We decided to use a wearable LED mask that is already integrated in the market. The mask utilizes 2074 RBG light beads and supports Bluetooth communication to transmit facial images. In the final operation, the device can be used as an output to display the face image transmitted by the higher level system.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" style="width:75%;" >
</div>

For the software implementation, we finally selected a solution by Japanese designer Shinya Ishikawa. The scheme captures the user's facial expression in real time by invoking the camera and classifies it into different facial emotions such as happy, angry and sad.

The original scheme maps the recognized facial emotions to the robot expressions on the video stickers. In the subsequent work, we can adjust the robot expressions to the face clusters of the corresponding emotions, realizing a kind of facial interaction game; we can also call the facial emotion data recognized by the system background, match them with the emotion labels in the face database, and project the corresponding faces onto the LED screen.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" style="width:75%;" >
</div>
