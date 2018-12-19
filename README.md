# chatbot2018

## Introduction
* 這是簡單的聊天機器人，用來快速查詢當日的電影播放場次，如果平常想要殺時間或找點休閒，這是一個不錯的選擇。</br>
* 使用方法:
 1. 輸入'know more'，會看到3個按鈕，其中兩個可以選電影類型，最後一個會連到影評連結或電影介紹。
 2. 選擇好類型之後，繼續選擇實際要看哪部電影。
 3. 接下來，選擇要去哪個影城觀賞。
 4. 最後，會出現該影城的地圖以及當日電影播放之場次。
 5. 回到1. 重新開始。
 
## My Fsm Image
 ![alt](https://i.imgur.com/wavxNFb.png)

## How to Implement My Chatbot

* user state:</br>
  Type everything you like.</br>
  1. If the users type 'know more',then go to state1.</br>
  2. If the users type 'contact',then go to state2.</br>
  3. If the users type 'give me a hug',then go to hug state.</br>
  4. If the users type something which is not mentioned above,then back to user state.</br>

* state1:</br>
  The users will see 3 buttons,which we can choose one service.</br>
  1. If the users choose 'blockbusters',then go to state2.</br>
  2. If the users choose 'high score movies',then go to state3.</br>
  3. If the users choose 'movie introduction',then go to state4.</br>

 * state2:</br>
  The users will see top3 blockbusters in theather now.</br>
  Pick one movie we are interested in.</br>
  After we choose,then we can go to choice state.</br>
 
* state3:</br>
  The users will see top3 movies with highest score in theather now.</br>
  Pick one movie we are interested in.</br>
  After we choose,then we can go to choice state.</br>

* state4:</br>
  We can get a link for movie introduction.</br>
  
* hug state:</br>
  It will reply 'thank you!!!' and back to user.</br>

* choice state:</br>
  Now we just pick uo  one movie,so we are going to choose one movie theather in Tainan.</br>
  The users will see 3 buttons,which we can choose one theather.</br>
  1. If we choose theather1,go to theather state.</br>
  2. If we choose theather2,go to theather2 state.</br>
  3. If we choose theather3,go to theather3 state.</br>

* theather state:</br>
  It will print the movie broadcast time(just for today) and the picture for the location of the theather.</br>
  Now you can back to user state if you type anything you like again.</br>
  
* theather2 state:</br>
  It will print the movie broadcast time(just for today) and the picture for the location of the theather2.</br>
  Now you can back to user state if you type anything you like again.</br>
  
* theather3 state:</br>
  It will print the movie broadcast time(just for today) and the picture for the location of the theather3.</br>
  Now you can back to user state if you type anything you like again.</br>

