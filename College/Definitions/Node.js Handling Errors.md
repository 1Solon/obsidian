![[Pasted image 20231011151930.png]]
> » Errors can be especially troublesome when they occur in an EventEmitter. « If we do not have a listener registered to handle an error event, a stack trace will be printed and the process will exit. » Therefore, it is good coding practice to have a listener for an error event. + Take a copy of https://github.com/paul-kelly-dit/web-application- architecture/blob/master/week6/nodejs/event-transmitter-error-handling.js and run » Does not seem much different from our previous code example, it should be noted that the error events are special and need to be handled. » Try to emit an error event in the first code example and see what happens.