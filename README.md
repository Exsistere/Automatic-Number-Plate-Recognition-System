

Traffic control and vehicle owner identification has become major problems in every country. Sometimes it becomes difficult to identify vehicle owner who violates traffic rules and drives too fast. Therefore, it is not possible to catch and punish those kinds of people because the traffic personal might not be able to retrieve vehicle number from the moving vehicle because of the speed of the vehicle. Therefore, there is a need to develop Automatic Number Plate Recognition (ANPR) system as a one of the solutions to this problem. This project presents an Automatic Number Plate Recognition (ANPR) system developed using the Object Detection API and EasyOCR for number plate extraction. The ANPR system can detect and recognizing vehicle license plates from input images, providing a valuable tool for various applications such as traffic monitoring, law enforcement, and parking management. The system leverages the power of deep learning models from the Object Detection API for accurate vehicle and number plate detection, and EasyOCR for optical character recognition to extract the license plate number. To enhance accessibility and user interaction, the ANPR system has been deployed on Streamlit, a popular open-source app framework for Machine Learning and Data Science projects. This deployment allows users to easily utilize the system through a web-based interface, making the ANPR system more practical and user-friendly. The system demonstrates promising results in terms of both detection and recognition accuracy, showcasing the effectiveness of combining object detection and optical character recognition technologies for ANPR. Future work may involve further optimizing the system for real-time processing and expanding its capabilities to handle a wider variety of license plate formats.





![image](https://github.com/user-attachments/assets/1efb89e5-a671-4880-aba6-5d6774b811af)

![image](https://github.com/user-attachments/assets/67fb48b1-98d9-45c4-a204-4011d7aff586)



1.	Introduction


Automatic Number Plate Recognition (ANPR) is a sophisticated technology that employs pattern recognition to effectively 'read' vehicle number plates. In simple terms, ANPR cameras capture digital images of passing vehicles' number plates. These images are then processed by a computer system to extract details about the respective vehicles. ANPR systems typically comprise cameras connected to a computer, and the captured digital images are converted into data for analysis.

Our proposed method primarily relies on edge detection, Optical Character Recognition (OCR) operations, and the identification of rectangles in vehicle images. This approach enhances the accuracy and efficiency of ANPR technology.

In today's context, owning a vehicle has transitioned from being a symbol of luxury to a practical necessity. However, the unpredictable nature of vehicular situations underscores the urgent need for adequate safety and security measures. The proposed ANPR method addresses these concerns and offers various potential applications:

1. Instantaneous Vehicle Details Retrieval: Utilizing image processing, our method allows for the rapid retrieval of vehicle details, facilitating quick identification and verification.

2. Location Detection: Agencies can effectively track the location of their vehicles using the proposed ANPR system, promoting enhanced monitoring capabilities.

3. Automated Traffic Violation Notifications: The system can automatically notify users of any registered traffic violations associated with their vehicles, promoting adherence to traffic regulations.

While vehicle tracking systems using GPS have become commonplace, our ANPR approach complements these systems by providing additional functionalities, particularly in the realm of license plate recognition.

ANPR technology can store images captured by cameras along with the extracted text from license plates. Some configurations even allow for the storage of driver photographs. The use of infrared lighting enables cameras to capture images at any time of day, and certain intersection monitoring cameras incorporate a powerful flash for illumination and to alert offenders of their violations.

It's important to note that ANPR technology may exhibit region-specific characteristics due to variations in license plate formats. This regional specificity is a crucial consideration in the design and implementation of ANPR systems to ensure optimal performance across diverse geographical areas.

The major factors driving the growth of the ANPR system market include the increasing deployment of ANPR systems in security and surveillance and traffic management applications, infrastructure growth in emerging economies, increasing allocation of funds by various governments on ITS, and the growing use of video analytics technology for intelligent monitoring of vehicles. Additionally, the rapid surge in demand for smart parking solutions is a major driver for the growth of the ANPR system market. The integration of advanced technologies such as IoT, Deep Learning, and Al with the ANPR system is promoting the growth of ANPR systems across applications such as access control and road usage charging. Growing number of infrastructure development projects across the world such as the Smart Cities mission and roadways modernization projects are promoting the growth of the ANPR system market. Moreover, surging use of video analytics technology for intelligent monitoring of vehicles is enhancing the growth of the ANPR system industry.

Evolution of ANPR:

The roots of ANPR extend back to the mid-20th century, marked by manual methods prevalent in recording license plate data. However, it is the digital age that has witnessed the metamorphosis of ANPR from a rudimentary concept to a sophisticated system. The infusion of cutting-edge technologies such as digital imaging, advanced software, and machine learning has propelled ANPR to new heights, enabling real-time recognition of license plates under challenging environmental conditions.

The evolution of ANPR is not merely a chronological progression; it represents a continuous refinement of its core components. Advancements in camera technologies, image processing algorithms, and database integration have collectively elevated the accuracy and efficiency of ANPR systems. This evolution has expanded the scope of ANPR applications, positioning it as an indispensable tool in various sectors, from law enforcement and traffic management to secure access systems and beyond.

Components Driving Evolution:

Camera Technologies: High-resolution cameras are fundamental to ANPR, capturing clear images of license plates and facilitating precise recognition.

Image Processing Algorithms: The heart of ANPR lies in sophisticated algorithms, which meticulously analyze captured images, isolate license plate areas, and extract alphanumeric characters.

Database Integration: Seamless integration with databases enhances ANPR functionality, enabling swift cross-referencing of license plate information with pertinent data.

Machine Learning Advancements: ANPR systems continually evolve through machine learning, adapting to diverse scenarios and improving accuracy over time.









1.1 Purpose of Project

The purpose of this project is to develop an efficient and user-friendly Automatic Number Plate Recognition (ANPR) system. The system aims to automate the process of vehicle identification by accurately detecting and recognizing vehicle license plates. This is achieved by leveraging advanced technologies such as the Object Detection API for vehicle and number plate detection, and EasyOCR for optical character recognition to extract the license plate number.
The project also aims to make this technology accessible and easy to use by deploying the ANPR system on Streamlit, a popular open-source app framework. This allows users to interact with the system through a web-based interface, making it more practical for real-world applications. The ANPR system can be used in various scenarios such as traffic monitoring, law enforcement, and parking management, among others. By automating the process of number plate recognition, the system can help save time, reduce manual errors, and increase efficiency in these areas. The project also contributes to the field of computer vision by demonstrating the effectiveness of combining object detection and optical character recognition technologies for practical applications.


1.2	Salient contributions of the project

EasyOCR Integration:
The ANPR system seamlessly integrates EasyOCR for accurate OCR and multilingual support, enhancing text extraction from license plates. Its adaptability to diverse language characters and fonts, coupled with a straightforward implementation, expedites development, reducing time and costs. This integration ensures efficient and precise text recognition, a vital component for successful license plate identification.

Object Detection API:
The Object Detection API is pivotal for precise license plate localization, utilizing pre-trained models to optimize speed and accuracy. Real-time capabilities enable quick image processing, ensuring timely recognition as vehicles move through surveillance areas. This feature is fundamental in enhancing the ANPR system's overall efficiency, making it well-suited for real-world applications.

Efficient License Plate Recognition:
Leveraging EasyOCR and Object Detection API, the ANPR system excels in real-time license plate recognition, optimizing speed through parallel processing. Swift identification of vehicles is ensured, and error handling mechanisms enhance robustness, addressing issues like incorrect OCR readings and solidifying the system's reliability.

Integration with Machine Learning Models:
Integration with machine learning models enables continuous adaptation and improvement, learning from new data to enhance proficiency. Region-specific training datasets bolster accuracy, making the system dynamic and proficient in recognizing diverse license plate formats. This adaptability ensures the ANPR system remains effective across various scenarios.

Configurable Data Storage:
Configurable data storage provides flexibility, allowing users to define parameters based on compliance and capacity needs. Integration with databases supports structured storage of images and metadata, ensuring scalability and easy retrieval. Archiving options efficiently manage long-term storage, enabling quick access for analysis and reporting.

Web Deployment using Streamlit for Remote Accessibility:
The ANPR system is deployed on the web using Streamlit, enhancing remote accessibility and management. Users can effortlessly monitor and control the system from any location with internet access, leveraging the user-friendly interface provided by Streamlit. This deployment method ensures seamless interaction with the ANPR system, allowing users to stay connected and informed regardless of their physical location.

1.4 Scope of assigned work

The ANPR project aims to enhance vehicle monitoring and management through real-time improvements, focusing on accurate license plate recognition with the integration of advanced OCR technologies like EasyOCR. Additionally, the project emphasizes remote accessibility via Streamlit for efficient monitoring and management from any location. Proactive traffic violation detection is a key feature, contributing to enhanced traffic regulation and safety. The overarching goal is to optimize system efficiency through streamlined processes, error handling mechanisms, and a user-friendly interface, creating a versatile and effective solution for ANPR in diverse scenarios.

 
2. Literature Review
PAPER 1: 

Title: 
Amninder Kaur, Sonika Jindal ,Richa Jindal “License Plate Recognition Using Support Vector Machine (SVM)” Dept. Of Computer Science, International Journal of Advanced Research in Computer Science and Software Engineering, Volume 2, Issue 7. 

Context: 
ANPR is a mass surveillance system that captures the image of vehicles and recognizes their license number. In this paper, A system is proposed that incorporates to successfully locate and read Indian vehicle number plates in digital images by using SVM. In this proposed model preprocessing and number plate localization is performed by using ―Otsu’s methods and ―feature based localization methods respectively. It gives reliability and time optimization. Finally, the character reorganization performs using the Support Vector Machine.

PAPER 2: 

Title: 

ANISH LAZRUS, SIDDHARTHA CHOUBEY,SINHA G.R.,”AN EFFICIENT METHOD OF VEHICLE NUMBER PLATE DETECTION AND RECOGNITION” Department of Computer Science, International Journal of Machine Intelligence, Volume 3, Issue 3. 

Context: 
The images of various vehicles have been acquired manually and converted into grayscale images. Then the Wiener2 filter is used to remove noise present in the plates. The segmentation of grayscale image generated by finding edges using Sobel filter for smoothing image is used to Dept of CSE, CMRIT 2018-19 Page 11 reduce the number of connected components and then Bilateral filter is used to calculate the connected component. Finally, a single character is detected. However, sets of blurry and skewed snapshots give worse recognition rates than a set of snapshots, which has been captured clearly Due to rapidly increase in number of vehicles across the world’s big cities, vehicle number plate recognition system has become one of the most important digital image processing systems to be used. This system will solve so many problems for these city facilities which are hard to be controlled by humans 24 hours.



PAPER 3: 

Title: 
Abhay Singh, Anand Kumar Gupta ,Anmol Singh, Anuj Gupta ,Sherish Johri, “VEHICLE NUMBER PLATE DETECTION USING IMAGE PROCESSING”, Department of IT, Volume: 05 Issue: 03 | Mar-2018 

Context: 
In this technology we will be working on CCTV footage or input images given. The CCTV footage must be clear to extract the Vehicle number from the image taken as Input. These input images are converted to grayscale and characters are segmented and recognised using OCR. There are some conditions for this software to work: 1) Vehicle plates should be white and according to the rules given by the government of India. 2) Image should be of appropriate brightness and contrast: In this, a software is designed which detects the vehicle number plate number using MATLAB. In this technique we will be performing several methods step by step to find the vehicle number. Then using that vehicle number found we will be comparing that number from our database.



PAPER 4: 

Title: 
Ganesh R. Jadhav, Kailash J. Karande, “Automatic Vehicle Number Plate Recognition for Vehicle Parking Management System”, IISTE, Vol.5, No.11, 2014. 


Context: 
This paper discusses a method for the vehicle number plate recognition from the image using mathematical morphological operations. The main objective is to use different morphological operations in such a way that the number plate of vehicles can be identified accurately. This is based on various operations such as image enhancement, morphological transformation, edge detection and extraction of number plates from vehicle images. After this segmentation is applied to recognize the characters present on the number plate using template matching. This algorithm can recognize the number plate quickly and accurately from the vehicle's image. The goal of the research is to investigate the possibility to create a comprehensive system for Indian vehicle identification based on the license plate recognition. In that case no additional hardware, such as e.g. transmitters, mounted on a vehicle, and responders will be required. The system performs well on various types of vehicle license plate images.

PAPER 5:

Title: 
Mutua Simon Mandi ,Bernard Shibwabo, Kaibiru Mutua Raphael, ”An Automatic Number Plate Recognition System for Car Park Management”, International Journal of Computer Applications, Volume 175 – No.7, October 2017

Context: 
It proposes the adoption of a mobile based software solution that has ANPR capabilities to aid in vehicle identification and vehicle registration. The software that was developed adopted an object-oriented analysis and design methodology and implements Optical Character Recognition. (OCR) using the mobile device camera to detect and capture the vehicle number plate. The proposed system turned out to be efficient when it came to implementation of automatic number plate recognition system for car park management, using Optical Character Reader (OCR) on a mobile device. Successful implementation of ANPR systems have resulted in faster and easier vehicle identification. This has also resulted in faster and easier search and retrieval of vehicle information mostly done by law enforcers in identifying vehicles that are uninsured, stolen, or driven by someone without a license or prohibited from driving. It was recorded that the system required 1/5th of the original time that was needed by the manual system. Requires an efficient Local Area Network Systems need to be integrated to be efficient.


 
2.	Description of project


Dataset: 

The dataset used in this project is used from Kaggle https://www.kaggle.com/datasets/andrewmvd/car-plate-detection. The dataset is used to train the object detection model to accurately detect vehicles and their license plates.

Model: 

The project utilizes deep learning model from the Object Detection API for the detection of vehicles and their license plates. These models are trained on the dataset and are capable of accurately identifying and locating vehicles and license plates in input images.

Load Model: 

Once the models are trained, they are saved and can be loaded for use in the ANPR system. The loading process involves retrieving the trained model parameters from storage and initializing a model instance with these parameters.

Image Detection: 

The loaded model is used to perform image detection on new input images. This involves passing the images through the model, which outputs the locations of detected vehicles and license plates. The detected license plates are then cropped from the original image for further processing.

Text Extraction: 

The cropped license plate images are processed using EasyOCR, an optical character recognition tool, to extract the license plate numbers. This involves converting the image data into a format that EasyOCR can process, and then using EasyOCR to recognize and extract the text from the image.

This process flow allows the system to take an input image, detect any vehicles and license plates in the image, and extract the license plate numbers. The extracted license plate numbers can then be used for various applications such as traffic monitoring, law enforcement, and parking management. The system has been deployed on Streamlit, allowing users to easily interact with it through a web-based interface.







Image Detection:


In this module, the image of the number plate is captured from an in-built camera. After reading and visualizing the image of the number plate, the image is then sent for further processing where it is scaled and tested using the techniques proposed in the system, specifically the Object Detection API. The Object Detection API is a robust framework for object detection tasks, including number plate detection. It plays a major role in real-time operations, which is very important in terms of technology and user-interface. By using it, one can process images and videos to identify objects, such as vehicles and their license plates. When integrated with various libraries, such as NumPy, Python is capable of processing the array structure for analysis provided by the Object Detection API. This API, combined with image processing algorithms, is used in our project to detect the number plate effectively and efficiently.


Character Recognition:

After the image detection, the image is sent for text extraction. In this module, the text from the detected image i.e., the number plate is extracted. For extracting the text from the image we have used Optical Character Recognition (OCR). OCR is a technology used to convert different types of documents, such as scanned paper documents, PDF files or images captured by a digital camera into editable and searchable data. EasyOCR is used for extracting the text from the image. EasyOCR is a python module for extracting text from image. It is a general OCR that can read both natural scene text and dense text in document. They are many features of EasyOCR few of them are, it can read more than 70 languages including English, Hindi, Tamil, Telugu, Kannada, Punjabi, etc. It can also read both horizontal and vertical text. It’s also capable of reading text from a noisy background.


By leveraging the capabilities of EasyOCR, our system can accurately extract the license plate number from the detected number plate image, thereby completing the Automatic Number Plate Recognition process. user’ Web Deployment The final step in the project is deploying the ANPR system on the web using Streamlit, an open-source app framework. Streamlit provides a user-friendly interface that allows users to interact with the system through a web-based platform. The deployed application includes features for uploading images and videos, as well as accessing a live feed for real-time number plate recognition. Users can upload an image or video of a vehicle, and the system will detect the vehicle, extract the license plate, and display the recognized number plate text. For the live feed, users can connect a camera to the system, and the ANPR system will continuously analyze the feed and recognize any number plates in real-time. This deployment makes the ANPR system accessible to users without any need for local installation or setup, further enhancing its practicality and usability.

Deployment: 

The final step in the project is deploying the ANPR system on the web using Streamlit, an open-source app framework. Streamlit provides a user-friendly interface that allows users to interact with the system through a web-based platform. The deployed application includes features for uploading images and videos, as well as accessing a live feed for real-time number plate recognition.
Users can upload an image or video of a vehicle, and the system, powered by the Object Detection API and EasyOCR, will detect the vehicle, extract the license plate, and display the recognized number plate text. For the live feed, users can connect a camera to the system, and the ANPR system will continuously analyse the feed and recognize any number plates in real-time.


 


Activity Diagram For The System

![image](https://github.com/user-attachments/assets/8a8a9e20-e4a0-4807-845f-4f802701a1f3)


 
Iterative Design Diagram

![image](https://github.com/user-attachments/assets/8a5a382b-1524-4014-a0e2-c427d830eea4)

 
 
DFD Level 1 Diagram of the system

![image](https://github.com/user-attachments/assets/cfa7545c-8f34-41d8-9e8b-d125a0ac05a2)














