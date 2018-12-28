# MobileAppProject
# Book Donation System

#### Developers
* Muaadh Esmail Qaid Almrahm 1529799 
* Rama Ashoor 1415615
* Maha Abdulmaleka 1322200
* Mohammad Hilmi Bin Halid 1611309

# 1.1    INTRODUCTION 
We are developing a system that helps to make use of the Neglected books to deliver them to the interested readers. The system will view a plenty of different books along with their owners' details. On the other hand, the readers will have a chances to either donate or borrow a book from the system.   
# 1.2    PROBLEM DESCRIPTION
### 1.2.1    Background of the problem 
In the 21st century, the interest of student has changed gradually in the educational system.
However, the main change the impact the learners generally are turning away from reading the books and relying on other learning materials. 
Which eventually leads to a new careless generation of the books. 
As a result, students are no longer giving a good care for the books they receive or buy. 
On the other hand, there are still some learners depending on books for their studies. 
Therefore, this system emerged to come up with the solution for the gap. 

### 1.2.2    Problem Statement
 It is well known that some book owners carelessly throw their books after they gain what they need from them.
 While some other readers are seeking to gain such a book.
 Above all that, knowledge should be respected and put in proper place until its fans come
# 1.3    PROJECT OBJECTIVE 
 From this knowledge  project we want to  allow the user to use the system easy to check what the books are available to borrow and help the book owner to share their book to give benefit to whom in need, this app process will have two main process, the first process allows the user to donate with his book by upload the book in the system with short description or use the QR code to define the book with it details, another process can check what is the book available if want to borrow. so by this app can protect the book from a throw and encourage the students to search if their requirement book is available to borrow or not.
# 1.4    PROJECT SCOPE 
### 1.4.1    Scope 
The scope of the Book Donation project to :
- Reuse the Neglected book in use not just put on the shelve.
- Easy to donate with the unused books anymore to give a chance to other to borrow and read.
- Use QR code/ barcode to set the details of a book
### 1.4.2    Targeted 
IIUM community
     
### 1.4.3    Specific Platform
 For the project to be working, we might need to use the software such as Microsoft Visual Studio Code to write the application code. We might also need to use Android Studio software or Expo application as an emulator to see whether the code can be compiled and run to become an application or not.
     
# 1.5    CONSTRAINTS 
 As for the constraints, we might be having difficulties in discussing physically since our team member didn't stay in the same mahallah. Due to that, we might have difficulties to integrate the project from everyone. Since our project might not be using any financial budget, we hope that we could finish the project by using the existing software and platform that we have learned from the class.
     
# 1.6     PROJECT STAGES 
 - Project Initiation
      - Project Proposal 30/11/2018
 - Project Planning
      - determine the mains functions , database "firebase" , 
 - Project Execution
      - The first version should be done during the first week of development 7/12/2018
      - Have an appointment with dr.sidery, sister Khutar to solve any problems 8/12/2018
 - Project Closure
      - submit the project and do the final presentation in the class 14/12/2018

# 1.7    SIGNIFICANCE OF THE PROJECT 
 This mobile app provide a helpful service for IIUM society by using the book probably and don't storage the books in the rooms, donators will have a barakah when he donators or rent his book on the other side students can find books easily and with low cost.

# 1.8    SUMMARY 
 This project is done as an assignment for Mobile Application Course, Sem 1 2018/2019 at IIUM.
provide a bookstore service for IIUM society by using react native framework to develop a mobile application platform
# 1.9    Functionalities in details 

Sign Up: The user must be sign up to access to the information in the application.Connecting with database.Use firebase auth using email and password in login 
Login:
import { createStackNavigator, createAppContainer } from 'react-navigation';
 
 
Add book:
 the details  of the book will in the form of Textinput where the user need to provides all the information. Regraidng the image of the book and BarCode I created a new external component where can handle all functionality of photoupload. These information will be stored in states then forwarded to addNewbook(). Which will eventually result into pushing up the data to the DB (Firebase). 
To send the data object to DB firebase 
firebase.database().ref().child('books').push().set(data);
On the other hand, I have created the DB and tables required to store the data of the users as well as the books using FireBase.
 
Edit book:
User can update the details of the book. This includes updating the book title, book description and book number. As for the codes, we use the 
Upload Image:
 can access to the phone gallery and camera by using ImagePicker to display the system UI for choosing an image or a video from the phone's library.
Also require a permission to access to the phone gallery and camera
await ImagePicker.launchImageLibraryAsync();
await Permissions.askAsync (Permissions.CAMERA);
 
Bar Scan code:scan the barcode on the book by using , BarCodeScanner
 
Home page: contain all available book to borrow, all the add book from the user will send to home page.
Show page: This page is to display the book details. This comprises the book title, book description and book number. As for the codes, we use the <Text> to display the book details.

Features
List.Section
TouchableOpacity: Opacity is controlled by wrapping the children in an Animated
Card
Object 
Components 
Different Libraries.
Button
StyleSheet
Image
BarCode
React-native-paper

# 2.0    Data storage structure

# 2.1    REFERENCES
See [React-Native](https://facebook.github.io/react-native/docs/getting-started)
See [Firebase](https://firebase.google.com/docs/)
