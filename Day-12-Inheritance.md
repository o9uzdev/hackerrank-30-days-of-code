# Day 12: Inheritance

https://www.hackerrank.com/challenges/30-inheritance

```java
class Student extends Person{

    protected int id;
	private int[] testScores;
    
    public Student(String firstName, String lastName, int id, int[] scores){
        super(firstName, lastName, id);
        this.testScores = scores;
    }
    
    public char calculate(){
        int average = 0;
        for(int i = 0; i < testScores.length; i++){
            average += this.testScores[i];
        }
        average = average / testScores.length;
        if( 90 <= average && average <= 100 ){
            return 'O';
        } else if( 80 <= average && average < 90 ){
            return 'E';
        } else if( 70 <= average && average < 80 ){
            return 'A';
        } else if( 55 <= average && average < 70 ){
            return 'P';
        } else if( 40 <= average && average < 55 ){
            return 'D';
        } else {
            return 'T';
        }
    }
}
```