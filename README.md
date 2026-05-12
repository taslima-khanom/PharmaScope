# PharmaScope
PharmaScope is a computer vision system designed to help users identify medications from images and detect potential risks such as drug and food interactions.
The project combines object detection and optical character recognition (OCR) to analyze photographs of pills and extract meaningful medical information. First off, the system uses a pretrained YOLOv8 deep learning model to locate pills in an image by drawing bounding boxes around each detected tablet or capsule. Each detected pill is then cropped and sent to an OCR model (EasyOCR), which reads the imprint engraved on the pill surface. The OCR does this by converting the image to grayscale so that the engraved marking is made clear and is easier for the OCR to read. The imprint text is cleaned and matched against a small medication database that contains drug names, strengths, risks, as well as warnings. If a medication is successfully identified, the system displays this information and checks for potential interactions with other detected drugs or common food triggers such as caffeine or grapefruit.
The goal of this project is to demonstrate how deep learning and neural networks can be used to improve medication safety and reduce human error. It highlights how computer vision and neural networks can assist patients, students, and healthcare workers by providing drug identification and educational safety feedback.
In the future, I would like to improve PharmaScope by training a pill-specific object detection model using a medical pill dataset, which would improve detection reliability. OCR accuracy could also be improved using a specialized text recognition model trained on pill imprints. 

#How to Use:
step1: take clear images of the tablets
step2: upload images into system and run!
