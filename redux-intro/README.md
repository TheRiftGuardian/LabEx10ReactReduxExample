Hello, my application is a counter similar to the one done in the lab recording. I have used react redux to accomplish this. 
By using the redux fundamentals:
Redux
0 - State
1 - Store
2 - Reducer
3 - Action
4 - Dispatch
5 - Subscribe
We are able to make this application work properly.

Our main object is to create a counter that increases and decreases on button click in real-time. This means it'll get updated on every change and displays that change.

We first create a state for the counter with an initial state of 0. In our Counter.js we would then have a function that returns the current states.count. This will be later used to update Counter.

We would then create a store with our reducer as a constant called store. Our reducer function will take two parametrs, being the initial state which was zero and action. Inside this function is a switch statement that will determine the action type, if its increment the count will increase by 1 and if its decrement the count will decrease by 1. The dispatch will provide the type and the action would occur. 

Finally, our subscribe, which connect is implemented with is used to watch and listen for changes in the counter state. Once it detects a change it will then tell react to redraw/redisplay the information and that is why the application is updated in real-time.