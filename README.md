# Remote-Intelligent-Assistant-REIA
A Linux based desktop assistant using Machine Learning and Natural Language Processing

**Description of Project**: https://www.quora.com/What-is-your-favorite-coding-project-you-have-done/answer/Aseem-Raina-2?srid=JRQg

**Environment**
1. Linux based system
2. Python3
3. Slack

**Slack Configuration**
1. Create a new slack id on https://slack.com/. Choose a url for your team.
2. Generate your slack token from https://get.slack.help/hc/en-us/articles/215770388-Create-and-regenerate-API-tokens.  
   Paste this token in the config file under slack->slack_token.
3. You can get your user user_id, channel_id from https://api.slack.com/methods by testing the api method calls.  
   Copy these over to slack->user and slack->channel.
4. You should now be able to communicate with REIA. For security purposes, don't share the tokens with anyone. 

**Installation**
1. We have added the dependencies in a requirements.txt file. You can install the same by running   
   pip3 install -r requirements.txt
2. Download Stanford POS Tagger from https://nlp.stanford.edu/software/tagger.shtml. Extract the contents to the ~/Downloads
   folder (You can extract it in any directory). Be sure to modify the 'tagger' parameters appropriately in the config    
   file. 
3. Make sure your system has Java installed. If not proceed as give in the link:
   https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04
4. **Open the src/reia.py file, and change the path on line line 97 (cmd, sed) to reflect the path on your own system.**
5. Open two terminal windows. Navigate to the root directory of the project. Run the following commands in the two seperate
   windows:  
   -> python3 src/app.py  
   -> pyhton3 src/reia.py
   (You can run the commands using sudo for faster response times, but be careful of the commands you type. We have tried our best
   to avoid any commands that can break or mess with the system)
6. The application should display "Starting..." in the reia.py terminal. Now you are all set.
7. Open up the slack channel or mobile app. Type your messages in the channel with the prefix '@reia' (without quotes).  
   eg. @reia what is my ip address
8. You should see a reply posted to the channel.

Note: If the application doesn't run as expected, check the terminal for any error messages. We run the application with a clean install without any additional installations and debugging. Try and solve the error, as we currently do not have the resources to test the application on different environments. If the error still persists, open a new issue or contact me on my email.

Contact: aseemraina1996@gmail.com
