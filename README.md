# AS-P1-Gesture-Recognition
Using Neural Networks To Perform Simple Gesture Recognition
How can we make hospitals a safer place for everyone?

Why would people be concerned about this?
Nowadays, hospitals have become a place where mostly everybody comes just so they can get themselves checked for any infection or disease. People also crowd to hospitals so they can get treatment or surgery done and this statement does not need endorsement after witnessing the ongoing pandemic of SARS-COV-2(COVID-19). And so there are high chances that some communicable disease may spread due to accidental contact with somebody when at hospitals or other health institutions. And so given below is a way to prevent this situation.

How can machine learning be used for such a task?
There is a simple answer to that question,  no it can’t be used. But, to some extent, we can minimize the amount of contact between two people using two simple ways: Gesture Communication and Mask Detection. 
Let’s take a special case, suppose some person is infected by a disease which is communicable. This person is likely to be isolated in a hospital nearby by local authorities, maybe in an isolation ward. Now, for treatment of this person, the staff needs to go in and out, providing him/her with medication, food, and water. As of now, according to me machine learning can’t detect if the staff would contract the infection or not but it can help see if the staff going in and out are wearing a mask or not and then trigger a flag which sprays a sanitizer on their hands before going in. This can act as a lock system, that if you’re not wearing a mask, you’re not allowed in no matter what.
Consider again the previously infected person’s case. Although the staff maybe be well aware of when to provide the infected with medication, food or water, it can be the case that sometimes they forget or they have been sent for. The patient can have a camera installed in his ward which will read a gesture being shown by the patient, classify it accordingly, and then send a message which corresponds to the detected class which then gets relayed to the staff and they provide the infected with the needed commodities. Say, that a simple fist corresponds to ‘Need Water’,  this message is relayed to the staff which then proceed appropriately.





Report of data used for the tasks:

Mask/No Mask Detection:
My brother is well-versed in coding. He created a script in Python which takes the feed from the camera of the device the script is running on and takes 250 by 250 images of faces with masks on and off. This model used pictures of me, my brother and my mother, masked and unmasked. Each person giving 500 images of mask on and off. So, total images for mask on: 1500 and mask off: 1500. Total Images Used: 3000
The images have different masks on three different people with varying face positions and distance from camera so the model can detect on a variety of colours and situations which may occur inside an open space or hospital.

Gesture Messaging System:
The dataset used for this task was provided by the website Kaggle. The dataset has 6 classes for a 6 different gestures which can be mapped to 6 different messages. The model is trained as such that each class is named A, B, C, D, E, F, G … and so on so a message can be mapped to any gesture without changing the underlying trained model. A mapping scheme I thought of:
A: Need Water
B: Need Food
C: Need Medicine
D: Emergency … and so on.
The amount of each images for each label is not uniform throughout, but the range varies from 200 – 400 for each class. But, the total amount of images: 1782
The images have been clicked with a piece of paper behind them, which loosely captures the usual tone of hospital walls and so the amount of variety is not a significant problem to worry about. Also, some images have a purple background and some have a fair coloured hand with a cream coloured background to provide some variety in the data. This data was extracted by my camera feed directly. 
