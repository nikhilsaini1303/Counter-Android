# Counter-Android


To create a simple counter app in Android Studio, follow these steps:

1. Create a new project in Android Studio. In the "Create New Project" dialog, choose "Empty Activity" as the template.

2. Design the user interface for the counter app. Open the layout file for the main activity and add a TextView to display the counter value, and two Buttons to increment and decrement the counter value. You can arrange these UI elements as per your design preference.

3. Implement the counter logic. In the MainActivity.java file, define an integer variable to store the counter value, and initialize it to 0. Then, add a method to increment the counter value and another method to decrement the counter value.


      public int i = 0;
      
4. Add an OnClickListener to the increment and decrement buttons. In the onCreate() method of MainActivity.java, add OnClickListener to the increment and decrement buttons to trigger the counter increment and decrement methods when the respective button is clicked.


      btn1.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                i += 1;
                txt.setText(Integer.toString(i));
            }
        });

        btn2.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                i -= 1;
                txt.setText(Integer.toString(i));
            }
        });

        btn3.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                i = 0;
                txt.setText(Integer.toString(i));
            }
        });
        
 5. Test the app. Run the app on an emulator or a physical device and test the counter by clicking the increment and decrement buttons. The app should display the updated counter value in the TextView.

       
        
      
