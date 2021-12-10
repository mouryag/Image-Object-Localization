# Image-Object-Localization
This is a Object Localization problem in which we find what the object is in the image(image classification) and where the object is present in the image and draw bounding boxes(Object Localization).It involves both classification and regression problems.
<br><br>

**Image Classification**: Predict the type or class of an object in an image.
<br>Input: An image with a single object, such as a photograph.
<br>Output: A class label (e.g. one or more integers that are mapped to class labels).
<br><br>**Object Localization**: Locate the presence of objects in an image and indicate their location with a bounding box.
<br>Input: An image with one or more objects, such as a photograph.
<br>Output: One or more bounding boxes (e.g. defined by a point, width, and height).
<br><br>**Object Detection**: Locate the presence of objects with a bounding box and types or classes of the located objects in an image.
<br>Input: An image with one or more objects, such as a photograph.
<br>Output: One or more bounding boxes (e.g. defined by a point, width, and height), and a class label for each bounding box

<br><br><br><br>

Here I used custom dataset for finding bounding boxes for an object.

<br><br>
In our first example, we did what is quite possibly the simplest thing possible, localize a **white box on a black background**
<br><br>
And our second example, we started using a real object, **an image of Charmander(pokemon)**.
<br><br>
And our third example, we resize the object so that our network would be able to find **objects of different sizes**.
<br><br>
In the fourth example, we flip the objects so that our network would be able to find the **same object at different orientations** and uses resizing,flip,rotation,different contrast,brightness and other image trasformation techniques.
<br><br>
And our fifth example, we added **real background to the image**, since in real applications, images can have many objects in them, not all relevant.
<br><br>
In our six example, we considered the case **where the objects need not appear**, which of course is alsomore realistic.
<br><br>
In seventnh example, we are going to consider the case where we have **multiple classes of objects** (Pokemons), so,for example, in a self-driving application, you will have to recognize people, traffic signs, cars,bicycles and so forth.
<br><br>
We know that for the three classes we would like to apply the softmax activation and for the other five we use sigmoid activation and custom loss function using Binary cross entropy and Categorical cross entropy.

<br><br><br>
![localize1](outputs/localize1.PNG)
<br><br>
![localize1](outputs/localize2.PNG)
<br><br>
![localize1](outputs/localize3.PNG)
<br><br>
![localize1](outputs/localize4.PNG)
<br><br>
![localize1](outputs/localize5.PNG)
<br><br>
![localize1](outputs/localize6.PNG)
<br><br>
![localize1](outputs/localize7.PNG)
<br><br>
![localize1](outputs/localize8.PNG)
