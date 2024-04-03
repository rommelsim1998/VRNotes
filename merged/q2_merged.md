# Interaction
[Discussion Link](https://github.com/orgs/sit-dia/discussions/14)

## Viewpoint Control
- Basically controlling the camera
- Is a **passive** interaction
- Inertial Measurement Units (IMUs) use accelerometers and gyroscopes to determine where a device is in 3D space
> - Viewpoint control in VR typically involves the following aspects:
> -Positional Tracking: VR systems often use sensors or cameras to track the user's head movements in real-time, allowing them to change their position within the > -virtual environment by moving their head. This enables users to look around and explore the virtual world from different angles.

> - Orientation Control: Users can also rotate their viewpoint by turning their head or using input devices such as controllers to change their orientation within the virtual environment. This allows them to view the surroundings from different perspectives.

> - Teleportation or Locomotion: In addition to natural movement, VR applications may offer alternative methods of navigation such as teleportation or simulated > -walking. These techniques allow users to move to different locations within the virtual space, expanding their ability to explore and interact with the > -> -environment.

> - Scale and Proximity Control: Some VR experiences allow users to dynamically adjust their scale within the virtual environment or manipulate their proximity to objects. This feature can be useful for examining details, interacting with objects, or adapting the environment to fit personal preferences.

## Hand Gestures
- Haptic Gloves
- Computer Vision-based Finger Tracking
- Dedicated VR controllers

## Body Gestures
- Embodiment: "the feeling of being in control of a virtual representation of the human self"
> - Perception that a virtual body is one's own. Often correlated to Presence
- Hand gestures are partial embodiment, because only the hands are being controlled
- IMU Trackers
- 360 degree treadmills
- Haptic suits
- No real desktop replacement using desktop modalities (e.g. keyboard, mouse) to give embodiment

## Interaction Authenticity
- Interaction Authenticity: "the consideration of whether the desired experience should be natural or artificial"

### Natural Interactions
- Natural Interactions: "interactions where the outcome is very close to what is done in the real world"
> - Natural interaction offers the most optimal interaction authenticity

### Artificial Interactions
- Artificial Interactions: "interactions that are impossible in the real world"

#### Magical Interactions
- Plausibility Illusion: "events that happen in the virtual world closely affects the perception of how credible these things can actually happen IRL"
- Having the Plausibility Illusion is the key to providing an immersive experience for the user
- E.g literally controlling the flow of time by moving (Superhot)

#### Augmented Natural Interactions
- Allows users to perform highly exaggerated versions of a familiar IRL action
- E.g. super high jumps in video games

## Interaction Use Cases

### GUI Interactions
- GUI = Graphical User Interface
- HUD = Heads Up Display
- HMD = Head Mounted Device

#### E.g. Meta Quest 2
-  An "all-in=one" VR HMD, where all selections and menu interactions are displayed in the VR display itself
- It uses Viewpoint Control & Hand Gestures 
- Creates a laser pointer ray, acting as an extension of the VR controllers, to click options in the menu with a trigger button

#### E.g. Google Cardboard
- Makes finger point at things by using Viewpoint Control, known as Gaze Control (because there are no controllers)
- Clicks in menus are done by staring at menu options long enough [Editor's Note: THAT'S HILARIOUS.]

### Locomotion Interactions
- Locomotion Interactions: "the ability to perform spatial navigation in the virtual environment"
- Can be pretty tricky to get right, especially with IRL spatial constraints (the room you're in can only be so big before bumping into stuff)
- Can be done by combining Viewpoint Control, Hand Gestures and Body Gestures
- Alternatively, users can move around with just teleporting from place to place instead, but that hampers Immersion a lot

# End  

Link: [Developing Immersive Applications: Interaction (youtube.com)](https://www.youtube.com/watch?v=dKRWH7O81yk)
> Written with [StackEdit](https://stackedit.io/).

# Implementing Interaction
[Discussion Link](https://github.com/orgs/sit-dia/discussions/17)

## Video/Stream Outline
01. Intro
02. Refactoring code
03. NPM run and serve scripts
04. Component-based architecture to structure code
05. Cleaning up d.ts files
06. Refactoring text plane into a component class
07. Preparing the Scene
08. Creating another component to manage meshes
09. Titbits on javascript interfaces, etc...
10. Overview of different methods to implement interactions
11. Using behaviors to implement interaction
12. Using actions to create behaviors
13. Using keyboard actions
14. Using observables to implement interactions
15. Implementing teleportation locomotion
16. Using more observables
17. Creating custom observer
18. Using coroutines
19. Implementing locomotion
20. Implementing teleportation locomotion
21. Implementing WIP locomotion
22. Implementing hand tracking
23. Implementing bimanual interaction
24. Implementing gizmos
25. Implementing natural grabbing

## Behaviors
- Predefined, reusable interactions w/o needing to customize
- Ex. Dragging, Scaling, Following, etc

## ActionManager
- Property changes triggered by pre-defined events
- Customizable interaction parameters 
    - Ex. Duration, Conditions, Triggers

## Observables
- General Code Construct for observer pattern
- Subscribe and receive notifications to events
- Fully customizable interactions

## Gizmo Manager
- Uses Gizmo to easily manipulate position, rotation and scale

# End  

# Interaction
[Discussion Link](https://github.com/orgs/sit-dia/discussions/19)

# Interaction
[Discussion Link](https://github.com/orgs/sit-dia/discussions/20)

Guest Speaker

Likelihood for tested in exam: Low

# Interaction
[Discussion Link](https://github.com/orgs/sit-dia/discussions/21)

Guest Speaker

Likelihood for tested in exam: Low

# Finals review

---

## Interaction
[Discussion Link](https://github.com/orgs/sit-dia/discussions/24)

- Differentiate AR,VR,MR and XR
> - AR overlays digital information or virtual objects onto the real world, where users are still able to see and interact with their physical surroundings while additional digital content is integrated into their environment
> - VR immerses users into a completely simulated environment, shutting out the physical world
> - Mixed Reality (MR) combines elements of both AR and VR. Blending digital content with the real world while maintaining interaction between the 2. MR systems are capable of understanding and responding to the user's physical environment in real time.
> - Extended Reality (XR) is an umbrella term that encompasses all immersive technologies. Including AR, VR, MR.

- explain milgram and kishino's Reality-Virtuality Continuum
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/30e1b6fc-d5c6-4c5f-8ce7-e00be7fe6362)
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/7a277687-b461-4ad9-838d-29a3de9f2241)
> - ```EWK``` refers to the familiarity and understanding that users have of the environment they are interacting with. 
> - ```Immersion``` refers to the degree to which users feel mentally and emotionally absorbed in a virtual environment, as if they're physically present within it.

- reproduction fidelity
>- Refers to how accurately and realistically the virtual environment reproduces real-world elements. Such as visual, audio and interaction fidelity.
>- Visual fidelity: quality and realism of graphics and visual effects in VR
>- Audio fidelity: accuracy and realism of spatial audio, including the positioning and behavior of sound sources
>- Interaction fidelity: concerns the realism and responsiveness of object interactions within the virtual environment.
  
- Extent of presence metaphor
>- Refers to the degree to which users feel present and engaged within the virtual environment. The feeling of "being there" immersed in the virtual world.

- Coherence
> - Refers to the Consistency and Believability of the virtual environment
> - For a moment I believed that i was actually 1000ft above ground.
> - Things are described from the user's perspective

- Affordance
> Refers to the perceived possibilities for action or interaction within the virtual environment. It influences how users intrinsically interact with objects and navigate the virtual space
> Improving affordance:
>> - Hand tracking that allows natural manipulation of objects
>> - Having objects with clear grooves for gripping
>> - Haptic feedback when an object correctly fits into place
>> - Highlighting interactive objects with subtle glow effects

- Embodiment
> perception that a virtual body is one's own. Often correlated to Presence. 
>> Improve tracking fidelity, implement multimodal sensory feedback: visual, auditory, haptic, implement personalization (meta mirror)

- Q: explain immersion as system properties
>- Example of factors describing immersion from a systems perspective
>> - Wide FOV
>> - 8K resolution display
>> - 6-DOF inside out tracking

- explain immersion as user experience
![image](https://github.com/Taterr/VRNotes/assets/90663945/2b40b70f-f1a6-4b2e-a709-7844f822f685)

- explain the key dimensions of presence, flow, cybersickness
- ```cybersickness```
> - Caused when a mismatch between the visual information received by the brain through the VR headset and the body's vestibular system, which senses motion and balance.
> - To mitigate cybersickness given poor motion tracking fidelity, we can __constrict the FOV when moving, and use teleportation locomotion. best is to use real walking but might have space constraints__
> - General cybersickness mitigation include: Optimize FPS and reduce latency lag, reduce motion intensity, use HTC Vive trackers.
> - Quantified using VRSQ (Virtual Reality Sickness Questionnaire)

- ```Flow```
> - "in the zone", a psychological state characterized by deep focus, intense concentration, and a sense of enjoyment in the activity. It occurs when individuals are fully engaged and absorbed in a task, to the point where they lose track of time and become completely immersed in the experience, bringing about effortless control and enjoyment.
> - To improve flow, __increase the difficulty of the game so that its challenging as the player progresses, and providing clear goals and feedback__
> - Quantified using FSS (Flow State Scale)

- ```Presence```
> - "being there", "being present" as if the virtual environment is perceived as real and the user feels a sense of spatial presence and immersion. Presence is influenced by factors such as sensory fidelity, interactivity, realism, and user engagement. The more convincing and immersive the virtual environment, the stronger the sense of presence.
> - Quantified using IPQ (Igroup Presence Questionnaire)
  
- describe how to employ different quantitative and qualitative user research methods to evaluate presence, flow and cybersickness

- ![image](https://github.com/Taterr/VRNotes/assets/90663945/29c5bb79-301e-4d91-a23e-d74fe37bb0b8)

--- 

## Development tools
- Describe common tools for developing immersive applications
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/d870046f-5b53-4501-89c6-8de580eac512)

- Differentiate the accessibility implications of choosing different types of tools
  
- Differentiate WebXR and OpenXR standards
> - **WebXR** is a standard for creating immersive experiences on the web, allowing developers to build VR and AR applications that can be accessed and experienced directly through web browsers without the need for additional plugins or software ```A-Frame, Babylon.js, Three.js```
> - **OpenXR** is a standard developed by Khronos, for building cross-platform VR and AR applications that are able to run on multiple hardware devices such as VR headsets, AR glasses, MR devices. ```Unity3D, Unreal Engine, OpenXR SDK```

## Hardware and Software Components
- Describe common hardware components in XR devices
> ![image](https://github.com/Taterr/VRNotes/assets/90663945/2a8d5a4b-9b85-4c31-aa14-419f4038040d)

- Explain the image formation process in typical XR HMDs
> ![image](https://github.com/Taterr/VRNotes/assets/90663945/bc810af6-80ec-44d1-8aab-222cb915daad)
> ![image](https://github.com/Taterr/VRNotes/assets/90663945/0ecb4854-3079-474e-b471-3369a506e8c1)
> ![image](https://github.com/Taterr/VRNotes/assets/90663945/7cdd568e-9c35-4ad2-8d03-c527328668cb)

- Describe common software components in immersive applications
>- What is the function of the **debug layer** in the scene class of **Babylon.js**?
>> allows the developer to visualize important scene information such as the positions, rotations, and bounding boxes of the mesh objects within the scene. The debug layer can also provide tools for monitoring and analyzing the performance of the scene, including fps, memory usage and draw calls.
>- **PhotoDome** class in babylonjs: used to display a 360 degree panoramic image within a 3D scene. allowing developers to create immersive environments by wrapping the panoramic image around a sphere, enabling users to explore the scene from any angle.
  
- Describe the architecture of a typical WebXR application
> ![image](https://github.com/Taterr/VRNotes/assets/90663945/fdb0fb24-364b-41dc-8775-a918f05791ce)
>> What is the order of the console logs in this Babylon.js code? (2,3,4,1)

## Model-based approach
> Hand made 3D models using 3D modelling tools. Requires deep technical art expertise. Enables full interactive interactions
> **pros:** High fidelity, Customization, Interactivity, Realism in terms of level of details.
> **cons:** Complexity, Performance overhead, File size

## Image-based approach
> 360 photos / videos. More accessible to untrained creators, limited to static surroundings.
> **pros:** Ease of implementation, Performance efficiency, Realism in terms of its closeness with real world visual cues (lighting, shadows, perspective)
> **cons:** Limited interactivity, Dependency on Environment (relies on scanning real world images), Quality of capture


## Interaction
- Viewpoint Control
> - Top priority. Helps to give a sense of presence
> - Passive interaction: Not done consciously

- Hand Gestures
  
- Body Gestures

## Implementing Interaction
- ```ActionManager```
> - Consists of a collection of actions, each representing a specific behavior of action that should occur when triggered. Customize interaction parameters (duration, conditions, triggers)
> - For example: an action action may be triggered when a user clicks on a mesh object, when 2 objects collide, or when a certain condition is met.

- ```Observables (Source)```
> Holds the state and notifies its observers when its state has been changed. It is responsible for managing and notifying its list of observers
> - Used in event driven programming paradigms such as GUIs, where UI elements (observables) notify listeners (observers) of user interactions or state changes.

- ```Observers```
> An object that subscribes to an Observable and receives notifications when the Observable's state changes. It defines a callback or handler function that is invoked by the Observable when conditions are met.
> - Used where objects need to react to changes in the state of other objects without being tightly coupled to them.
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/f920e303-85e4-4b9e-b3c8-5b63c39fae6e)
>> - How many observers were used here (1)
>> - In total, how many observables did we operate on? (1)
>> - In total, how many observables did we create? (0)

- ```Pointer Drag Behavior```
> The ability to interactively drag and move objects within a 3D scene using mouse or touch inputs
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/49751331-3a03-46e9-921c-6d87d778b03c)
>> The following code allows the sphere to be dragged around a plane perpendicular to the direction the player is viewing
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/5497d40e-ece1-4423-bd74-9bda68f115a4)
>> Can you suggest an improvement to the "debug code" to get the position of the sphere only when it is being dragged? (add observer to the onDragObservable of pointerDragBehavior to get position)

- ```Movement```
> - ![image](https://github.com/Taterr/VRNotes/assets/90663945/c55cce4a-bdd4-4338-86a2-215c8d4cc1c7)
>> What happens when I change "timeToTeleport" to 0 in the following babylonjs code? (Teleportation triggers immediately when the button is pressed)

## Case Studies
