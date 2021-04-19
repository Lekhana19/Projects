# Third Eye Project

## Overview
The "Third Eye" project is designed to enhance the mobility and safety of visually impaired individuals, providing a modern alternative to the traditional white cane and guide dogs, which can be costly. This project aims to develop affordable, efficient, and technologically advanced solutions to help users navigate with greater ease, speed, and confidence.

## Components
The Third Eye system comprises several smart wearable devices:

### Smart Cap
- **Functionality**: Navigates through traffic by reading and vocalizing traffic signboards.
- **Technology**: Equipped with a camera for real-time video capture, the cap analyzes traffic signs and provides audio instructions to the user.

### Smart Glove
- **Functionality**: Detects nearby obstacles and alerts the user through vibrations.
- **Technology**: Embedded with Ultrasonic sensors to monitor the proximity of objects and ensure safe navigation.

### Smart Body Module
- **Functionality**: Provides comprehensive obstacle detection around the user’s body.
- **Components**:
  - **Shoulder Modules**: Two modules located on each shoulder to detect upper body obstacles.
  - **Knee Modules**: Two modules placed near the knees to detect lower body obstacles.

## Traffic Signs Detection
The traffic signs detection feature uses a sign lookup matrix to interpret simple traffic directives from visual inputs. Here's how the system recognizes specific traffic signs:

```python
SIGNS_LOOKUP = {
    (1, 0, 0, 1): 'Turn Right',
    (0, 0, 1, 1): 'Turn Left',
    (0, 1, 0, 1): 'Move Straight',
    (1, 0, 1, 1): 'Turn Back',
}
