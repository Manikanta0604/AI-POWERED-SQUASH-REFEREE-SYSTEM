# AI-POWERED-SQUASH-REFEREE-SYSTEM
Introduction: AI-Powered Squash Referee System is a personal project which I created to automate and enhance the process of refereeing squash matches and test emerging technologies like OpenCV and Deep Learning. Traditionally, squash is intrinsically a judgement-based game and, mistakes happen, especially in fast-paced games where instant decision-making is vital. This project intends to design a system that generates detailed analysis of matches, detecting critical events accurately in a timely fashion, providing near real-time feedback on infractions for let calls, strokes, and faults. By applying computer vision methods of tracking the ball and players' movement, the system is able to detect key actions in a game. The structured data captured in this process provides a basis to train deep learning models on labeled match footage where the model can automatically predict specific scenarios, such as the "in" or "out" state of a player hitting the ball, when the player faults or when a let is called. The squash AI referee marks a new era for players around the world, as it drastically minimizes error from a human standpoint, but also brings a level of fairness and consistency to each match. The algorithm was analyzed under real match conditions to verify its accuracy, and constantly improved according to performance data and feedback. Furthermore, by automating the refereeing decision-making process, this project illustrates the practicality of implementing AI and computer vision in the sports domain, paving the way for further innovations in the refereeing process for future sports events.  
Rules of the Game: A serve must be hit from within the service box and land in the opposite corner of the court; a game is usually played to 11 points, with a two-point advantage needed to win; players are free to move around the court but cannot obstruct the movement of other players; the goal of squash is to hit the ball against the front wall, above the "tin" (low line), and below the "outline" by taking turns with your opponent, making sure the ball bounces only once on the floor before hitting the front wall again. Before the ball bounces on the floor, it must strike the front wall above the tin and below the outline. When striking the ball, the server must have at least one foot in the service box, and the serve must fall in the court's diagonally opposite corner. Before striking the front wall once more, the ball can only bounce once on the floor. The ball is deemed out if it strikes the floor, the tin, or any outline before striking the front wall. It is forbidden for players to purposefully block their opponent's path to the ball. A "let" may be called and the rally is replayed if an opponent unintentionally blocks a player. A player must win by two points in a game that is played to eleven points. 
Objective: The goal of squash is to hit the ball so that the opponent cannot return it within the rules. Points are scored by making the ball bounce twice before the opponent can return it. Players: In singles or doubles, squash is usually played between two or four players. Court: A typical squash court has a floor, two side walls, a front wall, and a back wall. It is rectangular in shape. Lines delineate the receiving area, the serve, the "tin" (bottom boundary), and the "service box." Serving: The service line is a 48-cm strip at the bottom of the front wall, 3 feet above the tin. The 1.6 m × 1.6 m service box is situated close to the side walls and behind the short line.  
Rally: Players take turns striking the ball after the serve until one of them either smashes the ball outside the bounds or is unable to return it. Before the ball bounces on the floor, it must strike the front wall between the outline and the tin. It must stay inside the court's bounds, but it may strike the sidewalls. 
Score: Rally scoring allows both players to score points regardless of who is serving, while standard hand-inhand-out allows only the server to get points. A player must win by at least two points in a match that is usually played to 11 or 15 points. 
Winning a Point: The opponent fails to return the ball before it bounces twice. The opponent hits the ball outside the court boundaries (tin or above the outline). The opponent fails to hit the ball before it bounces on their side of the court. 
Let and Faults: A let occurs when the rally is stopped for some reason (e.g., interference or confusion in shot selection), and the point is replayed. A fault occurs if the server breaks a serving rule (e.g., stepping out of the service box or hitting the ball incorrectly). Two faults result in the loss of the serve. 
Winning the Game: The match is won when a player wins a set (usually 11 or 15 points, depending on the rules) and wins a pre-determined number of sets (typically 3 or 5). Functional Requirements:  
Ball Tracking: The system should be able to accurately track the position and movement of the ball throughout the match. It should handle various ball speeds and trajectories, including fast-paced shots and unpredictable bounces. 
Player Movement Detection: The system must detect and track player movements, including positioning on the court and interactions with the ball. It should distinguish between players, identify their positions, and track their actions during rallies. 
Violation Detection: The system should automatically identify common violations such as faults (e.g., serving faults) and lets (e.g., interference between players). It should detect whether the ball lands in or out of bounds with high accuracy, considering the court’s layout. 
Real-Time Decision Making: The system should provide real-time feedback on decisions, such as scoring updates or violation calls, within seconds of the event occurring. It must generate appropriate rule-based decisions (e.g., "Let", "Fault", or "In/Out"). 
Match Event Logging: The system should log all match events, including the start and end times of rallies, scores, and violations. It should provide a history of decisions for review purposes. 
User Interface (UI): A graphical user interface (GUI) should display real-time match data, such as score updates, time tracking, and detected violations. The interface should allow users (e.g., referees, players, or coaches) to interact with the system for adjustments or review of match events. 
Training and Evaluation: The system should allow for continuous learning, enabling the deep learning model to improve accuracy over time based on new match footage. The model should be evaluated against labeled match footage to ensure performance accuracy and system reliability. 
Non-Functional Requirements 
Performance: The system should be capable of processing high-resolution video footage in real-time without noticeable lag. It should handle high-frame-rate video streams (e.g., 30 FPS or higher) and provide timely decision-making. 
Scalability: The system should be able to scale for different match environments, handling various court sizes, lighting conditions, and camera angles. 
Accuracy: The model should achieve a high level of accuracy in detecting ball positions, player movements, and rule violations, with minimal false positives or negatives. 
Reliability: The system should operate without crashes or errors during long-duration matches, ensuring continuous operation from start to finish. high
Portability: The system should be portable enough to run on different hardware setups, such as       performance computers, laptops, or cloud environments. 
Security and Privacy: If match footage involves sensitive data or player interactions, the system should adhere to appropriate security standards, ensuring data protection and privacy. 
Usability: The user interface should be intuitive and easy to use for referees, players, or coaches with varying technical expertise. 
Technical Requirements 
Hardware: Cameras: High-definition cameras capable of capturing the entire squash court with a wide-angle view for accurate tracking. Processing Unit: A powerful GPU or CPU for real-time image processing and deep 
learning inference. 
Software 
Programming Languages: Python for deep learning, OpenCV for computer vision, and other relevant libraries 
for data processing. 
Deep Learning Framework: TensorFlow or PyTorch for model training and evaluation. 
Video Processing Tools: OpenCV and other libraries for video capture, manipulation, and analysis. 
Constraints 
Environmental Conditions : The system must work in varying light conditions (e.g., indoor courts with artificial lighting or outdoor courts). The system must work with diverse video qualities (e.g., different camera resolutions, frame rates, and angles). 
Real-Time Constraints: The system must provide decisions in real time without causing delays in the match. The processing speed should be optimized to handle live matches without noticeable latency. 
Technologies Used 
The system integrates a combination of computer vision, deep learning, and real-time video processing technologies to automate squash refereeing. Below is a categorized list of the key technologies used: 
Programming Languages 
Python – The primary language due to its vast ecosystem of AI, machine learning, and computer vision 
libraries. 
Deep Learning & Machine Learning 
TensorFlow / PyTorch – For training deep learning models to detect rule violations, track ball movement, 
and analyze player actions. 
Scikit-learn – For traditional machine learning tasks, such as clustering player movement patterns or 
anomaly detection. 
Computer Vision & Image Processing 
OpenCV – Used for ball tracking, player detection, and frame-by-frame match analysis. 
MediaPipe – For pose estimation and skeletal tracking of players to analyze movement. 
Pillow (PIL) – For handling image data and frame manipulation. 
albumentations – For image augmentation to enhance training datasets. 
Video Processing & Analysis: 
FFmpeg – For handling different video formats, frame extraction, and video pre-processing. 
MoviePy – For extracting relevant sections of match videos and overlaying decision data. 
ImageIO – For reading and writing image frames from video footage. 
Data Processing & Storage 
NumPy & Pandas – For handling numerical data, match event logs, and performance analytics.  
Dask – For large-scale, parallelized data processing. 
PyArrow – Efficient data serialization and storage optimization. 
SQLite / SQLAlchemy – For storing match logs and historical data. 
Real-Time Processing & Streaming 
Apache Spark / PySpark – If large-scale, real-time processing of match data is required. 
Kafka – For handling streaming video data efficiently. 
ZeroMQ – Lightweight messaging system for real-time data transfer between modules. 
Visualization & User Interface 
Matplotlib & Seaborn – For visualizing ball trajectories, player movement heatmaps, and rule violation 
patterns. 
Plotly / Bokeh – For interactive dashboards and match performance analytics. 
Tkinter / PyQt – For building a GUI to display real-time referee decisions and match statistics. 
System Architecture 
The system follows a modular architecture with key components: 
Video Processing Module: Handles video capture and preprocessing. 
Object Detection Module: Tracks the squash ball and players. 
Rule Violation Detection Module: Applies squash rules and AI-based decision-making. 
Visualization & Output Module: Displays live decisions on the video feed. 
Components Breakdown 
Video Processing Module 
Input: Squash match video footage (MP4, live feed). 
Processing: 
OpenCV reads and preprocesses frames. 
Frames converted to HSV format for ball tracking. 
Frames converted to RGB format for player detection. 
Output: Processed frames passed to detection modules. 
Object Detection Module 
Ball Tracking: 
Uses color thresholding (HSV) to detect the squash ball. 
Applies contour detection to extract ball position. 
Player Detection: 
Uses MediaPipe Pose Estimation to detect player movements.Rule-based logic (basic checks): 
Ball out-of-bounds detection. 
Player interference (distance-based check). 
Deep learning model: 
Trained on squash violations (Let, Stroke, Fault).  
Predicts violations using CNN/LSTM model (pre-trained). 
Visualization & Output Module 
Displays decision: Real-time overlay on match video
