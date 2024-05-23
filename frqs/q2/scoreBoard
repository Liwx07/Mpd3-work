public class Scoreboard {
  private String t1;
  private String t2;
  private int s1;
  private int s2;
  private int active;

  public Scoreboard(String n, String n2){
    t1 = n;
    t2 = n2;
    s1 = 0; 
    s2 = 0;
    active = 1;
  }
  
  public String getScore(){
    String name = "";
    if(active == 1){
      name = t1;
    }
    else if(active == 2){
      name = t2;
    }
    return s1 + "-" + s2 + "-" + name;
  }

  public void recordPlay(int s){
    if(active == 1){
      if(s != 0){
        s1 += s;
      }
      else{
        active = 2;
      }
    }
    else{
      if(s != 0){
        s2 += s;
      }
      else{
        active = 1;
      }
    }
  }

}
