# Build Your Own Chatbot
   - Full tutorial https://pythonprogramming.net/chatbot-deep-learning-python-tensorflow/
   - Can be used to for Twitter - Charles the AI - https://twitter.com/Charles_the_AI?lang=en

## Build custom chatbot
  1. Download Dataset https://www.reddit.com/r/datasets/comments/3bxlg7/i_have_every_publicly_available_reddit_comment/?st=j9udbxta&sh=69e4fee7
  2. Create chatbot_database.py. Create tables, & columns (parent id, comments, parent data, body, subreddit, score)
  3. Clean data - Format/remove quotes, spaces, unnecessary characters
  4. Find out if comments are acceptable (grab data with upvoted comments)
  5. Insert data - Browse/View results
  
## Create training data
  1. create_training_data.py. Two data files train.from and train.to (Parent comment and child reply)

## Run Model - Tensorflow NMT - Neural Machine Translation 

  1. Prepare GPU VM or Desktop 
     - Install Python 3.6, Tensorflow GPU 1.4, Cuda 8.0 Toolkit, cuDNN
     - Cuda and cuDNN enable GPU processing
     - Paperspace provides ML-in-a-Box for $10 (Versions have been updated)
  2. Clone NMT github project https://github.com/daniel-kukiela/nmt-chatbot
  3. Install requirements pip install -r requirements (tqdm, colorama, regex)
  4. Copy train.from and train.to to data folder
  5. Cd to setup folder and run python prepare_data.py
  7. Cd to root folder and run python train.py 
     This will tokenize the data using a BNN Bidirectional Neural Network - https://github.com/tensorflow/nmt
 <p align="center"><img src="https://user-images.githubusercontent.com/25274772/52161583-0698fb00-267c-11e9-912f-df4b134307c0.png" width="550" height="300">
  
## View Data in Tensorboard 
  1. Access by running in command prompt nmt-chatbotmaster\model>tensorboard --logdir=train_log/
  1. Check for Blue Score & Epochs
  2. View Word vector projector
  
## Deploy 
  1. View training data in output.dev
  2. Run python inference
  3. Run modded inference
  4. Chat with your bot - Ctrl+Win+Enter = Narrator
  
## Additional chatbot project
https://github.com/llSourcell/tensorflow_chatbot
  
  
  
  

  
