<style>
code {
  font-family: Consolas,"courier new";
  background-color: #f1f1f1;
  padding: 2px;
  font-size: 105%;
}
</style>
2022:
 - 0.1.4a:
   - Added support for sprite and image rendering/drawing.
 - 0.2.0a | Codename: Seedling:
   - Added keyboard input support. 
     From a inheriated `Application` class, you can check for keys, like e.g. space button, like this: 
     ```cpp
     if (this->KeyPressed(SDLK_SPACE)) 
         square.position.y += 10;
     ```
     <br>
     Returns: Either `true` or `false` depending on pressed keys.
    - Fixed issue with SDL_Surface and sprite code, which crashed the game after close of the game.
    
    - Deleted away `Size` class, replaced with `Vector2`
    
    - Updated SDL -  2. 2.24.0