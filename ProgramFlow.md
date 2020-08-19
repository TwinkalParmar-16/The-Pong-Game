# Functions

## Start 
   ### Variables
   - Username
   - Password
   ### Methods
   - signIn(){
     <br/> Enter username and password
     <br/>authenticateUser()
    }
   - signUp(){
     <br/> Enter username and password
     <br/>authenticateUser()
   }
   - authenticateUser(){
   <br/> Matches with database
   <br/> Go to next activity
   }
  
## Player Class
   ### Variables
   - name
   - score
   - is_my_turn
   ### Abstract Methods
   - upOperation()
   - downOperation()
   - missedBall()
   - notMissedBall()
   - toggle()
   ### Methods
   - updateScore(){
   <br/> score = score+1
   }
   - resetScore(){
   <br/> score =0
   }

## Style Class
   ### Variables
   - display_name
   - color_of_bar
   - color_of_ball
   - background_color
   ###  Methods
   - chooseFontStyle()
   - chooseColor()
   
## Player1 Class
   Inherits Player Class and Style Class
   ### Impelentation of abstract Methods from Player class
   - upOperation(){
    <br/> use up key
   }
   - downOperation(){
    <br/> use down key}
   - missedBall(){
    <br/> player2.updateScore()
   }
   - notMissedBall(){
    <br/> changeDirection()
    <br/> toggle()
   }
   - toggle(){
   <br/> player1.is_my_turn=false
   <br/> player2.is_my_turn=ture
   }

## Player2 Class
   Inherits Player Class and Style Class
   ### Impelentation of abstract Methods from Player class
   - upOperation(){
    <br/>  use W key
   }
   - downOperation(){
    <br/>  use S key}
   - missedBall(){
    <br/> player1.updateScore()
   }
   - notMissedBall(){
    <br/> changeDirection()
    <br/> toggle()
   }
   - toggle(){
   <br/> player2.is_my_turn=false
   <br/> player1.is_my_turn=ture
   }
  
## Fuctions
   - stop(){
    <br/>  if(player1.score==5 or player2.score==5)
    <br/> then
    <br/> declareWinner()
    <br/> exit()
   }
   - declareWinner(){
    <br/>  if(player1.score > player2.score)
    <br/>  then
    <br/> Display Winner is player1.name
    <br/> if(player2.score > player1.score)
    <br/> then
    <br/> Display Winner is player2.name
    <br/> else
    <br/> Display Tie
   }
   - quit(){
   <br/> player1.resetScore()
   <br/> player2.resetScore()
   <br/> exit()
   }
   - sessioExpeired(){
   <br/> after fixed time period
   <br/>Show session Experied
   <br/> quit()
   }

   
    
 
   
   

  
   
