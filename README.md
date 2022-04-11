# kaboom-animations
a repo i use to host things for kaboom (use https://kaboom-animations.dainfloop.repl.co to see all of these used)

## how to use?
create a new folder and the following files must be in it:
- sprite.png (the sprite of your character)
- atlas.json (sprite data) (should be a [SpriteAtlasEntry](https://kaboomjs.com/#SpriteAtlasEntry))  
animation names for atlas.json should be a [Key](https://kaboomjs.com/#Key) string, with one being called "idle" for no buttons pressed. If there is a movement sprite, name it "move" and it will automatically be rotated when either left or right is pushed.
- create a pr with it

example (no animations):

- sprite.png  
![bean](https://cdn.jsdelivr.net/gh/replit/kaboom/src/assets/bean.png)  

- atlas.json
```json
{} // leave it empty!
```  

example (has animations):

- sprite.png ([https://deadrevolver.itch.io/pixel-prototype-player-sprites](https://deadrevolver.itch.io/pixel-prototype-player-sprites))  
![pixel-prototype-player-sprites](https://cdn.jsdelivr.net/gh/dainfloop/kaboom-animations/pixel-prototype-player-sprites/sprite.png)  

- atlas.json
```json
{
  "sliceX": 14,
  "sliceY": 18.9,
  "anims": {
    "idle": {
      "from": 14,
      "to": 20
    },
    "movement": {
      "from": 42,
      "to": 49
    },
    "up": {
      "from": 113,
      "to": 117
    },
    "w": {
      "from": 113,
      "to": 117
    },
    "space": {
      "from": 113,
      "to": 117
    },
    "down": {
      "from": 127,
      "to": 131
    },
    "s": {
      "from": 127,
      "to": 131
    }
  }
}
```
