# MFSDKAndroid

# Introduction
Those building new integrations should consider using  MyFatoorah, which is the easiest way to accept Knet, credit cards, and many other MyFatoorah payment methods.

The MFSDK makes it easy to add MyFatoorah payments to mobile apps.

# Prerequisites
You will need a [My Fatoorah](https://myfatoorah.com) account.

# Using the Android archive (*.aar) file

1. In Android Studio, create a new project or open up an existing project that you want to use the Android archive file library.
2. In the Project view, expand the libs node of the app.
3. Using the Mac Finder or Windows Explorer, select and copy the Android archive file (*.aar) e.g. MFSDK.aar. Paste the aar file into the libs node in Android Studio.

The Copy dialog box appears.

![Screenshot](https://github.com/MyFatoorahHub/MFSDK/blob/master/Setp%201.png)

4.If necessary, change the name. Click OK.

The Aar file is added to the project.
5. In Android Studio, open the app's build.gradle file in the editor.

![Screenshot](https://github.com/MyFatoorahHub/MFSDK/blob/master/Setp%202.png)


6. As shown above, add in the repositories section.

      repositories {
                flatDir {
                       dirs 'libs'
                        }
                   }

7. Add in the following line to the dependencies section.

     compile (name: 'myaarlibrary-release', ext:'aar')

Now the classes and methods in the Android archive file can be used in your app, as shown in the example below.

![Screenshot](https://github.com/MyFatoorahHub/MFSDK/blob/master/Setp%203.png)


# Test Cards Details
1. KNET Test Cards
    - 8888880000000001 (any Pin /Expiry) Captured
    - 8888880000000002 (any Pin /Expiry) Not Captured

2. MasterCard Test Cards
    - Card No: 5123456789012346 
    - Expiry Date : 05/17
    - CVV: 123

    - Card No : 5313581000123430
    - Expiry Date : 05/17
    - CVV: 123

3. Visa Test Cards
    - Card No: 4005550000000001 
    - Expiry Date : 05/17
    - CVV: 123

    - Card No : 4557012345678902
    - Expiry Date : 05/17
    - CVV: 123
    
    
 # Requirements

- Android Studio Version 
- Android 9.0+ target deployment
- phone and Tablet of all sizes and resolutions
 
