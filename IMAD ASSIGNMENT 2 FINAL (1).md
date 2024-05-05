**Londeka Nokuhlengwa Zulu – ST10444789**

**Ice Task 6**

**<u>3.GitHub and GitHub Actions</u>**

Go to the GitHub website (https://github.com/) and sign in to your
account.

Click on the "+" icon in the top right corner and select "New
repository".

Give your repository a name (Assignment2), add a description (use
IMAD5112 Assignment 1) and choose public.

Click on the "Create repository" button.

2\. Initialise the Repository with a README File:

After creating the repository, you'll see an option to "Initialize this
repository with a README". Check this option to create a README file.

Click on the "Create repository" button to finalize the creation of the
repository.

3\. Commit and Push Your Project Files to the GitHub Repository:

In Android Studio, go to VCS (Version Control System) -> Import into
Version Control -> Share Project on GitHub.

Log in to your GitHub account if prompted and select the repository you
created earlier.

Click on the "Share" button to push your project files to the GitHub
repository.

4\. Regularly Commit and Push Your Code as You Make Progress:

After the initial push, continue making changes to your project in
Android Studio.

Whenever you make significant progress or changes, commit your changes
locally in Android Studio using VCS -> Commit Changes.

Once committed, push your changes to the GitHub repository using VCS ->
Git -> Push.

**<u>Github Repository Link</u>**

<https://github.com/Londekazulu/Assignment2.git>

**VCS -> Git-> Push.>**
<https://github.com/Londekazulu/Paw_Play_VirtuaApp.git>

***<u>Run Test</u>***

<img src="media/image1.jpeg" style="width:6.26806in;height:2.89792in" alt="A screenshot of a computer Description automatically generated" />

***<u>Build APK</u>***

<img src="media/image2.png" style="width:6.26806in;height:3.13542in" alt="A screenshot of a computer Description automatically generated" />

**<u>4. YouTube Link</u>**

<https://youtu.be/K6x268TN7s8>

**5<u>. MainActivity</u>**

package
com.example.myapplication.myapplication.myapplication.myapplication.ppvapp  
  
import android.content.Intent  
import androidx.appcompat.app.AppCompatActivity  
import android.os.Bundle  
import android.widget.Button  
  
class MainActivity : AppCompatActivity() {  
override fun onCreate(savedInstanceState: Bundle?) {  
super.onCreate(savedInstanceState)  
setContentView(R.layout.*activity_main*)  
  
//Button to navigate to the second screen  
val startButton = findViewById\<Button>(R.id.*startButton*)  
startButton.setOnClickListener **{  
**val intent = Intent(this,Activity2::class.*java*)  
//Pass the message "I am hungry" as an extra with the intent  
intent.putExtra("FEED_MESSAGE","I am hungry")  
startActivity(intent)  
**}  
**}  
}

**<u>Activity2</u>**

package
com.example.myapplication.myapplication.myapplication.myapplication.ppvapp  
  
import android.annotation.SuppressLint  
import androidx.appcompat.app.AppCompatActivity  
import android.os.Bundle  
import android.widget.Button  
import android.widget.ImageView  
import android.widget.TextView  
class Activity2 : AppCompatActivity() {  
@SuppressLint("MissingInflatedId")  
override fun onCreate(savedInstanceState: Bundle?) {  
super.onCreate(savedInstanceState)  
setContentView(R.layout.*activity_2*)  
val petImageView = findViewById\<ImageView>(R.id.*petImageView*)  
val feedButton = findViewById\<Button>(R.id.*feedButton*)  
val washButton = findViewById\<Button>(R.id.*washButton*)  
val playButton = findViewById\<Button>(R.id.*playButton*)  
  
val feedTextView = findViewById\<TextView>(R.id.*feedTextView*)  
val cleanTextView = findViewById\<TextView>(R.id.*cleanTextView*)  
val playTextView = findViewById\<TextView>(R.id.*playTextView*)  
  
//Retrieve the message passed from the first screen  
val feedMessage = *intent*.getStringExtra("FEED_MESSAGE")  
//Set the text of the feed TextView to the feed message  
feedTextView.*text* = feedMessage  
  
//Logic for the Feed button  
feedButton.setOnClickListener **{  
**//Change the pet's image to match feeding action icon  
petImageView.setImageResource(R.drawable.*marcus2*)  
  
  
//Update the pet's values(e.g., health, hunger,cleanliness)  
//Update the feed TextView  
feedTextView.*text* = getString(R.string.*feed_thank_you*)  
  
//Update the play TextView  
playTextView.*text* = getString(R.string.*play_with_me*)  
  
**}  
  
  
**//Logic for the Wash button  
washButton.setOnClickListener **{  
**//Change the pet's image to match cleaning action icon  
petImageView.setImageResource(R.drawable.*marcus4*)  
  
//Update the pet's status values (e.g., health ,hunger,cleanliness)  
//Update the clean textview  
cleanTextView.*text* = getString(R.string.*clean_nice_and_clean*)  
  
**}  
  
**// Logic for the Play button  
playButton.setOnClickListener **{  
**// Change the pet's image to match playing action icon  
petImageView.setImageResource(R.drawable.*marcus1*)  
  
//Update the pet's status value(e.g.,health,hunger,cleanliness)  
//Update the play TextView  
playTextView.*text* = getString(R.string.*clean_after_playing*)  
  
**}  
**}  
}

**6. <u>Reference for assignment 2
</u>**<https://www.reddit.com/e3ulkdloyeq01.jpg?auto=webp&s=cf19462d2d15cceb5113fa1bf34932d4475b9f18>

IMAD5112/d/p/w (2021). Introduction to Mobile Application Development
\[Module code: IMAD5112/d/p/w\]. The Independent Institute of Education
