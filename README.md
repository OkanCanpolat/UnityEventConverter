# UnityEventConverter

In Unity you can add a UnityEvent to a random script and then you can see it on the Inspector (if it is public or Serializefiled attribute added on it). Lets say you add some listeners to UnityEvent named "MyEvent" and you want these listeners to pass to the dynamically created UI button OnClick Event.

You can not simply pass the "MyEvent" to the UI Button's OnClick Event. Becasue OnClick Event only accept UnityAction type parameter not the UnityEvent. 

So somehow we must get the listeners from the "MyEvent". This script will help you to get listeners from an UnityEvent and convert them to UnityAction type. Thus you can add these UnityActions to the dynamically created UI button.
## Note: You should add only parameterless listeners to the UnityEvent on the Unity Inspector.
