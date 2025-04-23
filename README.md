# Exno-3-Prompt-Engg

# Ex.No: 3 	Evaluation of 2024 Prompting Tools Across Diverse AI Platforms: 
ChatGPT, Claude, Bard, Cohere Command, and Meta 
### DATE:                                                                            
### REGISTER NUMBER : 
 
###Aim:
To compare the performance, user experience, and response quality of different AI platforms (ChatGPT, Claude, Bard, Cohere Command, and Meta) within a specific use case, such as summarizing text or answering technical questions. Generate a Prompt based output using different Prompting tools of 2024.

### Algorithm:
Define the Use Case:
Select a specific task for evaluation across platforms (e.g., summarizing a document, answering a technical question, or generating a creative story / Code).
Ensure the use case is applicable to all platforms and will allow for comparison across response quality, accuracy, and depth.
Create a Set of Prompts:
Prepare a uniform set of prompts that align with the chosen use case.
Each prompt should be clear and precise, ensuring that all platforms are evaluated using the same input.
Consider multiple prompts to capture the versatility of each platform in handling different aspects of the use case.
Run the Experiment on Each AI Platform:
Input the prompts into each AI tool (ChatGPT, Claude, Bard, Cohere Command, and Meta) and gather the responses.
Ensure the same conditions are applied for each platform, such as input format, time to respond, and prompt delivery.
Record response times, ease of interaction with the platform, and any technical issues encountered.
Evaluate Response Quality:
Assess each platform’s responses using the following criteria: Accuracy,Clarity,Depth,Relevance 
Compare Performance:
Compare the collected data to identify differences in performance across platforms.
Identify any platform-specific advantages, such as faster response times, more accurate answers, or more intuitive interfaces.
Deliverables:
A comparison table outlining the performance of each platform (ChatGPT, Claude, Bard, Cohere Command, and Meta) based on accuracy, clarity, depth, and relevance of responses.
A final report summarizing the findings of the experiment, including recommendations on the most suitable AI platform for different use cases based on performance and user 


### Algorithm: Design and Develop a Test scenario and execute the prompts under Diverse AI Platforms.
1.How does the alcohol sensor work in detecting alcohol content in the breath, and how is the sensor output used to trigger the engine locking system?    
 
 
CHATGPT 	CLAUDE 	GEMINI 
An alcohol sensor, commonly a MQ-3 or similar type, works on the principle of semiconductor gas sensing. It contains a sensitive material (typically tin dioxide) that changes its resistance when exposed to alcohol vapors. When a person breathes into the sensor, the ethanol in the breath reacts with the sensing material, causing a change in electrical resistance. This change is converted into an analog voltage signal proportional to the alcohol concentration. A microcontroller (like Arduino or Raspberry Pi) reads this signal, processes it, and compares it to a predefined threshold. If the detected alcohol level exceeds the legal or safe limit, the 
microcontroller triggers a relay or electronic control unit (ECU) to prevent the engine from starting. This system ensures that a driver under the influence cannot operate the vehicle, thereby enhancing road safety. Some systems may also store data or send alerts for monitoring purposes. 
 	The alcohol sensor (typically a semiconductor-based or fuel cell breathalyzer) works by detecting ethanol molecules in exhaled breath through an electrochemical reaction. When the driver breathes into the device, alcohol molecules in the breath oxidize on the sensor's surface, generating an electrical current proportional to the alcohol concentration. This analog signal is then converted to a digital value through an ADC (Analog-toDigital Converter). The system compares this measured value against a preprogrammed threshold that corresponds to the legal blood alcohol concentration limit. If the detected alcohol level exceeds this threshold, the system's microcontroller triggers a relay or electronic control unit that interrupts critical circuits in the vehicle's ignition system. This interruption can prevent the starter motor from engaging, cut power to the fuel pump, or disable the engine control module, effectively preventing the vehicle from starting. 
 	The alcohol sensor, typically a 
semiconductor or electrochemical device, quantifies breath alcohol content through a chemical interaction. When alcohol molecules in exhaled air come into contact with the sensor's active material (like tin dioxide or a catalytic electrode), it triggers a measurable change in the sensor's electrical characteristics. For instance, semiconductor sensors exhibit a decrease in electrical resistance proportional to the alcohol concentration, while electrochemical sensors generate a voltage or current. This mechanism usually involves an electromechanical relay or a similar switching device integrated into the vehicle's starting circuit or fuel supply system. Upon receiving the signal, the relay activates, interrupting the flow of electricity to the starter motor or blocking the fuel line, thereby effectively preventing the vehicle's engine from being started or causing it to stall if already running. 
 
2.What are the key components used in the engine locking system, and how do you ensure that the locking mechanism is reliable and secure when triggered by alcohol detection?    
 
 
 
CHATGPT 	CLAUDE 	GEMINI 
The key components used in the engine locking system include an alcohol sensor (e.g., MQ-3), a microcontroller 
(such as Arduino or Raspberry Pi), a relay module, and the vehicle’s ignition system interface. When the sensor detects alcohol above the set threshold, the microcontroller processes the data and activates the relay to cut off the ignition or fuel supply, effectively locking the engine. To ensure the locking mechanism is reliable and secure, the system uses realtime monitoring, calibrated sensors, and fail-safe programming to avoid false triggers. The relay is chosen based on its current and voltage ratings to handle the ignition circuit safely. Additionally, the wiring and connections are well-insulated and secured to prevent tampering. For enhanced security, the system can include authentication methods like RFID or biometric verification before engine start, ensuring only authorized and sober individuals can operate the vehicle. 
 	The key components of an engine locking system include the alcohol sensor (typically MQ-3 or fuel cell-based), a microcontroller for processing sensor data, an analog-todigital converter, a relay circuit for interrupting the ignition, and an electronic control unit that interfaces with the vehicle's systems. Reliability and security are ensured through redundant sensing mechanisms, tamper-evident 
seals, encrypted communication between components, regular calibration routines, backup power supplies, and comprehensive self-diagnostic procedures that identify system faults. The system typically incorporates data logging capabilities to record usage patterns and attempts to circumvent the mechanism, while physical design elements like specialized connectors and mounting hardware prevent unauthorized removal.  	The key components of an engine locking system triggered by alcohol detection typically include a relay or solenoid switch to interrupt the engine's electrical circuit (ignition or fuel pump), a microcontroller to process the sensor signal and activate the locking mechanism, and the necessary wiring and power supply to connect these components. To ensure reliability and security, several measures are crucial. Firstly, the alcohol sensor should be highly accurate and calibrated to minimize false positives or negatives. Secondly, the microcontroller's decisionmaking logic should be robust and tamper-proof, preventing easy circumvention of the system. Thirdly, the electrical connection to the engine locking mechanism must be secure and protected against manipulation or accidental disconnection. Finally, incorporating redundancy or fail-safe mechanisms can enhance reliability,  even in case of minor component failures. 
 
 
 
3.What type of microcontroller would be suitable for this project, and how would you implement the logic for detecting alcohol levels and triggering the engine lock under different conditions?    
CHATGPT 	CLAUDE 	GEMINI 
A suitable microcontroller for this project would be an Arduino Uno due to its simplicity, affordability, and sufficient I/O pins for sensor and relay integration. It can read analog signals from the MQ-3 alcohol sensor, process them, and control the relay module to lock the engine. The logic implementation involves continuously reading the analog voltage from the sensor and comparing it to a predefined threshold value representing the maximum safe alcohol level. If the reading exceeds the threshold, the microcontroller sends a HIGH signal to the relay, cutting off the ignition circuit. For better accuracy, the system can average multiple readings and apply software debouncing to avoid false positives. Additional logic can include time delays, alerts via LEDs or buzzers, and conditional checks to allow engine start only when alcohol levels return to safe values. For advanced control, the setup can be expanded with a display module and data logging features. 	An Arduino Nano or ESP32 microcontroller would be ideal for this project due to their compact size, low power consumption, adequate processing power, and built-in ADC capabilities. The implementation logic would involve reading analog values from the MQ-3 alcohol sensor, applying a calibration formula to convert raw readings to BAC (Blood Alcohol Concentration) equivalent, and comparing against legal thresholds 
(typically 0.08% in the US). The microcontroller would employ a state machine architecture with conditions for normal operation, warning levels (0.05-0.07%), and lockout (>0.08%), with hysteresis to prevent rapid oscillation around threshold values. Timebased constraints would ensure sustained readings above threshold for 3-5 seconds to avoid false positives from environmental factors. When alcohol detection triggers a lockout, the microcontroller would activate 
a relay to interrupt the vehicle's ignition circuit, requiring a supervised reset procedure after a mandatory timeout period of 15-30 minutes. 	A low-power, cost-effective microcontroller like the Arduino Uno or Nano, or a PIC microcontroller (e.g., PIC16F series) would be suitable for this project due to their sufficient processing power, analog-to-digital converter (ADC) for reading the alcohol sensor output, and digital I/O pins for controlling the engine lock relay. The logic would involve reading the analog voltage from the alcohol sensor using the ADC and converting it to a digital value. This value would then be compared against predefined thresholds stored in the microcontroller's memory. For example, a single threshold could trigger the immediate engine lock. More complex logic could involve multiple thresholds for warning levels or a delay before locking. The microcontroller program would continuously monitor the sensor, execute the comparison logic, and activate the relay connected to the engine lock when the alcohol level exceeds the set limit. 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
Conclusion:    
ChatGPT, Claude, and Gemini each excel in different areas: ChatGPT is known for its conversational abilities and broad knowledge, Claude offers strong capabilities in natural language understanding and reasoning, while Gemini specializes in deep research and data analysis. Each platform caters to unique user needs based on task complexity and specialization. Ultimately, the best choice depends on the specific use case and desired outcome.    
 























### Result:
Thus the Prompting tools are executed and analysed sucessfully .

