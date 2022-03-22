%%%%%%%%PSEUDO%%%%%%%%%%%

#include "humppila"
 
#include "forssa"
 
#include "tampere"
 
 
void setupFunc()
{
    me = new humppilaJäbä();
    me.name = Leevi;
    timer thougthDog = new timer(1000);
    thoughtDog.enable();
}

void main()
{
     me.wakeUp();
     me.hunger = checkHunger()
     if(hunger > 50 && day.time = morning)
      me.actionToRun = eat(foodType.breakfast)
     else if(hunger > 50)
      me.actionToRun = eat(something);
     
    if(!day.weekendQuery())
      me.actionToRun = goToWork();
    if(day.weekendQuery())
      me.actionToRun = NOYB();
  }
  
  ISR_internalClock(thoughtDogOverflow)
  {
    if(!me.taskList.Empty)
      exeucuteAction();
  }
