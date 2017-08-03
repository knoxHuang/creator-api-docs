## `FiniteTimeAction` Class

Extends [`Action`](Action.md)


Module: [cc](../modules/cc.md)




Base class actions that do have a finite time duration. <br/>
Possible actions: <br/>
- An action with a duration of 0 seconds. <br/>
- An action with a duration of 35.5 seconds.

Infinite time actions are valid

### Index



##### Methods

  - [`getDuration`](#getduration) get duration of the action. (seconds).
  - [`setDuration`](#setduration) set duration of the action. (seconds).
  - [`reverse`](#reverse) Returns a reversed action. <br />
For example: <br />
- The action will be x coordinates of 0 move to 100. <br />
- The reversed action will be x of 100 move to 0.
- Will be rewritten
  - [`clone`](#clone) to copy object with deep copy.
returns a clone of action.
  - [`isDone`](#isdone) return true if the action has finished.
  - [`getTarget`](#gettarget) get the target.
  - [`setTarget`](#settarget) The action will modify the target properties.
  - [`getOriginalTarget`](#getoriginaltarget) get the original target.
  - [`getTag`](#gettag) get tag number.
  - [`setTag`](#settag) set tag number.



### Details




<!-- Method Block -->
#### Methods


##### getDuration

get duration of the action. (seconds).

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:200](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L200) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### setDuration

set duration of the action. (seconds).

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:210](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L210) |

###### Parameters
- duration <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 


##### reverse

Returns a reversed action. <br />
For example: <br />
- The action will be x coordinates of 0 move to 100. <br />
- The reversed action will be x of 100 move to 0.
- Will be rewritten

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:220](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L220) |
| Return 		 | Null 



##### clone

to copy object with deep copy.
returns a clone of action.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:236](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L236) |
| Return 		 | <a href="../classes/FiniteTimeAction.html" class="crosslink">FiniteTimeAction</a> 



##### isDone

return true if the action has finished.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:65](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L65) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">Boolean</a> 



##### getTarget

get the target.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:97](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L97) |
| Return 		 | <a href="../classes/Node.html" class="crosslink">Node</a> 



##### setTarget

The action will modify the target properties.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:107](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L107) |

###### Parameters
- target <a href="../classes/Node.html" class="crosslink">Node</a> 


##### getOriginalTarget

get the original target.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:117](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L117) |
| Return 		 | <a href="../classes/Node.html" class="crosslink">Node</a> 



##### getTag

get tag number.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:134](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L134) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### setTag

set tag number.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js:144](https:/github.com/cocos-creator/engine/blob/master/cocos2d/actions/CCAction.js#L144) |

###### Parameters
- tag <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 


