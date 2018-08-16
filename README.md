# designPatternsJava
Singleton Pattern

public class Singleton {

private static Singleton instance;

private Singleton(){
  // as the constructor is private can't be a subclassed by any class
}

public static void getInstance(){

  if(instance == null){
      synchronised(this){
        if(instance == null)
          instance = new Singleton()
      } // synchronised closed
    } // if condition closed
    return instance;
  }// main close 
  
  .... other static functions
  
}// class close


-----------------------------------------------------------------------------------------

