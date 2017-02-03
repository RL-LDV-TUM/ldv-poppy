The MoveDemo is a basic programm to play several recorded movements.


The File starts with the standard initialization section:
```python
# Initialize the robot
from poppy.creatures import PoppyHumanoid
from pypot.primitive.move import MoveRecorder, MovePlayer, Move

poppy = PoppyHumanoid()
```

In the next section the different movements are loaded
```python
# Load recoreded movements
with open('movements/hello.move') as f:
    hello_move = Move.load(f)
    
with open('movements/posing.move') as f:
    posing_move = Move.load(f)
    
(...)
```

The following sections start or stop a certain movement. When the cursor is set in a cell you can execute the cell by hitting *Crtl* and *Return*:
```python
# Stand still
poppy.stand_position.start()
```
```python
# IDLE Motion Start
poppy.upper_body_idle_motion.start()
poppy.head_idle_motion.start()
```
```python
# IDLE Motion Stop
poppy.upper_body_idle_motion.stop()
poppy.head_idle_motion.stop()
```
```python
# Stand still
poppy.stand_position.start()
```
```python
# Cross Your Arms
player = MovePlayer(poppy, cross_move)
player.start()
```
```python
# Greet People
player = MovePlayer(poppy, salut_move)
player.start()
```
```python
# Shake Hands
player = MovePlayer(poppy, shake_move)
player.start()
```
```python
# Say YES
player = MovePlayer(poppy, yes_move)
player.start()
```
```python
# Say NO
player = MovePlayer(poppy, no_move)
player.start()
```
```python
# Start Copy Motion (Left --> Right)
poppy.arms_copy_motion.start()
```
```python
# Stop Copy Motion
poppy.arms_copy_motion.stop()
```
```python
# Dub
player = MovePlayer(poppy, dance_move)
player.start()
```
```python
# Do the Robot Dance
player = MovePlayer(poppy, robot_move)
player.start()
```
