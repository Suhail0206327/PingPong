# PingPong

Welcome to the PingPong documentation. We all know that ping pong is a favorite game of all time. Here I will walk you through how I made this game.

## Steps for making the game :

  1. We need a ball, a paddle.
  2.  The ball should be moving within the screen and should bounce back when it touches the edges.
  3.  The paddle movement should be controlled by the user. The paddle movement is linear it just moves to and fro on the x-axis.
  4.  When the ball hits the paddle it should increase the score and it should bounce back.
  5.  When the ball misses the paddle and hits the southern edge it should stop the ball and display the message game over.
  6.  The user should be able to start a new game after the game is over.

     1. So here a canvas is used in the screen1 and a ball sprite and an image sprite are added. An image made using Microsoft Paint is used for the paddle.
     2. To make the ball move its speed is set to 10, then in the block the when the ball reached edge block is used and then calling the bounce function which bounces the ball back according to the edge.
     3. To mage the paddle move, there are two buttons left and right. And we are using the funcion when the button is clicked we are changing the x value. That is when it is pressed left the x value is decreased in a specific rate and when the right button is pressed the x value is increased. More over to make the paddle down in the bottom of the screen we are using the screen initialize function and setting the paddles y coordinate to the canvas height.
     4. So first a global variable called score is declared and initialized to zero. And the function when ball collided with is used where setting the paddle as the other. Then the balls heading is changed to 360 - current ball heading, which means doing a full turn and making its heading to exact opposite one. Then the global variable score is increased by one when collided with the paddle.
     5. So in the block when ball reaches the edge an if loop is used inside and then we are getting the edge and checking if the edge is -1. Here in MIT app inventor the top, right, bottom and left edges are denoted by 1, 3 , -1 and 3. So when the ball reaches the edge with the value -1 the ball is disabled and a message is shown as "game over".
     6. Anytime when the user touches the ping pong button the game is rest. This is achieved by setting the when clicked block of PingPong button and doing the score change and enabling the ball along with changing its position to the top right corner.


     This game is pretty straint forward one i used one procedure here to update the score that will add one when ever it is called 
         
