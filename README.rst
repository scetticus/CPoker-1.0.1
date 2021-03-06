
CPocker: An poker game against the machine.                               
===========================================
                                                                           
 :Writing by: Eddie Brüggemann

 :Programmed in: C

 :release: 18/01/2015

 :Version: 1.0.1               

 :Contact: mrcyberfighter@gmail.com
                                          
 :Credits: Thank's to my beloved mother, my family and to the doctors.              
           Stay away from drugs, drugs destroy your brain and your life.    
                                                                           

.. image:: ./CPoker_Icon.png

Description                              
-----------

 **CPocker**: a poker game against the machine.                               
                                                                           
 By Start **CPoker** display an welcome screen with a little animation, in which
 you can choose the number of rounds you want to play against the machine  
 20 per default.                                                           
 You can increase the value with the **ARROW UP** and decrease it with the **ARROW DOWN**.                                                                     
 Once you have selected the number of rounds you want to play, you can press
 the **Return** key to start the game.                                         
                                                                           
 By game start there only a stack of card displayed and you must press the
 **"Distribute cards"** Button so that the machine mix the cards and distribute
 it to the player and to the computer so that everyone get his fives start 
 cards.                                                                    
                                                                           
 The cards are presented returned to you, so that you don't know immediately
 what cards you get in hand. You can press the left mouse key by holding   
 the mouse over a card to return it and discover what cards you get.       
                                                                           
 Then you can throw the cards you don't want to keep by dragging it to the 
 throw card frame at the middle-right from the playground.                 
 
 **Note** that you can exchange the place of your cards if you want, so you can
 order it Ace you like, even move it into an emtpy frame. To get a better view 
 of your hand.                                                                
                                                                           
 Then you must press the **"Computer play"** button so that the computer, your 
 adversary, can throw the cards he doesn't want to keep. The cards of the  
 computer are covered so that you cannot sea what the computer get in hand,
 until the round end and the cards combination comparison.                 
                                                                           
 The programme is implemented so that you sea your cards but the computer  
 doesn't not know what cards you get in hand until the round end and the   
 cards combination comparison.                                             
                                                                           
 Then you must press the **"Give new cards"** button so that the cards you and 
 the computer have throw rare replaced by news. They are presented to you  
 returned again, so that you can return it or not before seeing what       
 the computer get in hand or seeing.                                       
                                                                           
 One the all the cards are returned you must press the **"Update score"**      
 button. And the programme will compute the round winner, display a blinking
 round winner notify message, and update the rounds win score window at the
 down-left corner from the screen from CPoker.                             
                                                                           
 Now that the round is finish you must press the "New round" button so that
 the programme gather all cards from the playground mix it again and prepare
 all the settings for a new round.                                         
                                                                           
 You are ready for a new round: press the **"Distribute cards"** button to     
 continue playing.                                                         
                                                                           
 Wenn the count of rounds to play is reached the computer display which from
 you or the computer have win the entire game, even nobody: egality.       

 Wenn the game is finish you can come back to the main scren by pressing The
 **ESCAPE** key or at every time you want it.                                     

CPocker cards combinations hierarchy
------------------------------------                  

                                                                           
 CPoker follow the cards combination hierarchy according to the poker rules:
                                                                           
  From the highest to the lowest combination:                              
                                                                           
  1. **ROYAL QUINTE FLUSH**
                                                   
     5 following cards values ending with an *Ace* from the same color (*Diamond*,
     *Heart*, *Spade*, *Club*).                                                  
     if the two players get a **ROYAL QUINTE FLUSH** there is an egality.     
     No color have precedence on another.                                  
                                                                           
  2. **QUINTE FLUSH**
                                                        
     5 following cards values not ending with an Ace from the same color    
     (Diamond , Heart, Spade, Club).                                          
     if the two players get a **QUINTE FLUSH** the highest card decide which is
     the winner. If the tow players get the same **QUINTE FLUSH** in different 
     colors (*Diamond*, *Heart*, *Spade*, *Club*) they are at egality.               
     No color have precedence on another.                                  
                                                                           
  3. **FOUR**
                                                                 
     4 same cards from the same value.                                     
     It's impossible that the 2 players get the same four at the same time 
     in a 32 cards game (from *7* to *Ace*). **CPocker** use a *32 cards game*.      
                                                                           
  4. **FULL HOUSE**
                                                           
     3 same cards from the same value (a **BRELAN**) and 2 same cards from the
     same value (a **PAIR**).                                                 
     Egality is not possible with a 32 cards games, because for comparing 
     2 **FULL HOUSE** we must compare the **BRELAN** values which cannot be the same
     in a 32 cards game (from *7* to *Ace*).                                   
                                                                           
  5. **COLOR**
                                                              
     5 cards from the same color.                                          
     In case the two players get a **COLOR** there are egality.                
     No color have precedence on another.                                  
                                                                           
  6. **QUINTE**
                                                              
     5 following cards values from different colors.                       
     In case the two players get a **QUINTE** the value of the highest card    
     decide which is the winner.                                           
     If the highest card is the same by the two players there is egality.  
     No color have precedence on another.                                  
                                                                           
  7. **BRELAN**
                                                               
     3 same cards from the same value.                                     
     If the two players get a brelan the highest **BRELAN** decide which is the
     winner.                                                               
     It's impossible that the two players get the same **BRELAN** at the same  
     time in a 32 cards game (from *7* to *Ace*).                              
                                                                           
  8. **TWO PAIRS**
                                                           
     2 times 2 sames cards from the same value.                            
     In case the two players get **TWO PAIRS** the highest value pair is compared
     and the highest value decide which is the winner. In case the highest 
     pair is from the same value we compare the lowest value pair to decide
     which is the winner.                                                  
     In case the 2 players get exactly the same **TWO PAIRS** combination we   
     compare the value of the resting card to decide which is the winner.  
                                                                           
  9. **PAIR**
                                                                
     2 same cards from the same value.                                     
     In case the tow players get the same value pair we compare the highest
     resting card to decide which is the winner. If a winner cannot be found
     there is an egality.                                                  
                                                                           
  10. **NOTHING**
                                                            
      No one of the combination. To decide which is the winner we compare the
      cards and the highest card decide which is the winner.               
      If no winner is found there is an egality.                           


Notes
-----

 By **CPocker** the computer, throw card algorithm and so, the computer strategie
 is implemented likewise his creator play poker.                           
                                                                           
   **So it is like you play poker against me !!!**                             
                                                                           
 I implement this game by taking care at the respect of the player in sense
 that the computer doesn't not never know what you get in hand before      
 comparing to take advantage of it for computing what cards the computer   
 will throw. And the computer doesn't know which cards are coming next from
 the distributing heap to cash in on.                                      
                                                                           
 I take care of:                                                           
                                                                           
 - Right mixing the cards before every round.                             
                                                                           
 - Respect of the cards distributing order which is inverted every round. 
                                                                           
 - To set the throwed cards under the heap after gathering it all after a 
   round.                                                                 
                                                                           
 By assured that the game is honest with the player.                       
 What i be in life with everyone and i hope you do so too.                                                                                 

Copyright
---------                                

 This programm is under copyright from the GPL GNU GENERAL PUBLIC LICENSE  

                

