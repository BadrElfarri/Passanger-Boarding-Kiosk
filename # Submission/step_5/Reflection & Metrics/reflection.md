<p style="text-align:center"> <h1> <font color=#BF9270> Reflection: Automated Passenger Boarding Kiosk </font>  </h1> </p>
<h2><font color=#E3B7A0> Challanges </font></h2>
<div style="margin-left:2.5em">
    <p>
        <font color=#FFEDDB> 
            There have been many challenges that have been encountered during this project.
            The main ones are described below.
            <ul>
                <li> 
                Blob Storage for model training: The form recognizer model training through files 
                stored in blob storage was a challenge. Using SAS authorization did not work when the 
                SAS generated is for a subfolder inside a container. This has been solved by having a 
                dedicated container for training files to be used in boarding-pass model training 
                </li>
                <li> 
                Lighter detection: The light was not dedicated properly using only images provided 
                in the starting files. Additional images were added, furthermore, the test images are 
                divided into 2, 3 pictures are used for training to increase the accuracy of the model. 
                The model is much better in the detection of lighter on the unused pictures in the model 
                training after adding 3 pictures from the luggage testing images. For future model training,
                more pictures from lugage container must be used to get a more accurate model. Training the 
                model on pictures that are closly identical to what its suppose to predicte will yield better
                results.
                </li>
                <li> For future goal: A React frontend with Flask backend application must be developed to make
                the project easier to play with and further develop on accurate detection and validation.
                Furthermore, different ids verification should be added. </li>
                <li> Personal info and flight specific info. </li>
            </ul>
        </font>
    </p>
</div>
