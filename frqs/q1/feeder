public class Feeder{
  private int currentFood;

  public Feeder(int f){
    currentFood = f;
  }

  public void simulateOneDay(int numBirds){
    int food = (int) (Math.random()*41 + 10);
    if(Math.random() > 0.95){
      if(currentFood - (numBirds*food) > 0){
        currentFood = currentFood - (numBirds*food);
      }
      else{
        currentFood = 0;
      }
    }
    else{
      currentFood = 0;
    }
  }

  public int simulateManyDays(int numBirds, int numDays){
    int count = 0;
    for(int i = 0; i < numDays; i++){
      simulateOneDay(numBirds);
      if(currentFood > 0){
        count++; 
      }
      else{
        return count;
      }
    }
    return count;
  }
  
}
