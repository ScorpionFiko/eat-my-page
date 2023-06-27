# EatMyPage


## Description

Repository containing the code for the EatMyPage applicaton on Scratch. This is a game where out main hero Sprite must skip along the pane and eat the apples that are arranged in a QR code representing an actual live webpage for my woodworking business https://www.kokabora.com (go ahead and scan it...). The goal of the game is to score as many points as possible during the allotted time.  


Below is the image of game at start up.
![ECP - Landing](./assets/images/ECP-01-cart.png)

Below is the image of game during game play
![ECP - Landing Logged In](./assets/images/ECP-02-cart-logged-in.png)

Below is the image of game when completed
![ECP - Checkout](./assets/images/ECP-03-checkout.png)




## Table of Contents

- [Installation](#installation)
- [Gameplay](#gameplay)
- [Functionality](#functionality)
- [Credits](#credits)
- [Tests](#tests)
- [License](#license)
- [Future Development](#future-development)
- [Contact](#contact)

## Installation

No special installation requirements. Simply visit https://stefans-ecommerce-platform.herokuapp.com/ to use the application.


back to [Table of Contents](#table-of-contents)


## Gameplay

Use the Arrow keys to move Sprite on the board. 

Info on QR apples (or dots):
- Red Apples: those are the regular apples that are edible from the get-go. They contribute 1 point to your score. But there's a twist: somewhere in between 60 to 120 seconds, the eaten apples reappear reducing your score by 1.
- Purple Apples: those are mystery apples and are not edible from the start. You need to accumulate somewhere in between 300 and 400 points before the apples become edible and turn green. However if your score goes below the random threshold, the apples will become inedible again (and turn purple). The mystery apples do not reappear after they have been eaten, but their mystery lies in the fact that eating them can either increase your score (a varied level of deliciousness) or decrease it (a varied level of rot). 



back to [Table of Contents](#table-of-contents)


## Functionality

The following discusses at a high level about some of the features of the game. 


### Apple Sprites:

The apples were quite simple Sprites to develop and use. The trickiness comes from the fact that they are over 500 of them all following a particular grid structure. In most cases "global" variables were used and initialized in the cat Sprite in order to facilitate quicker updates to the game play.

### Cat Sprite:

The cat sprite was developed in such a way to simulate movement (i.e. skipping) along the pane. The skipping is done in the left and right direction as well as up an down direction. No diagonal costumes have been used so pressing horizontal and vertical direction keys at the same time is not going to have a proper 45 degree sprite movement (for the time being).

In addition to the movement, Sprite is made to bounce of the edge of the pane as well as bounce of inedible apples. 


back to [Table of Contents](#table-of-contents)



## Credits
PAC-MAN was the inspiration of the game, but it has a few twist to make it different. The only similar thing at this point is the "edibles"; aside from that, the current game involves 
- reappearing apples
- mystery apples that:
    - require the accumulation of a particular threshold before they are edible
    - can potentially reduce your score
- no enemies to chase Sprite

back to [Table of Contents](#table-of-contents)


## Tests

All tests have been performed manually using Chrome.

back to [Table of Contents](#table-of-contents)


## License

Please refer to the LICENSE in the repo.

back to [Table of Contents](#table-of-contents)


## Future Development

Here are some of the items to be considered for future development.
1. Diagonal costumes and movement when a combination of a horizontal and vertical arrow buttons have been pressed.
2. Introduction of speed. In other words, the more Sprite eats, the faster Sprite becomes and the distance travelled with a single click of a button become more than the starting 5 pixels. Similarly if apples reappear, Sprite's energy level drops and becomes slower. The game has the groundwork for it, however, initial tests showed an extreme speed increase after eating more than 100 apples and that makes Sprite uncontrollable.
3. Themed background that's somewhat different than a single colour. This needs further consideration as the QR still needs to be scannable regardless of the background.
    

back to [Table of Contents](#table-of-contents)


## Contact
Stefan Marinov
stefan@marinovnet.com

back to [Table of Contents](#table-of-contents)