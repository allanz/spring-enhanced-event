spring-enhanced-event
=====================

Provide enhanced way to fire events or observer events.

1.Fire event.

Events.instance().fire("eventKey",arg1,arg2....);

2.Observer event

If you want to observer an event fired by fireXX in Events:

@Observer("eventKey")
public void someOvserver(Type1 arg1,Type2 arg2...){
  //balabalabala
}

If youwant to observer an event published by spring:

@Observer(type=EventType.class)
public void someOvserver(EventType event){
	//balabalabala
}

