Brandon Devan
ST10442244

link to repository: https://github.com/branz8/IMADSUPP.git

The purpose of this app is to help and encourage people to drink water. It tracks how much water they have drank and also sets reminders to tell them when to drink water. I designed the app in a way thas very user friendly nd it helps people to use the application with ease and no complications

flowchart:
START

SplashActivity.onCreate
     setContentView(activity_splash)
     Set delay (2 seconds)
     Navigate to MainActivity
     finish() SplashActivity

MainActivity.onCreate
     setContentView(activity_main)
     Set OnClickListeners for buttons
        btnViewDetails.onClick
    Navigate to DetailedViewActivity
       btnClearData.onClick
    Clear Data Logic

DetailedViewActivity.onCreate
     setContentView(activity_detailed_view)
     Set OnClickListener for btnBack
     finish() DetailedViewActivity
END

Pseudocode:
FUNCTION SplashActivity.onCreate
    CALL setContentView(activity_splash)

    SET splashScreenDuration TO 2000 milliseconds

    CALL Handler.postDelayed WITH delay: splashScreenDuration, ACTION:
        CALL startActivity WITH Intent(this, MainActivity)
        CALL finish()

END FUNCTION

FUNCTION MainActivity.onCreate
    CALL setContentView(activity_main)

    SET OnClickListener FOR btnViewDetails TO:
        CALL startActivity WITH Intent(this, DetailedViewActivity)

    SET OnClickListener FOR btnClearData TO:
        CALL clearData

END FUNCTION

FUNCTION clearData
    // Add logic to clear hydration data
END FUNCTION

FUNCTION DetailedViewActivity.onCreate
    CALL setContentView(activity_detailed_view)

    SET OnClickListener FOR btnBack TO:
        CALL finish()

END FUNCTION

Screenshots of app:
![Screenshot (28)](https://github.com/user-attachments/assets/a0f59594-1aa6-4378-807b-000ec18786f9)
![Screenshot (30)](https://github.com/user-attachments/assets/1bf2ce82-01cb-44cf-b5ef-4ebab9441c19)
![Screenshot (31)](https://github.com/user-attachments/assets/0cf6fe5c-d04c-4a74-90bb-fc0cc58a307a)
![Screenshot (32)](https://github.com/user-attachments/assets/42db2b42-b489-4070-9e5d-88471f6b2f18)
![Screenshot (33)](https://github.com/user-attachments/assets/d94c90cc-cf37-4b4a-9e12-24da6bfe86c5)
![Screenshot (34)](https://github.com/user-attachments/assets/a47c9db7-8b03-466f-b021-f5260b5a1b86)
![Screenshot (35)](https://github.com/user-attachments/assets/990506e6-157a-49fb-8413-0da92e24f750)

