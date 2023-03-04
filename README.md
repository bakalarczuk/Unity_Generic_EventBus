# Generic Event Bus In Unity

An event bus is a pipeline of events where the publisher triggers an event and subscribers receive that event and act accordingly.

Just write the following codes in your desired classes. It is highly recommended to put the start listening call in OnEnable and put the stop listening in the OnDisable function.

```
//Trigger Event
EBM.TriggerEvent<THEME>(EventBusEnum.EventName.THEME_CHANGE, THEME.WHITE);
//Start Listening 
EBM.StartListening<THEME>(EventBusEnum.EventName.THEME_CHANGE, OnThemeChanged);
//Stop Listening 
EBM.StopListening<THEME>(EventBusEnum.EventName.THEME_CHANGE, OnThemeChanged);
```

[Detailed description in Medium](https://habibur-rahman-ovie.medium.com/generic-event-bus-in-unity-7e8a35dffcce)

[Linkedin]([https://habibur-rahman-ovie.medium.com/generic-event-bus-in-unity-7e8a35dffcce](https://www.linkedin.com/in/habibur-rahman-32547b109/))

[If you want you can support me here](patreon.com/CaptainNemo288)
