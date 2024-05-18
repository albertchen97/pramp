# [Event Emitter](https://www.pramp.com/challenge/bKxy5GyazrSbWQGLQzMJ)

Implement an EventEmitter that supports standard operations, such as adding and removing listeners and emitting events by topic.

## Starter Code

```javascript
// Add your implementation here, and initialize eventEmitter with an actual value;
var eventEmitter = undefined;

function responseToEvent(msg) {
    console.log(msg);
}

eventEmitter.on('pramp', responseToEvent);
eventEmitter.once('pramp', function(msg) { console.log(msg + ' just once!'); });
eventEmitter.emit('pramp', '1st');
eventEmitter.emit('pramp', '2nd');
eventEmitter.off('pramp', responseToEvent);
eventEmitter.emit('pramp', '3rd');
eventEmitter.emit('pramp', '1st');
```
